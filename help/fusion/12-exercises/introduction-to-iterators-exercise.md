---
title: 迭代器練習簡介
description: 瞭解如何使用反複專案型別的應用程式，並對每個資訊套件執行動作。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11046
thumbnail: KT11046.png
exl-id: 8d751885-372a-4716-9542-079cc3d36caf
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# 迭代器簡介

瞭解如何使用反複專案型別的應用程式，並對每個資訊套件執行動作。

## 練習概述

檢視Workfront中的特定專案，然後檢視該專案中的所有任務。 您將使用增量工具模組來計算專案中的任務數量。 最後，您將使用Set變數模組，從未完成的問題數中減去子係數目，以產生每個任務組合的數值。

![迭代器簡介Image 1](../12-exercises/assets/introduction-to-iterators-walkthrough-1.png)

## 要遵循的步驟

**閱讀專案和相關任務。**

1. 開始新情境。 將其命名為「反複專案簡介」。
1. 選擇Workfront作為觸發程式模組，讀取記錄。
1. 對於「記錄型別」，請選擇「專案」。
1. 對於輸出，請選擇ID、名稱和說明。
1. 在ID欄位中，放置您Workfront試用版執行個體中Northstar Fashion Exhibitors Booth專案的專案ID。
1. 將此模組重新命名為「尋找WF專案」。
1. 新增另一個Workfront模組以讀取與此專案相關的任務。 選擇讀取相關記錄模組。
1. 對於「記錄型別」，請選擇「專案」。
1. 對於「父記錄ID」，請從「讀取記錄」模組選擇ID。
1. 若為「集合」，請選取「任務」。
1. 對於輸出，請選取ID、名稱、說明、子係數目、未完成的問題數目和工作。
1. 將此模組重新命名為「讀取專案的任務」。
1. 儲存情境，然後按一下「執行一次」以檢視輸出。

   + 按一下執行檢測器，您會看到一個組合作為輸入（專案），28個組合作為輸出（任務）。

   **計算及處理反複專案組合。**

1. 在讀取相關記錄後新增另一個模組。 選擇「遞增」功能工具模組。

   + 將「重設值」欄位保留為「永不」，然後按一下「確定」。

1. 將此模組重新命名為「計算任務數量」。
1. 新增設定變數模組。 將變數名稱設為「隨機數學」。
1. 在「變數值」欄位中，從開啟的opTasks數目減去開啟的子係數目。

   **看起來應該像這樣：**

   ![迭代器簡介Image 2](../12-exercises/assets/introduction-to-iterators-walkthrough-2.png)

1. 將此模組重新命名為「隨機數學」。
1. 儲存情境並按一下「執行一次」。

對於讀取相關記錄迭代器模組產生的每項工作，Workfront Fusion已執行28個執行。 除非新增彙總以關閉回圈，否則這28個套件組合會在整個案例中繼續處理。
