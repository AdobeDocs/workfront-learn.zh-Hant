---
title: 篩選器練習
description: 了解如何在模組之間使用篩選器來限定特定類型的套件通過。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11040
thumbnail: KT1101.png
recommendations: noDisplay,catalog
exl-id: d2cec1ea-7ff9-48ae-8bfb-0c767d346079
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:43:22.961Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 230
ht-degree: 100%

---

# 篩選器練習

了解如何在模組之間使用篩選器來限定特定類型的套件通過。

## 練習概觀

在「超越基本對應」情境的兩個模組之間新增一個篩選器，限定只可以建立在 CSV 檔案中專案顏色為「紅色」的專案。

![篩選器影像 1](../12-exercises/assets/filters-walkthrough-1.png)

## 執行步驟

1. 原地複製「超越基本對應」情境，並將副本命名為「使用功能強大的篩選器」。

   **在「建立 Workfront 專案」模組之前新增一個篩選器，僅允許建立紅色的專案。**

   ![篩選器影像 2](../12-exercises/assets/filters-walkthrough-2.png)

1. 按一下連接模組的虛線，或是按一下扳手並選取「設定篩選器」來新增篩選器。
1. 使用「標籤」欄位來命名篩選器為「僅限紅色的專案」。
1. 在「條件」欄位中，對應「專案顏色」欄位 (CSV 檔案中第 3 欄)。 選取「等於 (不區分大小寫)」運算子，然後輸入「red」(紅色)。
1. 按一下「確定」。

   ![篩選器影像 3](../12-exercises/assets/filters-walkthrough-3.png)

   **測試篩選器並驗證結果。**

1. 按一下「儲存」來儲存情境並按一下「執行一次」。
1. 按一下篩選器的執行檢查程式，了解篩選器如何檢查每個套件，並且無論通過或不通過均要繼續執行「建立 Workfront 專案」模組。

   ![篩選器影像 4](../12-exercises/assets/filters-walkthrough-4.png)

1. 尋找在您的 Workfront 執行個體中建立的專案。
