---
title: 迭代程式練習簡介
description: 了解如何使用迭代類型的應用程式，並對每個資訊組合執行動作。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11046
thumbnail: KT11046.png
exl-id: 8d751885-372a-4716-9542-079cc3d36caf
source-git-commit: 1ab337568afd314d461ddea5952c9b4c900b9c26
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# 迭代程式簡介

了解如何使用迭代類型的應用程式，並對每個資訊組合執行動作。

## 練習概觀

查看Workfront中的特定專案，然後查看該專案內的所有工作。 您將使用增量工具模組來計算專案內的任務數。 最後，您將使用「設定」變數模組，從「未結問題數」中減去「子項數」，為每個任務包生成一個數值。

![迭代器簡介影像1](../12-exercises/assets/introduction-to-iterators-walkthrough-1.png)

## 遵循步驟

**閱讀專案和相關工作。**

1. 開始新情境。 將其命名為「小版本簡介」。
1. 選擇Workfront作為觸發模組，讀取記錄。
1. 對於記錄類型，選擇項目。
1. 對於輸出，選擇ID、名稱和說明。
1. 在ID欄位中，將來自您的Workfront測試驅動器實例的Northstar Fashion Invertoers Booth項目的項目ID放入。
1. 將此模組更名為「查找WF項目」。
1. 新增其他Workfront模組以讀取與此專案相關的工作。 選擇讀取相關記錄模組。
1. 對於記錄類型，選擇項目。
1. 對於父記錄ID，從讀取記錄模組中選擇ID。
1. 對於集合，選擇任務。
1. 對於輸出，請選擇ID、名稱、說明、子項數、未結問題數和工作。
1. 將此模組更名為「讀取項目的任務」。
1. 儲存情境，然後按一下「執行一次」以查看輸出。

   + 按一下執行檢查器，您將看到一個包作為輸入（項目）,28個包作為輸出（任務）。

   **計數和處理迭代捆綁。**

1. 在讀取相關記錄後新增另一個模組。 選擇增量功能工具模組。

   + 將「重置值」欄位保留為「永不」 ，然後按一下「確定」。

1. 將此模組更名為「計算任務數」。
1. 新增設定變數模組。 將變數名稱設為「隨機數學」。
1. 在「變數值」欄位中，從open opTasks數量中減去未結子項的數量。

   **應該如下所示：**

   ![迭代器簡介圖2](../12-exercises/assets/introduction-to-iterators-walkthrough-2.png)

1. 將此模組更名為「隨機數學」。
1. 儲存案例，然後按一下執行一次。

對於讀取相關記錄迭代器模組生成的每個任務，Workfront Fusion執行了28次。 除非新增匯總器以關閉回圈，否則在整個案例中會繼續處理這28個套件組合。
