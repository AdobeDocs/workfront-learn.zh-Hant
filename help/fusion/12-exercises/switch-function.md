---
title: Switch函式
description: 瞭解如何使用Switch函式來使用交換器功能。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11051
thumbnail: KT1101.png
exl-id: 3142fae2-5210-4f63-9d2c-66dec58867fa
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Switch函式

瞭解如何使用Switch函式來使用交換器功能。

## 練習概述

若是簡單的資料變更，請使用Switch函式，在模組欄位中將一個值轉換為另一個值。 在本練習中，將兩字母金鑰變更為專案進度狀態的實際名稱，以透過電子郵件傳送。

![切換函式影像1](../12-exercises/assets/switch-function-walkthrough-1.png)

## 要遵循的步驟

1. 複製名為「在路由路徑之間共用變數」的情境。
1. 將新情況命名為「在路由路徑之間共用變數 — 切換」。
1. 按一下觸發程式模組，然後將進度狀態新增至輸出區段。
1. 在「傳送電子郵件」模組中，將「進度狀態」新增至「內容」欄位。

   + 如果您將對應到搜尋模組的值上，進度狀態會有一個兩個字母的代碼。
   + 若要「切換」每個可能進度狀態的完整名稱代碼，請使用「一般函式」標籤中的「切換」函式。

1. switch函式使用Progress Status值或運算式作為索引鍵，然後根據該索引鍵傳回輸出值。

   + 進度狀態(「LT」)之後的第一個位置會定義一個索引鍵值，而第二個位置則會定義對應的輸出（「延遲」）。
   + 下一個索引鍵值會在第三個位置定義，而對應的輸出則會定義在第四個位置等，以便視需要提供任意數目的索引鍵。

     ![切換函式影像2](../12-exercises/assets/switch-function-walkthrough-2.png)
