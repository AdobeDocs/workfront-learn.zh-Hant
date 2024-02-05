---
title: 彙總
description: 瞭解如何將多個資訊套件彙總成為一個值。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11047
thumbnail: KT11047.png
exl-id: 4626b623-8b05-41be-9cfc-917e28222855
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '294'
ht-degree: 100%

---

# 彙總

瞭解如何將多個資訊套件彙總成為一個值。

## 練習概觀

使用您在上次練習時建置的「疊代簡介」情境，將專案中每個工作任務的規劃時數彙總，然後使用電子郵件把這份資訊傳送給自己。

![彙總影像 1](../12-exercises/assets/aggregation-walkthrough-1.png)

## 執行步驟

**新增篩選器並將規劃時數加總 (SUM)。**

1. 原地複製您在之前練習時建立的「疊代簡介」情境，並命名為「彙總簡介」。
1. 在「讀取專案的任務」模組和「計算任務數量」模組之間新增篩選器。將篩選器命名為「限工作任務」。
1. 設定條件為「子系數量 [數值運算子：等於] 0」。

   ![彙總影像 2](../12-exercises/assets/aggregation-walkthrough-2.png)

1. 在「隨機數學」模組之後，新增「數值彙總計算器」工具模組。
1. 設定來源模組為「讀取專案的任務」。
1. 將彙總函數設定為「SUM」。
1. 將值設為「讀取專案的任務」模組中的「工作」欄位。
1. 將這個模組重新命名為「SUM 所有任務的規劃時數」。

   ![彙總影像 3](../12-exercises/assets/aggregation-walkthrough-3.png)

   **請注意陰影顯示彙總後疊代便結束。**

   ![彙總影像 4](../12-exercises/assets/aggregation-walkthrough-4.png)

   **傳送包含彙總時數的電子郵件。**

1. 在數值彙總計算器之後，新增來自電子郵件應用程式的「傳送電子郵件」模組。
1. 傳送電子郵件給自己。
1. 主旨行是「專案詳細資料」。
1. 在「內容」欄位中，寫入「有一個專案名為 [專案名稱]，擁有總共 [結果] 個規劃時數。」「[專案名稱]」取自「讀取一筆記錄」模組，而「[結果]」取自彙總計算器模組。

   ![彙總影像 5](../12-exercises/assets/aggregation-walkthrough-5.png)

1. 按一下「儲存」，然後「執行一次」。在您的收件匣中尋找電子郵件。

在疊代內可以存取個別套件。但在疊代之外，在「傳送電子郵件」模組中，只能存取彙總的欄位。
