---
title: 開關函式
description: 了解如何使用交換機功能。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11051
thumbnail: KT1101.png
exl-id: 3142fae2-5210-4f63-9d2c-66dec58867fa
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# 開關函式

了解如何使用交換機功能。

## 練習概觀

對於簡單的資料更改，請使用Switch函式將模組欄位內的一個值轉換為另一個值。 在本練習中，將兩個字母的鍵更改為項目進度狀態的實際名稱，以發送電子郵件。

![切換函式影像1](../12-exercises/assets/switch-function-walkthrough-1.png)

## 遵循步驟

1. 原地複製名為「在路由路徑之間共用變數」的案例。
1. 將新案例命名為「在路由路徑之間共用變數 — 交換機」。
1. 按一下觸發器模組，然後將「進度狀態」新增至「輸出」區段。
1. 在「傳送電子郵件」模組中，將「進度狀態」新增至「內容」欄位。

   + 如果您只對應來自搜尋模組的值，進度狀態會有兩個字母的代碼。
   + 要「切換」代碼，以顯示每個可能進度狀態的全名，請使用「常規函式」頁簽中的「切換」函式。

1. 開關函式使用進度狀態值或表達式作為鍵，然後根據該鍵返回輸出值。

   + 在進度狀態(「LT」)之後的第一位置中定義鍵值，並在第二位置(「Late」)中定義相應的輸出。
   + 下一個鍵值被定義在第三位置，並且相應的輸出被定義在第四位置等中，以滿足所需數量的鍵。

      ![切換函式影像2](../12-exercises/assets/switch-function-walkthrough-2.png)
