---
title: 瞭解現有的篩選器
description: 瞭解「存在」篩選器是什麼、它可以對您做什麼，以及如何從頭開始建立篩選器。 此外，您還能看到許多「存在」篩選器的實用範例。
activity: use
team: Technical Marketing
feature: Reports and Dashboards
type: Tutorial
role: User
level: Intermediate
jira: KT-1880
last-substantial-update: 2025-08-25T00:00:00Z
doc-type: video
source-git-commit: 7be0b8cce9cba04927d6704d0009b482bbcf4b41
workflow-type: tm+mt
source-wordcount: '682'
ht-degree: 0%

---

# 瞭解現有的篩選器

「存在」篩選器是進階的文字模式篩選器，可讓我們在標準Report Builder中繞過2個表格/欄位跳轉限制。 或者，它們可用於透過NOTEXISTS識別系統中缺少特定關係條件的物件。

在本影片中，您將瞭解如何建立存在篩選器，以在校訂核准報告中檢視「目前專案的校訂核准」。

如需有關EXISTS函式的更深入逐步解說，請參閱[使用EXISTS陳述式建立複雜的文字模式篩選器](https://experienceleague.adobe.com/en/docs/workfront/using/reporting/reports/text-mode/create-complex-text-mode-filters-using-exists-statements)檔案。

>[!VIDEO](https://video.tv.adobe.com/v/3471181/?quality=12&learn=on&enablevpops)

## EXISTS篩選範例

### 專案報告存在

透過比較在任務層級找到的projectID並將其與專案層級ID欄位比對，這會使用任務作為連結物件。 這可讓我們比較任務上的工作分派使用者與$$USER.ID萬用字元。 這會導致只傳回檢視使用者被指派到的專案
工作，無論他們是否為主要受指派人。

```
EXISTS:A:$$OBJCODE=TASK
EXISTS:A:assignmentsUsersMM:ID=$$USER.ID
EXISTS:A:assignmentsUsersMM:ID_Mod=in
EXISTS:A:projectID=FIELD:ID
```


這會使用問題(optask)作為連結物件，方法也是比較在問題(optask)層級找到的專案ID，並將其與專案層級ID欄位進行比對。 然後會檢查是否有任何這些問題(optasks)的進入日期在指定的範圍內。 在此情況下，它會傳回任何具有
由於NOTEXISTS，在過去30天內沒有記錄問題(optask)。

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=OPTASK
EXISTS:A:entryDate=$$TODAY
EXISTS:A:entryDate_Mod=between
EXISTS:A:entryDate_Range=$$TODAY-30d
EXISTS:A:projectID=FIELD:ID
```

### 範本報告已存在

此篩選器將顯示所有在過去一年中尚未用於建立專案或已附加至專案的範本。 需要注意的是，若要瞭解範本是否作為附件使用，須視範本中是否有任務而定。

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=TASK
EXISTS:A:entryDate=$$TODAY-1y
EXISTS:A:entryDate_Mod=gte
EXISTS:A:templateTask:templateID=FIELD:ID
EXISTS:B:$$EXISTSMOD=NOTEXISTS
EXISTS:B:$$OBJCODE=PROJ
EXISTS:B:entryDate=$$TODAY-1y
EXISTS:B:entryDate_Mod=gte
EXISTS:B:templateID=FIELD:ID
```

### 任務報告存在

這會使用「使用者」表格作為連結物件，由工作總攬taskID和任務ID連線。 接著會將ID的團隊集合檢查為使用者團隊ID，如果有任何受指派者與檢視使用者位於相同的團隊，則會傳回任務。

```
EXISTS:1:$$OBJCODE=USER
EXISTS:1:teams:ID=$$USER.teamIDs
EXISTS:1:userAssignments:taskID=FIELD:ID
```

### 使用者報告存在

這將傳回過去3週內未發佈更新的所有使用者。 這會使用Note物件來橋接間隙，並將ownerID與使用者ID進行比較。 然後，如果使用者擁有的筆記的輸入日期沒有超過3週前，則傳回該使用者。

```
EXISTS:A:$$OBJCODE=NOTE
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:ownerID=FIELD:ID
EXISTS:A:entryDate=$$TODAY-3w
EXISTS:A:entryDate_Mod=gt
```

這會傳回上週未記錄時數的所有使用者。 這會使用與上述範例極為類似的方法，相反會使用小時擁有者資訊和小時輸入日期來建立其傳回之使用者的基礎。

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=HOUR
EXISTS:A:entryDate=$$TODAY-1w
EXISTS:A:entryDate_Mod=gte
EXISTS:A:ownerID=FIELD:ID
```

在使用者報表中，顯示符合專案之「人員」索引標籤的使用者清單。

```
EXISTS:1:$$OBJCODE=PRTU
EXISTS:1:projectID=<projectID>
EXISTS:1:userID=FIELD:ID
```

### 類別（自訂表單）報告存在

此文字會提供您專案上從未使用過的所有專案表單清單。 這應該與指定我們著重關注的表單的物件型別結合使用。 因此在此案例中，焦點是「專案」，因此我們應將編號說明包含在objTypes行中。 可以使用此選項
對於其他物件型別，可透過變更物件程式碼相關部分來進行。 這會檢查附加表單至所清單單的專案集合，如果沒有相符專案，則會傳回。

```
EXISTS:A:$$OBJCODE=PROJ
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:objectCategories:categoryID=FIELD:ID
objTypes=PROJ
objTypes_Mod=in
```

### 引數（自訂欄位）報表存在

這會傳回目前未附加至系統中自訂表單的任何自訂欄位。

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```

### 報告報告存在

這將會傳回任何在其篩選器中使用特定值的報表。

```
EXISTS:1:$$OBJCODE=UIFT
EXISTS:1:ID=FIELD:filterID
EXISTS:1:preference:value=<value here>
EXISTS:1:preference:value_Mod=cicontains
```

這會傳回附加至任何控制面板的任何報告。

```
EXISTS:A:$$OBJCODE=PRTBSC
EXISTS:A:internalSectionID=FIELD:ID
EXISTS:A:portalTab:ID_Mod=notblank
```

### 校訂核准報告存在

這將只傳回對狀態為「目前」的專案的校訂核准。 這會使用Document物件，將currentVersionID核取至documentVersionID，藉此橋接從校訂核准到專案的間隙，從該處我們跳至專案狀態。

```
EXISTS:1:$$OBJCODE=DOCU
EXISTS:1:currentVersionID=FIELD:documentVersionID
EXISTS:1:project:status=CUR
EXISTS:1:project:status_Mod=in
```
