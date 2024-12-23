---
title: 進階彙總練習
description: 要求網頁服務回傳有關多個國家的詳細資料，然後確認人口並依子區域分組。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11048
thumbnail: KT11048.png
recommendations: noDisplay,catalog
exl-id: 5364befa-491d-4b75-b1f0-10244f70ad7c
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: ht
source-wordcount: '493'
ht-degree: 100%

---

# 進階彙總練習

了解彙總時如何使用分組。

## 練習概觀

要求網頁服務回傳關於多個國家的詳細資料，並確認所有國家的總人口，再以子區域分組。

![進階彙總影像 1](../12-exercises/assets/advanced-aggregation-walkthrough-1.png)

## 執行步驟

**取得國家的詳細資料。**

![進階彙總影像 2](../12-exercises/assets/advanced-aggregation-walkthrough-2.png)

1. 建立一個新情境並命名為「進階彙總」。
1. 將觸發模組設定為 HTTP - 提出請求模組。
1. 使用這個 URL `https://restcountries.com/v2/lang/es`，提供使用西班牙語的所有國家清單。
1. 「方法」仍維持是「Get」。
1. 按一下「剖析回應」核取方塊。
1. 將這個模組重新命名為「擷取國家資料」。
1. 按一下「儲存」和「執行一次」。

   **輸出是單一套件，卻是含有 24 個集合的陣列，每個集合都是一個使用西班牙語的國家。**

   ![進階彙總影像 3](../12-exercises/assets/advanced-aggregation-walkthrough-3.png)

   **您需要收集每個國家/地區的子區域資訊，因此您必須提出額外的 HTTP 請求。**

1. 新增另一項請求來取得子區域資訊。此請求只會回傳第一個國家，但是目前不成問題。新增另一個 HTTP 提出請求模組並使用 URL `https://restcountries.com/v2/name/{country name}`。
1. 要取得第一個國家的名稱，請前往對應面板並按一下「資料」，然後按一下陣列中的「名稱」。資料欄位中的 [1] 表示將會傳回陣列中第一個項目。

   + 按一下數字，必要時可以變更索引，但是這個情況下您只需要第一個項目。

![進階彙總影像 4](../12-exercises/assets/advanced-aggregation-walkthrough-4.png)

1. 在對應面板中勾選「剖析回應」，然後按一下「確定」。
1. 重新命名為「擷取國家詳細資料」。
1. 按一下「儲存」，然後按一下「執行一次」。

   + 輸出是單一國家的資訊。

1. 要取得其他國家的資訊，您必須在整個陣列中進行疊代。新增一個疊代器，輸入清單上的多個物件然後在清單中輸出每個項目的套件。

   **新增疊代器和彙總計算器。**

1. 在 HTTP 模組之間按一下右鍵並新增「疊代器流程控制」模組。
1. 在「陣列」欄位中，選取來自「擷取國家資料」模組的資料。

   ![進階彙總影像 5](../12-exercises/assets/advanced-aggregation-walkthrough-5.png)

1. 在「擷取國家詳細資料」模組中，更新 URL 欄位，以便擷取疊代器的名稱欄位而不是「擷取國家資料」模組的欄位。

   ![進階彙總影像 6](../12-exercises/assets/advanced-aggregation-walkthrough-6.png)

1. 在「擷取國家詳細資料」之後新增數值彙總計算器，把人口分組並計算總和。
1. 來源模組是疊代器模組。
1. 彙總函數是 SUM。
1. 數值是來自「擷取國家詳細資料」模組的 [data:population]。
1. 按一下底部的「顯示進階設定」選項，並根據取自「擷取國家詳細資料」模組的 [data:subregion] 進行分組。

   ![進階彙總影像 7](../12-exercises/assets/advanced-aggregation-walkthrough-7.png)

   **最後使用文字彙總器來彙總您在數值彙總計算器內組合的資料。**

1. 在尾端新增文字彙總器。
1. 來源模組是數值彙總計算器。
1. 在「文字」區域，插入「[KEY] 的總人口是 [result]」。

   ![進階彙總影像 8](../12-exercises/assets/advanced-aggregation-walkthrough-8.png)

1. 按一下「儲存」，然後「執行一次」。

   + 檢閱最後模組的輸出。
