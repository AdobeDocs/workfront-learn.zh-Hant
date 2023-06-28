---
title: 瞭解篩選器的基本文字模式
description: 瞭解什麼是文字模式、什麼是駝峰式大小寫，以及可以在Workfront的報告篩選器中使用的一些基本「隨插即用」文字模式。
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# 瞭解篩選器的基本文字模式

>[!IMPORTANT]
>
>先決條件：
>
>* 瞭解報表元素
>* 瞭解報表元件
>* 建立基本篩選器

>[!TIP]
>
>* 若要更深入地瞭解文字模式，我們建議您觀看錄製的網路研討會活動 [詢問專家 — 文字模式報告簡介](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=en)，長度為一小時。
>* 若要進一步瞭解文字模式，建議您觀看 [進階報告](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) 教學課程，總共有五個半小時的長度。


在本影片中，您將瞭解：

* 什麼是文字模式
* 什麼是駝峰式大小寫
* 您可以在報表篩選器中使用的基本「隨插即用」文字模式

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12&learn=on)


## 任務 — 篩選掉我已標籤「已完成我的部分」的任務

下列文字模式將排除使用者已標示「已完成我的零件」的任務。 您只需要建立一個任務篩選器，新增任何您想要的篩選器規則，然後切換到文字模式，並在您在篩選中看到的任何文字模式之後貼上下列程式碼。

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

## 任務 — 顯示所有等待我核准的任務

```
approvalProcessID_Mod=notblank
currentUserApproversMM:ID=$$USER.ID
currentUserApproversMM:ID_Mod=in
currentUserApproversMM_Join=allowingnull
```

## 任務 — 顯示我已核准的所有任務

使用您想要的任何篩選器建立任務報告，然後前往「篩選器」索引標籤，按一下「切換到文字模式」。 將此程式碼新增至已有的任何專案：

```
approvalProcessID_Mod=notblank
approverStatuses:approvedByID=$$USER.ID
approverStatuses:approvedByID_Mod=in
```

## 任務 — 顯示至少有一個跨專案前置任務的所有任務

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

## 任務 — 顯示我指派給其他人的所有任務

使用您想要的任何篩選器建立任務報告，然後前往「篩選器」索引標籤，按一下「切換到文字模式」。 將此程式碼新增至已有的任何專案：

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

這會顯示登入使用者至少指派一個目前受指派人的所有任務。 如果受指派人是由多個人員指派，則只有指派人員的第一個人員的姓名會在任務登陸頁面上顯示為「請求者」。

## 任務 — 顯示所有完成的任務 — 未決核准

```
status=CPL:A
status_Mod=in
```


## 問題 — 顯示所有完成的問題 — 未決核准

```
status=CPL:A
status_Mod=in
```


## 專案 — 顯示所有完成的專案 — 未決核准

```
status=CPL:A
status_Mod=in
```


## 注意 — 顯示我已標籤的所有註解

```
tags:userID=$$USER.ID
tags:userID_Mod=in
```


## 引數/自訂欄位報告 — 顯示未附加至自訂表單的自訂欄位（在清除工作中非常有用）

```
EXISTS:A:$$EXISTSMOD=NOTEXISTS
EXISTS:A:$$OBJCODE=CTGYPA
EXISTS:A:parameterID=FIELD:ID
```
