---
title: 切換函數
description: 瞭解如何透過切換函數來使用切換功能。
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
workflow-type: ht
source-wordcount: '234'
ht-degree: 100%

---

# 切換函數

瞭解如何透過切換函數來使用切換功能。

## 練習概觀

若是簡單的資料變更，可使用切換函數在模組欄位以內將一個值轉換成另一個值。在這項練習中，為了傳送電子郵件，把專案進度狀態的兩個字母縮寫變更為實際名稱。

![切換函數影像 1](../12-exercises/assets/switch-function-walkthrough-1.png)

## 執行步驟

1. 原地複製名為「在路由路徑之間共用變數」的情境。
1. 把新情境命名為「在路由路徑之間共用變數 - 切換」。
1. 按一下觸發模組並把「進度狀態」新增到「輸出」區段。
1. 在「傳送電子郵件」的模組中，把「進度狀態」新增到「內容」欄位。

   + 若您剛剛對應取自「搜尋」模組的值，則進度狀態中顯示兩個字母的代碼。
   + 若要把每一個可能的進度狀態的代碼「切換」成完整名稱，請使用「一般函數」標籤中的「切換」函數。

1. 切換函數使用「進度狀態」值或運算式作為索引鍵，然後根據該索引鍵傳回輸出值。

   + 在「進度狀態」之後的第一個位置定義索引鍵值 (「LT」)，而在第二個位置定義對應的輸出 (「Late」)。
   + 第三個位置定義下一個索引鍵值，而在第四個位置定義其對應輸出，以此類推，而索引鍵的數量無上限。

     ![切換函數影像 2](../12-exercises/assets/switch-function-walkthrough-2.png)
