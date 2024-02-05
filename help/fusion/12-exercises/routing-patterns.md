---
title: 路由模式
description: 強化路由和後援路徑的概念，但不需要實際處理任何其他 API。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11044
thumbnail: KT11044.png
exl-id: d8218115-5180-4e64-8ec1-d2d6afc88d23
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '344'
ht-degree: 100%

---

# 路由模式

強化路由和後援路徑的概念，但不需要實際處理任何其他 API。

## 練習概觀

使用「Set 變數」模組傳送一個數字通過多條路徑，瞭解路由時篩選器和後援機制的運作。

![路由模式影像 1](../12-exercises/assets/routing-patterns-walkthrough-1.png)

## 執行步驟

1. 建立一個新情境，並命名為「路由模式與後援」。
1. 對於觸發程序請新增「Set 變數」工具模組。在變數名稱中輸入「我的號碼」，「變數期限」保留「一個週期」，並把「變數」欄位設為「75」。

   ![路由模式影像 2](../12-exercises/assets/routing-patterns-walkthrough-2.png)

1. 新增另一個模組並選擇「路由器」模組。兩條路徑均選擇「遞增函數」工具，然後按一下「確定」，兩者均不進行任何變更。

   + 請為第一條路徑建立篩選器並命名為「少於 100」，並把條件設為「[我的號碼] 少於 100」。

   + 請為第二條路徑建立篩選器並命名為「少於 1000」，並把條件設為「[我的號碼] 少於 1000」。請確認兩條路徑均使用數值運算子。

   ![路由模式影像 3](../12-exercises/assets/routing-patterns-walkthrough-3.png)

   ![路由模式影像 4](../12-exercises/assets/routing-patterns-walkthrough-4.png)

1. 按一下「執行一次」並觀看套件沿著「少於 100」路徑傳遞。
1. 接著變更「Set 變數」模組欄位為「950」，並再按一下「執行一次」。觀察資料在第二條路徑的傳遞過程。
1. 按一下路由器並再新增一條路徑。新增「遞增函數」工具模組。對於篩選器，按一下「後援路徑」核取方塊。請注意指向該路徑的箭頭如何變成脫字符號，表示這是後援路徑。

   ![路由模式影像 5](../12-exercises/assets/routing-patterns-walkthrough-5.png)

1. 變更「Set 變數」的數字為「9500」並按「執行一次」。因為數字並非小於 100 或小於 1000，套件會循著後援路徑傳遞。

若您再新增一條使用「遞增函數」工具模組的路徑，但不設定篩選器，當您再次按一下「執行一次」會發生什麼事？在新增第四條路徑的情況下，套件是否仍會循著後援路徑傳遞？

+ 不會，因為並未設定任何篩選器，每個套件將永遠依循這一條路徑而非後援路徑傳遞。
