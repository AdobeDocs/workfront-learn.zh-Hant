---
title: 使用JSON
description: 了解如何在案例中建立和剖析JSON，以支援您的設計需求。
feature: Workfront Fusion
role: User
level: Beginner
kt: 11056
thumbnail: KT11056.png
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---


# 使用JSON

了解如何在案例中建立和剖析JSON，以支援您的設計需求。

## 練習概觀

本練習的目的在於從概念上說明如何運用以JSON格式傳送至案例的資訊，並將其剖析為您可在整個案例中對應的欄位和項目。 接著，您可以從這些對應陣列中擷取資訊，或將資訊匯總為JSON，然後傳送至另一個需要JSON作為接收輸入的系統。

![使用JSON影像1](../12-exercises/assets/working-with-json-walkthrough-1.png)

## 遵循步驟

**建立資料結構並剖析JSON。**

1. 建立新案例，並將其命名為「使用JSON環圈資料」。
1. 對於觸發器模組，請使用設定變數模組。
1. 對於變數名稱，輸入「環圈資料」。
1. 對於「變數」值，複製並貼上測試驅動器中Fusion Exerice Files資料夾中的「_Donut資料 — 示例JSON.rtf」文檔的內容。

   ![使用JSON影像2](../12-exercises/assets/working-with-json-walkthrough-2.png)

1. 將此模組重新命名為「來自其他連接器的JSON」。
1. 新增剖析JSON模組。
1. 按一下「資料結構」欄位的「新增」 。
1. 選取「產生器」 ，然後貼上您複製到「範例資料」欄位的「環圈資料 — 範例JSON」資料。

   ![使用JSON影像3](../12-exercises/assets/working-with-json-walkthrough-3.png)

1. 按一下「儲存」，將資料結構命名為「環圈資料」。 然後按一下「儲存」。
1. 將環圈圖資料從設定變數模組對應至JSON字串欄位。

   ![使用JSON影像4](../12-exercises/assets/working-with-json-walkthrough-4.png)

1. 儲存您的藍本，然後按一下「執行一次」以查看輸出。

   **剖析JSON模組的輸出應如下所示：**

   ![使用JSON影像5](../12-exercises/assets/working-with-json-walkthrough-5.png)

   **映射至特定陣列變數。**

1. 在分析JSON模組後添加路由器。
1. 在頂端路徑中新增設定變數模組。
1. 對於變數名稱，鍵入「按環圈鍵擊類型」。
1. 對於「變數」值，使用映射函式從批次陣列獲取批次類型。

   ![使用JSON影像6](../12-exercises/assets/working-with-json-walkthrough-6.png)

1. 按一下「確定」，然後按一下「運行」。
1. 開啟執行檢查器以查看這三個操作中每個操作的輸出包，並顯示每個操作的電池類型。

   ![使用JSON影像7](../12-exercises/assets/working-with-json-walkthrough-7.png)

   **將案例資料匯總至JSON。**

1. 在較低的路由路徑上，新增匯總至JSON模組。
1. 對於源模組，選擇迭代器 — 分析JSON模組。
1. 對於資料結構，建立或選擇任何資料結構。 在此範例中，請使用環圈資料。
1. 針對此範例，請直接將欄位對應至上，如下所示。
1. 當您遇到糊料和打頭時，請注意這些是陣列，因此您需要按一下「添加項」來映射它們。

   ![使用JSON影像8](../12-exercises/assets/working-with-json-walkthrough-8.png)

1. 儲存案例，然後按一下執行一次。

查看匯總至JSON模組的執行檢查器，並注意您如何能將三個套件組合匯總至單一JSON字串。 然後，您可以將此字串傳送至預期JSON的其他系統。

![使用JSON影像9](../12-exercises/assets/working-with-json-walkthrough-9.png)
