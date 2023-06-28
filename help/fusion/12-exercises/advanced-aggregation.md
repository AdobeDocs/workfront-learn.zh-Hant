---
title: 進階彙總
description: 呼叫網路服務以傳回多個國家/地區的詳細資訊並識別按次區域分組的母體。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11048
thumbnail: KT11048.png
exl-id: 5364befa-491d-4b75-b1f0-10244f70ad7c
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# 進階彙總

瞭解彙總時如何使用群組。

## 練習概述

呼叫網路服務可傳回多個國家的詳細資訊，並識別所有國家/地區的總人口（依次區域分組）。

![進階彙總影像1](../12-exercises/assets/advanced-aggregation-walkthrough-1.png)

## 要遵循的步驟

**取得國家/地區詳細資料。**

![進階彙總影像2](../12-exercises/assets/advanced-aggregation-walkthrough-2.png)

1. 建立新情境並將其命名為「進階彙總」。
1. 將觸發程式模組設定為HTTP — 建立請求模組。
1. 使用此URL、 `https://restcountries.com/v2/lang/es`，這會提供說西班牙語的所有國家/地區清單。
1. 將方法保留為Get。
1. 按一下剖析回應核取方塊。
1. 將此模組重新命名為「取得國家」。
1. 按一下「儲存並執行一次」。

   **輸出是單一組合，但它是以24個集合的陣列提供，每個西班牙語國家各一個。**

   ![進階彙總影像3](../12-exercises/assets/advanced-aggregation-walkthrough-3.png)

   **您需要收集每個國家/地區的次區域資訊，因此您需要提出額外的HTTP請求。**

1. 新增其他要求以取得子區域資訊。 它只會傳回第一個國家/地區，但現在還可以。 新增其他HTTP提出請求模組並使用URL `https://restcountries.com/v2/name/{country name}`.
1. 若要取得第一個國家/地區的名稱，請前往對應面板，按一下資料，然後按一下陣列中的名稱。 此 [1] 在資料欄位中，表示將傳回陣列中的第一個專案。

   + 視需要按一下數字並變更索引，但在此情況下，您只需要第一個專案。

![進階彙總影像4](../12-exercises/assets/advanced-aggregation-walkthrough-4.png)

1. 檢查對應面板中的「剖析」回應，然後按一下「確定」。
1. 將此重新命名為「取得國家/地區詳細資料」。
1. 按一下「儲存」，然後按一下「執行一次」。

   + 輸出是單一國家/地區的資訊。

1. 若要取得其他國家/地區，您必須逐一檢視陣列。 新增疊代器，它會取得專案清單並輸出清單上每個專案的組合。

   **新增疊代器和彙總。**

1. 在HTTP模組之間按一下滑鼠右鍵，然後新增疊代器流量控制模組。
1. 在「陣列」欄位中，從「取得國家/地區」模組選取「資料」。

   ![進階彙總影像5](../12-exercises/assets/advanced-aggregation-walkthrough-5.png)

1. 在取得國家/地區詳細資訊模組中，更新URL欄位以從迭代器取得名稱欄位，而不是從取得國家/地區模組中取得。

   ![進階彙總影像6](../12-exercises/assets/advanced-aggregation-walkthrough-6.png)

1. 現在，在取得國家/地區詳細資訊後新增數值彙總，以分組和加總母體。
1. 來源模組是疊代器模組。
1. 彙總函式為SUM。
1. 值為 [data：population] 從「取得國家/地區詳細資訊」模組。
1. 按一下底部的「顯示進階設定」選項，並依 [data：subminor] 從「取得國家/地區詳細資訊」模組。

   ![進階彙總影像7](../12-exercises/assets/advanced-aggregation-walkthrough-7.png)

   **以文字彙總器結束，彙總您在數值彙總器中分組的內容。**

1. 在結尾處新增文字彙總。
1. 來源模組是數值彙總。
1. 在文字區域中，插入「母體總計」 [金鑰] 是 [結果].」

   ![進階彙總影像8](../12-exercises/assets/advanced-aggregation-walkthrough-8.png)

1. 儲存並執行一次。

   + 檢閱最終模組的輸出。
