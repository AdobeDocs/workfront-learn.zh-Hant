---
title: 探索執行、週期和套件
description: 使用情境的執行歷史記錄來瞭解執行、週期和套件的運作。
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
workflow-type: ht
source-wordcount: '325'
ht-degree: 100%

---

# 探索執行、週期和套件

使用情境的執行歷史記錄來瞭解執行、週期和套件的運作。

## 練習概觀

練習不同的情境設定，探索如何使用執行與週期。

![探索執行、週期和套件影像 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)

## 執行步驟

1. 原地複製名為「在路由路徑之間共用變數」的情境。把新情境命名為「在路由路徑之間共用變數 - 週期測試」。
1. 移除「傳送電子郵件」模組，因為這項測試不需要此模組。

   **設定您的情境處理每次執行 3 個週期。每個週期處理 5 個專案。**

1. 按一下觸發模組，把「最大」欄位變更為「5」，讓每個週期僅處理 5 個專案。
1. 在「搜尋」條件中，移除限制搜尋一個專案的第二個篩選器。
1. 按一下「確定」。

1. 在 Fusion 工具列中，開啟「情境」設定並將「最大週期數」欄位從「1」改為「3」。
1. 按一下「確定」。

   ![探索執行、週期和套件影像 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-1.png)


   **安排情境每分鐘執行一次。**

1. 按一下觸發模組旁邊的時鐘圖示，並變更「分鐘」欄位為「1 分鐘」。

   ![探索執行、週期和套件影像 2](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-2.png)

1. 接下來，將「執行一次」之下的「排程」按鈕切換為開啟。儲存您的情境。

   ![探索執行、週期和套件影像 3](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-3.png)

1. 前往情境的「執行歷史記錄」並看到在下一分鐘出現新的歷史記錄。您可能需要重新整理頁面。

   ![探索執行、週期和套件影像 1](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-4.png)

1. 按一下執行的「詳細資料」按鈕。點進右側面板中的「簡易記錄」，與您之前在 Workfront Fusion 培訓的執行歷史記錄部分所做的動作類似。
1. 已處理操作的記錄被分成多個週期。

   ![探索執行、週期和套件影像 5](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-5.png)

1. 您可以透過視窗右上角的下拉式選單，從您設定每次都要執行的 3 個週期中選取任何一個。

   ![探索執行、週期和套件影像 6](../12-exercises/assets/exploring-runs-cycles-and-bundles-walkthrough-6.png)
