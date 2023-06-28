---
title: 彙總
description: 瞭解如何將多個資訊套件組合彙總為單一值。
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
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# 彙總

瞭解如何將多個資訊套件組合彙總為單一值。

## 練習概述

使用您在上一個練習中建立的「反複專案簡介」情境，彙總專案中每個工作任務的計畫時數，並傳送電子郵件給您自己並提供該資訊。

![彙總影像1](../12-exercises/assets/aggregation-walkthrough-1.png)

## 要遵循的步驟

**新增篩選器並加總計畫時數。**

1. 原地複製您在上一個練習中建立的「版序簡介」案例，並將其命名為「彙總簡介」。
1. 在「讀取專案」的「任務」模組和「計算任務數量」模組之間新增篩選器。 將篩選器命名為「僅工作任務」。
1. 將條件設定為「子項數目」 [數值運運算元：等於] 0.

   ![彙總影像2](../12-exercises/assets/aggregation-walkthrough-2.png)

1. 在「隨機數學」模組之後，新增數值彙總工具模組。
1. 將來源模組設定為「讀取專案任務」。
1. 將Aggregate函式設定為SUM。
1. 從「讀取專案」的「任務」模組，將「值」設定為「工作」欄位。
1. 將此模組重新命名為「所有任務計畫時數的總和」。

   ![彙總影像3](../12-exercises/assets/aggregation-walkthrough-3.png)

   **請注意顯示聚總結束疊代的陰影。**

   ![彙總影像4](../12-exercises/assets/aggregation-walkthrough-4.png)

   **傳送包含彙總時數的電子郵件。**

1. 在數值彙總器後方新增從電子郵件應用程式傳送電子郵件模組。
1. 傳送電子郵件給您自己。
1. 主旨列為「專案詳細資料」。
1. 在「內容」欄位中，放入「有一個名為 [專案名稱] 該檔案的總數為 [結果] 計畫時數。」 「[專案名稱]「 」是從「讀取記錄」模組和「」中取得[結果]「 」取自彙總器模組。

   ![彙總影像5](../12-exercises/assets/aggregation-walkthrough-5.png)

1. 儲存並執行一次。 在收件匣中尋找電子郵件。

在反複專案內，可存取個別組合。 但在反複專案之外，在傳送電子郵件模組中，只能存取彙總欄位。
