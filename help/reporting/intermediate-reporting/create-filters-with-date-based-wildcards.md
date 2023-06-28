---
title: 使用日期型萬用字元建立篩選器
description: 瞭解如何使用及何時使用日期型萬用字元，以及如何根據目前日期建立篩選器。
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
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# 使用日期型萬用字元建立篩選器

在本影片中，您將瞭解如何：

* 瞭解何時使用日期型萬用字元
* 瞭解Workfront兩個日期型萬用字元的差異
* 將日期型萬用字元新增至篩選器
* 使用萬用字元、屬性、運運算元和修飾元建立自訂日期
* 使用萬用字元建立自訂日期範圍

>[!VIDEO](https://video.tv.adobe.com/v/336812/?quality=12&learn=on)

## 活動問題

1. 如果您想要有到期日為昨天或今天的問題，該如何建立篩選規則？
1. 如何建立篩選規則來尋找上週到期的專案？
1. 下列篩選規則是您定期使用的任務報告的一部分。 您會從此報告獲得什麼型別的結果？

![使用日期型萬用字元建立任務篩選的畫面影像](assets/date-wildcard-answer-1.png)

## 答案

1. 篩選介於以下日期的問題計畫完成日期： [!UICONTROL $$TODAY-1d] 和 [!UICONTROL $$TODAY].
1. 篩選介於以下範圍的專案計畫完成日期： [!UICONTROL $$TODAYb-1w] 和 [!UICONTROL $$TODAYe-1w].
1. 此報表會尋找指派給您的尚未完成（換句話說，完成百分比小於100）且今天即過期或到期的任務。 任務的計畫完成日期的篩選規則表示，檢視到期日等於或早於今天日期的任務。
