---
title: 根據專案時間表追蹤進度
description: 瞭解如何使用  [!DNL  Workfront]  的專案時間表藉由完成百分比、狀態、指派或限制來追蹤工作進度。
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: track-work-progress-from-the-project-timeline.jpeg
type: Tutorial
role: User
last-substantial-update: 2023-08-16T00:00:00Z
level: Beginner
jira: KT-10150
hide: true
source-git-commit: 609df4be7b1115b7b624d9e8e758845cd2a51bdb
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 100%

---

# 根據專案時間表追蹤進度

確保任務保持應有的進度，以便在專案截止期限前完成。當您瀏覽「[!UICONTROL 任務]」清單時，[!DNL  Workfront] 中有若干功能可協助您監視工作的進度和狀態。

## 完成百分比

有時候會利用每項工作任務的完成百分比來衡量工作進展。請注意...這個欄位必須手動調整，因為它是受指派人自行預估的進度。

>[!TIP]
>
>儘管工作任務的完成百分比需要手動更新，但父任務的完成百分比是由 Workfront 根據每個子任務的完成百分比以及期間或計劃小時數來計算的。這意味著，如果您將大型任務分解為較小的子任務，您會獲得更準確的完成百分比。


![專案任務清單顯示「[!UICONTROL 完成百分比]」欄](assets/planner-fund-task-percent-complete.png)

完成百分比在三種情況下會自動變更：

* 當任務「[!UICONTROL 狀態]」設定為「完成」，完成百分比變更為「100」。
* 如果任務「[!UICONTROL 狀態]」還原為「新增」，則完成百分比重設為「0」。
* 在父任務中，當子任務的完成百分比變更時。

## 狀態

在「[!UICONTROL 視圖]」中加入「[!UICONTROL 狀態]」欄，可快速查看哪項任務已開始、哪項進行中以及哪一項已完成。您甚至可以在「[!UICONTROL 視圖]」中使用條件式格式化為每個狀態指定一種顏色，讓資訊更容易解讀。

## 任務指派

當您檢閱專案時，請檢閱任務分配。可能因為未指派任何人執行任務所以進度落後。或者，受指派的人員可能不具備完成工作所需的適當技能。增加更多人來處理任務，或是重新指派任務以確保完成工作。

## 任務限制

有時候任務限制有所變更但您卻未發現。限制會影響時間表的運作，所以您應確定限制的設定是否符合您的要求。

![專案任務清單顯示任務限制欄](assets/planner-fund-task-constraint.png)

建立一個包含「[!UICONTROL 任務限制]」欄的自訂視圖，便能在任務清單中看到這項資訊。若您從開始日期進行專案規劃，則您想要設定「[!UICONTROL 盡可能最早] ([!UICONTROL ASAP])」的任務限制。

有關任務限制的更多資訊，請參閱「[了解和管理期間類型和任務限制](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/manage-work/intermediate-projects/understand-and-manage-duration-types-and-task-constraints.html)」。
