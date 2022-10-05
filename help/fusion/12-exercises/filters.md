---
title: 篩選器
description: 了解如何使用模組之間的篩選器，以僅允許特定類型的套件組合穿過。
feature: Workfront Fusion
role: User
level: Beginner
kt: 11040
thumbnail: KT1101.png
source-git-commit: f367e016498d5c1814cab79e19e6e9001db2851f
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---


# 篩選器

了解如何使用模組之間的篩選器，以僅允許特定類型的套件組合穿過。

## 練習概觀

在「超出基本對應」案例中的兩個模組之間新增篩選器，以僅建立CSV檔案中具有「紅色」專案顏色的專案。

![篩選影像1](../12-exercises/assets/filters-walkthrough-1.png)

## 遵循步驟

1. 建立「超出基本對應」情境的複製項目，並將其命名為「使用強大篩選器」。

   **在「建立Workfront專案」模組之前新增篩選器，以僅允許建立紅色專案。**

   ![篩選影像2](../12-exercises/assets/filters-walkthrough-2.png)

1. 按一下連接模組的虛線或按一下扳手並選取「設定篩選器」，即可新增篩選器。
1. 使用「標籤」欄位將篩選器命名為「僅限紅色專案」。
1. 在「條件」欄位中，對應「專案顏色」欄位（CSV檔案中的欄3）。 選取「等於」（不區分大小寫）運算子，然後輸入「紅色」。
1. 按一下「確定」。

   ![濾鏡影像3](../12-exercises/assets/filters-walkthrough-3.png)

   **測試篩選器並驗證結果。**

1. 按一下「儲存」以儲存案例，然後按一下「執行一次」。
1. 按一下篩選器的執行檢查器，查看篩選器檢查每個套件組合的方式，以及傳遞或無法繼續移至建立Workfront專案模組。

   ![濾鏡影像4](../12-exercises/assets/filters-walkthrough-4.png)

1. 尋找在您的Workfront例項中建立的專案。
