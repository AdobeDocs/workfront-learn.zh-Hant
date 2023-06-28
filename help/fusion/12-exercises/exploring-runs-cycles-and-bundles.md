---
title: 探索回合、循環和組合
description: 瞭解使用案例的執行歷史記錄來執行、循環和套件組合的行為。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11050
thumbnail: KT1101.png
exl-id: f04c84b1-2a3c-418b-9db3-baa74cf364f3
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# 探索回合、循環和組合

瞭解使用案例的執行歷史記錄來執行、循環和套件組合的行為。

## 練習概述

使用不同的案例設定進行練習，以探索使用回合和週期。

![探索執行循環和套件組合影像1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)

## 要遵循的步驟

1. 複製名為「在路由路徑之間共用變數」的情境。 將新案例命名為「在路由路徑之間共用變數 — 循環測試」。
1. 移除「傳送電子郵件」模組，因為此測試不需要它。

   **設定您的情境為每次執行處理3個週期。 在每個週期中處理5個專案。**

1. 按一下觸發程式模組，並將「最大值」欄位變更為5，因此每個週期僅會處理5個專案。
1. 在搜尋條件中，移除將搜尋限制在單一專案的第二個篩選器。
1. 按一下「確定」。

1. 在Fusion工具列中，開啟Scenario設定，並將Max number of cycles欄位從1變更為3。
1. 按一下「確定」。

   ![探索執行循環和套件組合影像1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)


   **將案例排程為每分鐘執行。**

1. 按一下觸發模組旁的時鐘圖示，並將「分鐘」欄位變更為1分鐘。

   ![探索執行循環和套件組合影像2](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-2.png)

1. 接下來，將「執行一次」按鈕下的「排程」切換開關切換為「開啟」。 儲存您的案例。

   ![探索執行循環和套件組合影像3](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-3.png)

1. 前往案例的「執行歷史記錄」，並觀看下一分鐘內出現的新歷史記錄。 您可能需要重新整理頁面。

   ![探索執行循環和套件組合影像1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-4.png)

1. 按一下執行的詳細資訊按鈕。 在右側面板中，點進簡單記錄，類似於您在Workfront Fusion訓練的執行歷史記錄部分中所執行的操作。
1. 已處理作業的記錄會被分割成循環。

   ![探索執行循環和套件組合影像5](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-5.png)

1. 視窗右上方的下拉式選單可讓您選取您設定為每次執行的任意3個週期。

   ![探索執行循環和套件組合影像6](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-6.png)
