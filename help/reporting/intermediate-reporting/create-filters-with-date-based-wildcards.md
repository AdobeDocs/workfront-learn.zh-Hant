---
title: 建立含有日期型萬用字元的篩選器
description: 瞭解使用日期型萬用字元的方法和時機，以及如何根據目前日期建置篩選器。
activity: use
feature: Reports and Dashboards
thumbnail: 336812.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9082
exl-id: 0f7db4eb-a062-4eb3-99ca-c40d8e266943
doc-type: video
source-git-commit: 88c2161e897f23587ccc1d0e867b6f8961927a0f
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 71%

---

# 建立含有日期型萬用字元的篩選器

觀看這段影片，您將瞭解如何：

* 知道何時要使用日期型萬用字元
* 瞭解Workfront兩種日期型萬用字元的差異
* 新增日期型萬用字元到篩選器中
* 使用萬用字元、屬性、運算子和修飾元來建立自訂日期
* 使用萬用字元建立自訂日期範圍

>[!VIDEO](https://video.tv.adobe.com/v/336812/?quality=12&learn=on)


## 使用日期型萬用字元活動建立篩選器

[按一下這裡](/help/assets/create-filters-with-date-based-wildcards-activities.pdf)以下載此頁面的 PDF 版本。

### 活動問題

1. 如果您要把問題的截止日期設為昨天或今天，您該如何建置篩選規則？
1. 您要如何建置篩選規則來尋找上週到期的專案？
1. 以下篩選規則取自您經常使用的任務報告：您將從這份報告中得到什麼類型的結果？

![影像顯示使用日期型萬用字元建立任務篩選器的畫面](assets/date-wildcard-answer-1.png)

### 解答

1. 篩選介於 [!UICONTROL $$TODAY-1d] 和 [!UICONTROL $$TODAY] 之間的問題規劃完成日期。
1. 篩選介於 [!UICONTROL $$TODAYb-1w] 和 [!UICONTROL $$TODAYe-1w] 之間的專案規劃完成日期。
1. 此報表會尋找指派給您的尚未完成（換言之，完成百分比小於100）以及今天已過期或到期的任務。 任務的計畫完成日期的篩選規則表示，檢視到期日等於或早於今天日期的任務。
