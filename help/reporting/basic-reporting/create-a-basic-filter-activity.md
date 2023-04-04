---
title: 建立基本篩選活動
description: 在此活動中，您將建立名為「本月結束的專案」的專案篩選器。
activity: use
feature: Reports and Dashboards
thumbnail: 336807.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8856
exl-id: fc29b4ce-2937-478e-abd5-0b559657ead0
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# 建立基本篩選活動

在此影片中，您將建立名為「我擁有本月結束專案」的專案篩選器。 如果您持續關注許多專案，此篩選器可協助您放大顯示計畫近期結束的專案。

以下提供逐步指示。

>[!VIDEO](https://video.tv.adobe.com/v/336807/?quality=12&learn=on)

## 回答

![要建立新濾鏡的螢幕影像](assets/basic-filter-activity-updated-6-15-21.png)

1. 導覽至 [!UICONTROL 專案] 區域 [!UICONTROL 主菜單]. 這會顯示專案清單。
1. 按一下 **[!UICONTROL 篩選]** 選取 **[!UICONTROL 新增篩選]**.
1. 將篩選器命名為「我擁有本月結束的專案」。
1. 按一下 **[!UICONTROL 新增篩選規則]**.
1. 在 [!UICONTROL 開始鍵入欄位名稱] 欄位，鍵入「owner」。 然後選取 [!UICONTROL 擁有者ID] 在 [!UICONTROL 專案] 欄位來源。
1. 保留 [!UICONTROL 等於] 運算子。
1. 在「開始」鍵入名稱欄位中鍵入「$$」。
1. 選擇 [!UICONTROL $$USER.ID]. 這是登入使用者的萬用字元。
1. 按一下 [!UICONTROL 新增篩選規則] 。
1. 在 [!UICONTROL 開始鍵入欄位名稱] 欄位中，開始鍵入&quot;Is Complete&quot;。 然後選取 [!UICONTROL 已完成] 在「項目」欄位源下。
1. 保留 [!UICONTROL 等於] 運算子。
1. 選擇「False」。
1. 按一下 [!UICONTROL 新增篩選規則] 。
1. 在 [!UICONTROL 開始鍵入欄位名稱] 欄位類型「已規劃」，然後選取 [!UICONTROL 計畫完成日期] 在 [!UICONTROL 專案] 欄位來源。
1. 變更 [!UICONTROL 等於] 運算子到 [!UICONTROL 本月].
1. 按一下 **[!UICONTROL 儲存篩選]**
