---
title: 路由模式
description: 強化路由和備援路由的概念，而不需實際處理任何其他API。
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
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# 路由模式

強化路由和備援路由的概念，而不需實際處理任何其他API。

## 練習概述

使用「設定變數」模組透過多個路徑傳送數字，以瞭解篩選和遞補在路由時的行為。

![路由圖樣影像1](../12-exercises/assets/routing-patterns-walkthrough-1.png)

## 要遵循的步驟

1. 建立新情境並將其稱為「路由模式和遞補」。
1. 針對觸發器，新增「設定變數」工具模組。 將「My Number」設為變數名稱、將變數存留期保留為一個週期，並將「變數」欄位設為「75」。

   ![路由圖樣影像2](../12-exercises/assets/routing-patterns-walkthrough-2.png)

1. 新增另一個模組並選擇路由器模組。 針對這兩個路徑，選擇「增量函式」工具，然後按一下「確定」而不對每個路徑進行任何變更。

   + 對於第一個路徑，請建立篩選器，將其命名為「Less than 100」，並將條件設為 [我的號碼] 小於100。

   + 對於第二個路徑，請建立篩選器，將其命名為「Less than 1000」，並將條件設為 [我的號碼] 少於1000。 請務必對兩者使用數值運運算元。

   ![路由圖樣影像3](../12-exercises/assets/routing-patterns-walkthrough-3.png)

   ![路由圖樣影像4](../12-exercises/assets/routing-patterns-walkthrough-4.png)

1. 按一下「執行一次」並觀看套件組合沿著「少於100」的路徑移動。
1. 然後將「設定變數」模組欄位變更為950，並再次執行。 觀看它沿著第二個路徑執行。
1. 按一下路由器並新增一個路徑。 新增「增量」函式工具模組。 針對篩選，按一下「後援路由」核取方塊。 請注意指向該路徑的箭頭如何變成脫字元號，表示它是遞補路線。

   ![路由圖樣影像5](../12-exercises/assets/routing-patterns-walkthrough-5.png)

1. 將「設定變數」編號變更為9500，然後執行一次。 因為數字不小於100或小於1000，所以組合會沿遞補路徑向下傳送。

如果您使用「增量函式」工具模組新增一個路徑，但未設定篩選器，當您再次按一下「執行」時，會發生什麼情況？ 組合會隨著第四個路由而沿著遞補路由傳送嗎？

+ 否，因為沒有篩選器設定，每個套件組合將一律沿此路徑行進，而不是沿備援路徑行進。
