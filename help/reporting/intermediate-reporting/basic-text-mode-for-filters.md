---
title: 瞭解篩選器的基本文字模式
description: 瞭解您可以在Workfront的報告篩選器中使用的文字模式、駝峰式大小寫和一些基本文字模式。
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: 2025-07-30T00:00:00Z
jira: KT-9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
doc-type: video
source-git-commit: cc423944628d01e16d390842ecb25696505f923c
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 90%

---

# 了解篩選器的基本文字模式

>[!PREREQUISITES]
>
>* [了解報告元素](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-elements.html?lang=zh-hant)
>* [了解報告元件](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-components.html?lang=zh-hant)
>* [建立基本篩選器](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/basic-text-mode-for-filters.html?lang=zh-hant)


>[!TIP]
>
>* 為了深入了解文字模式，我們建議觀看錄影版網路研討會活動「[詢問專家 - 文字模式報告簡介](https://experienceleague.adobe.com/en/docs/events/classics/reporting-and-dashboards/introduction-to-text-mode-reporting)」，影片長度為 1 小時。
>* 若要更加深入了解文字模式，我們建議觀看「[進階報告](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=zh-hant)」教學課程，全部課程總長 5 個半小時。
>* 按一下此處以存取 [[!UICONTROL API Explorer]](https://developer.adobe.com/workfront/api-explorer/)


在這段影片中，您將了解以下內容：

* 文字模式
* 駝峰式大小寫
* 您可以用在報表篩選中的某些&#x200B;_文字模式程式碼區塊_

>[!VIDEO](https://video.tv.adobe.com/v/3470329/?captions=chi_hant&quality=12&learn=on&enablevpops=0)

## 「了解篩選器的基本文字模式」活動


### 任務 - 將我已標記為「已完成我的部分」的工作篩除

以下文字模式將會排除使用者已標記為「已完成我的部分」的任務。您只需要建立一個任務篩選器，新增任何想要的篩選規則，然後切換到文字模式，並把下列程式碼貼到您在篩選器中看到的任何文字模式之後。


>[!WARNING]
>
> 這不適用於行事曆篩選器。

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

### 任務 - 顯示所有等待我核准的任務

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

### 任務 - 顯示所有我已核准的任務

使用任何您想要的篩選器來建立任務報告，然後前往「篩選器」標籤並按一下「切換到文字模式」。把這段程式碼新增到任何原有內容之中：

```
approvalProcessID_Mod=notblank
approverStatuses:approvedByID=$$USER.ID
approverStatuses:approvedByID_Mod=in
```

### 任務 - 顯示至少擁有一項跨專案前置任務的所有任務

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

### 任務 - 顯示我指派給其他人的任務

使用任何您想要的篩選器來建立任務報告，然後前往「篩選器」標籤並按一下「切換到文字模式」。把這段程式碼新增到任何原有內容之中：

>[!WARNING]
> 
> 這不適用於行事曆篩選器。

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

這樣將會顯示已登入使用者至少指派其中一位目前受指派者的所有任務。如果受指派者由多名人員指派，只有進行指派的第一個人的名稱會在任務登陸頁面中顯示為「請求者」。

### 任務 - 顯示所有已完成 - 待核准的任務

```
status=CPL:A
status_Mod=in
```


### 問題 - 顯示所有已完成 - 待核准的問題

```
status=CPL:A
status_Mod=in
```


### 專案 - 顯示所有已完成 - 待核准的專案

```
status=CPL:A
status_Mod=in
```


### 注意 - 顯示我被標記的所有註解

```
tags:userID=$$USER.ID
tags:userID_Mod=in
```


### 參數/自訂欄位報告 - 顯示未附加到自訂表單的自訂欄位 (在清除工作中十分實用)

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```
