---
title: 高級聚合
description: 了解在匯總時如何使用分組。 （應介於60到160個字元之間，但為49個字元）
feature: Workfront Fusion
role: User
level: Beginner
kt: 11048
thumbnail: KT11048.png
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---


# 高級聚合

了解在匯總時如何使用分組。

## 練習概觀

呼叫Web服務，返回有關多個國家的詳細資訊，並確定按分區域分組的所有國家的總人口。

![高級聚合映像1](../12-exercises/assets/advanced-aggregation-walkthrough-1.png)

## 遵循步驟

**取得國家/地區詳細資訊。**

![高級聚合映像2](../12-exercises/assets/advanced-aggregation-walkthrough-2.png)

1. 建立新情境並將其命名為「進階匯總」。
1. 將觸發程式模組設為HTTP — 提出要求模組。
1. 使用此URL https://restcountries.eu/rest/v2/ lang/es，該URL為您提供了所有使用西班牙語的國家/地區的清單。
1. 將方法保留為Get。
1. 按一下「分析響應」複選框。
1. 將此模組重新命名為「取得國家/地區」。
1. 按一下「儲存並執行一次」。

   **產品只有一個組合，但它有24個系列，每個西班牙語國家/地區各一個。**

   ![高級聚合映像3](../12-exercises/assets/advanced-aggregation-walkthrough-3.png)

   **您需要收集每個國家/地區的分區域資訊，因此您需要提出額外的HTTP要求。**

1. 新增其他請求以取得分區域資訊。 它只會返回第一個國家，但暫時沒問題。 新增其他HTTP提出要求模組並使用URL https://restcountries.eu/rest/v2/name/ 。
1. 若要取得第一個國家/地區的名稱，請前往對應面板，按一下「資料」，然後按一下陣列中的「名稱」。 此 [1] 在「資料」欄位中，表示會傳回陣列中的第一個項目。

   + 視需要按一下數字並變更索引，但在此情況下，您只需要第一個項目。

   ![高級聚合映像4](../12-exercises/assets/advanced-aggregation-walkthrough-4.png)

1. 檢查映射面板中的「分析」響應，然後按一下「確定」。
1. 重新命名為「取得國家/地區詳細資料」。
1. 按一下「儲存」，然後按一下「執行一次」。

   + 產出是單一國家的資訊。

1. 若要取得其他國家/地區，您需要逐一檢查陣列。 添加迭代器，該迭代器會獲取項清單，並為清單上的每個項輸出一個包。

   **新增迭代器和匯總器。**

1. 在HTTP模組之間按一下滑鼠右鍵，然後新增迭代器流量控制模組。
1. 在「陣列」欄位中，從「獲取國家/地區」模組中選擇「資料」。

   ![高級聚合映像5](../12-exercises/assets/advanced-aggregation-walkthrough-5.png)

1. 在「取得國家/地區詳細資料」模組中，更新URL欄位，以取用迭代器中的名稱欄位，而非取用「取得國家/地區」模組中的名稱欄位。

   ![高級聚合映像6](../12-exercises/assets/advanced-aggregation-walkthrough-6.png)

1. 現在，在「取得國家/地區詳細資料」後新增數值匯總器，以分組並加總母體。
1. 源模組是迭代器模組。
1. 匯總函式為SUM。
1. 值為 [資料：人口] 從「取得國家/地區詳細資料」模組取得。
1. 按一下底部的「顯示進階設定」選項，然後依群組分組 [資料：子區域] 從「取得國家/地區詳細資料」模組取得。

   ![高級聚合映像7](../12-exercises/assets/advanced-aggregation-walkthrough-7.png)

   **使用文本聚合器完成，以聚合您在數字聚合器中分組的內容。**

1. 將文本聚合器添加到結尾。
1. 源模組是數值聚合器。
1. 在「文字」區域中，插入「 [代碼] is [結果].&quot;

   ![高級聚合映像8](../12-exercises/assets/advanced-aggregation-walkthrough-8.png)

1. 儲存並執行一次。

   + 檢閱最終模組的輸出。
