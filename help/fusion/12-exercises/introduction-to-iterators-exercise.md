---
title: 疊代器練習簡介
description: 瞭解如何使用疊代類型應用程式和針對每個資訊套件執行動作。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11046
thumbnail: KT11046.png
recommendations: noDisplay,catalog
exl-id: 8d751885-372a-4716-9542-079cc3d36caf
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:42:51.955Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 390
ht-degree: 100%

---

# 疊代器練習簡介

瞭解如何使用疊代類型應用程式和針對每個資訊套件執行動作。

## 練習概觀

查看 Workfront 中的特定專案，然後查看該專案中所有任務。 您將會使用遞增工具模組來計算專案中的任務數量。 最後，您會使用「Set 變數模組」，從「未決問題數量」減去「子系數量」，為每個任務套件產生一個數值。

![疊代器簡介影像 1](../12-exercises/assets/introduction-to-iterators-walkthrough-1.png)

## 執行步驟

**讀取專案和相關任務。**

1. 開始新的情境。 將其命名為「疊代簡介」。
1. 選取 Workfront 作為觸發模組「讀取一筆記錄」。
1. 對於「記錄類型」，請選擇「專案」。
1. 對於「輸出」，請選擇「ID」、「名稱」和「說明」。
1. 在「ID」欄位中，填入您的 Workfront 產品試用執行個體中「Northstar Fashion Exhibitors Booth」專案的專案 ID。
1. 把這個模組重新命名為「尋找 WF 專案」。
1. 新增另一個 Workfront 模組來讀取與這個專案相關的任務。 選擇「讀取相關記錄」模組。
1. 對於「記錄類型」，請選擇「專案」。
1. 對於父系記錄 ID，請從「讀取一筆記錄」模組選擇 ID。
1. 對於「集合」，選取「任務」。
1. 對於「輸出」，選取「ID」、「名稱」、「說明」、「子系數量」、「未決問題數量」和「工作」。
1. 把這個模組重新命名為「讀取專案的任務」。
1. 儲存情境，然後按一下「執行一次」來查看輸出。

   + 按一下執行檢查程式，您便會看到一個套件作為輸入 (專案) 以及 28 個套件作為輸出 (任務)。

   **計算並處理疊代產生的套件。**

1. 在「讀取相關記錄」之後新增另一個模組。 選擇「遞增函數工具」模組。

   + 保留「重設值欄位」的設定為「從不」再按一下「確定」。

1. 將這個模組重新命名為「計算任務的數量」。
1. 新增「Set 變數」模組。 設定變數名稱為「隨機數學」。
1. 在「變數值」欄位中，從未完成的 opTask 數量中減去未完成子系的數量。

   **應是如下所示：**

   ![疊代器簡介影像 2](../12-exercises/assets/introduction-to-iterators-walkthrough-2.png)

1. 將這個模組重新命名為「隨機數學」。
1. 請儲存情境並按一下「執行一次」。

針對「讀取相關記錄」疊代器模組所產生的每個任務，Workfront Fusion 已執行 28 次。 這 28 個套件在整個情境中將持續進行處理，除非新增一個彙總計算器來結束迴圈。
