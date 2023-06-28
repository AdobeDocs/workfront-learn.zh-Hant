---
title: 設定/取得變數
description: 瞭解如何使用「設定」和「取得變數」模組，以使用不同路徑中一個路徑可用的欄位。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11045
thumbnail: KT11045.png
exl-id: 225f0090-0428-40e2-8a4b-9c6b18b205d2
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 0%

---

# 設定/取得變數

瞭解如何使用「設定」和「取得變數」模組，以使用不同路徑中一個路徑可用的欄位。

## 練習概述

在Workfront中查詢專案的相關資訊，並傳送包含相關資訊的電子郵件。

![設定取得變數影像1](../12-exercises/assets/set-get-variables-walkthrough-1.png)

## 要遵循的步驟

1. 建立新情境並將其命名為「在路由路徑之間共用變數」。
1. 針對觸發器，選取Workfront應用程式中的搜尋模組。

   + 將記錄型別設定為專案。
   + 針對「結果集」，選擇「所有相符記錄」。
   + 對於搜尋條件，將其設定為「狀態等於CUR」。
   + 對於輸出，請選擇ID、名稱、說明和贊助者ID。

   ![設定取得變數影像2](../12-exercises/assets/set-get-variables-walkthrough-2.png)

   ![設定取得變數影像3](../12-exercises/assets/set-get-variables-walkthrough-3.png)

1. 按一下「確定」並將此模組重新命名為「尋找目前的專案」。
1. 新增另一個模組並選取Workfront讀取記錄模組。

   + 針對「記錄型別」，選擇「使用者」。
   + 對於輸出，選擇名稱。
   + 將贊助者ID從搜尋模組對應至ID欄位。

1. 按一下「確定」。
1. 將模組重新命名為「尋找贊助者名稱」。

   ![設定取得變數影像4](../12-exercises/assets/set-get-variables-walkthrough-4.png)

1. 儲存情境並按一下「執行一次」。

   如果您在讀取記錄模組上收到錯誤，可能是因為搜尋模組找到未列出贊助者的專案。

   **若要避免此錯誤，請建立兩個路徑：一個用於擁有贊助者ID的專案，另一個用於沒有贊助者ID的專案。**

1. 按一下路由器與「讀取記錄」模組之間的扳手圖示，在兩個模組之間新增路由器。 設定名為「贊助者存在」的篩選器，並將條件設定為「贊助者ID存在」。

   ![設定取得變數影像5](../12-exercises/assets/set-get-variables-walkthrough-5.png)

1. 按一下路由器以建立其他路徑。 從電子郵件應用程式新增傳送電子郵件模組。

   + 在[收件者]欄位中放入您自己的電子郵件地址。
   + 在「主旨」欄位中，輸入「目前的專案資訊」。
   + 在「內容」欄位中，輸入專案名稱、說明和贊助者。
   + 您無法從讀取記錄模組提取贊助者名稱輸出。 您只能從路由器前面的搜尋模組存取贊助者ID。 您必須找到從其他路由器路徑存取贊助者名稱的方法。

   ![設定取得變數影像6](../12-exercises/assets/set-get-variables-walkthrough-6.png)

1. 現在按一下「確定」，然後將此模組重新命名為「傳送專案資訊」

   **使用Set/Get變數可在不同路徑之間共用資料。**

1. 在尋找贊助者名稱模組之後，新增設定變數工具模組。

   + 將「贊助者名稱」設為變數名稱。
   + 將變數存留期保留一個週期。
   + 將欄位對應到尋找贊助者名稱模組的名稱輸出。

1. 按一下「確定」，然後將模組重新命名為「設定贊助者名稱」。

   ![設定取得變數影像7](../12-exercises/assets/set-get-variables-walkthrough-7.png)

1. 接下來，在路由器和傳送電子郵件模組之間按一下滑鼠右鍵，以新增Get variable工具模組。 在「變數名稱」欄位中輸入「贊助者名稱」。
1. 按一下「確定」。 將模組重新命名為「取得贊助者名稱」。

   ![設定取得變數影像8](../12-exercises/assets/set-get-variables-walkthrough-8.png)

1. 返回「傳送電子郵件」模組，並將「取得贊助者名稱」模組的值對應至內容欄位。 按一下「確定」。

   ![設定取得變數影像8](../12-exercises/assets/set-get-variables-walkthrough-8.png)

   >[!IMPORTANT]
   >
   >在您測試情景之前，我們建議您限制您處理的專案數量，以避免收到大量電子郵件。

1. 前往Workfront試用版，找到Northstar Fashion Exhibitors Booth專案。 此為目前有贊助者的專案。 從URL複製專案ID。

   ![設定取得變數影像10](../12-exercises/assets/set-get-variables-walkthrough-10.png)

1. 在您的案例中，按一下「尋找目前的專案」模組。 按一下綠色的「新增AND規則」按鈕，將另一個條件新增至搜尋條件。 指定ID必須等於您所複製的專案ID。 按一下「確定」。
1. 儲存您的情境並按一下「執行一次」。
1. 檢閱執行檢查員以及您收到的電子郵件。

   ![設定取得變數影像11](../12-exercises/assets/set-get-variables-walkthrough-11.png)
