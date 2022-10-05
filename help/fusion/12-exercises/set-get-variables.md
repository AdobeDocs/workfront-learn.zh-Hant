---
title: 設定/取得變數
description: 了解如何使用「設定」和「取得變數」模組，以使用不同路徑中一個路徑可用的欄位。
feature: Workfront Fusion
role: User
level: Beginner
kt: 11045
thumbnail: KT11045.png
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 0%

---


# 設定/取得變數

了解如何使用「設定」和「取得變數」模組，以使用不同路徑中一個路徑可用的欄位。

## 練習概觀

查詢Workfront中專案的相關資訊，並傳送包含相關資訊的電子郵件。

![設定Get變數影像1](../12-exercises/assets/set-get-variables-walkthrough-1.png)

## 遵循步驟

1. 建立新案例，並將其命名為「在路由路徑之間共用變數」。
1. 針對觸發器，選取Workfront應用程式中的搜尋模組。

   + 將記錄類型設定為「項目」。
   + 對於結果集，選擇「所有匹配記錄」。
   + 對於「搜索」條件，將其設定為「狀態等於CUR」。
   + 對於輸出，請選擇ID、名稱、說明和贊助商ID。

   ![設定Get變數影像2](../12-exercises/assets/set-get-variables-walkthrough-2.png)

   ![設定Get變數影像3](../12-exercises/assets/set-get-variables-walkthrough-3.png)

1. 按一下「確定」，然後將此模組更名為「查找當前項目」。
1. 新增其他模組並選取Workfront讀取記錄模組。

   + 對於記錄類型，請選擇用戶。
   + 對於輸出，請選擇名稱。
   + 將「贊助商ID」從「搜索」模組映射到「ID」欄位。

1. 按一下「確定」。
1. 更名模組「查找贊助商名稱」。

   ![設定Get變數影像4](../12-exercises/assets/set-get-variables-walkthrough-4.png)

1. 儲存案例，然後按一下執行一次。

   如果您在讀取記錄模組上收到錯誤，很可能是因為搜尋模組在未列出贊助商的情況下尋找專案。

   **若要避免此錯誤，請建立兩個路徑：一個用於具有贊助商ID的項目，另一個用於沒有贊助商ID的項目。**

1. 按一下路由器和讀取記錄模組之間的扳手錶徵圖，在兩個模組之間添加路由器。 設定名為「發起人存在」的篩選器，並將條件設定為「發起人ID存在」。

   ![設定Get變數影像5](../12-exercises/assets/set-get-variables-walkthrough-5.png)

1. 按一下路由器以建立其他路徑。 從電子郵件應用程式新增傳送電子郵件模組。

   + 在「收件人」欄位中放置您自己的電子郵件地址。
   + 在「主旨」欄位中，輸入「目前專案資訊」。
   + 在「內容」欄位中，放置專案名稱、說明和贊助商。
   + 您無法從讀取記錄模組提取贊助商名稱輸出。 您只能在路由器之前從搜索模組訪問發起者ID。 您需要找到從其他路由器路徑訪問贊助商名稱的方法。

   ![設定Get變數影像6](../12-exercises/assets/set-get-variables-walkthrough-6.png)

1. 按一下「確定」，然後將此模組更名為「發送項目資訊」

   **使用設定/取得變數，在不同路徑之間共用資料。**

1. 在「查找贊助商名稱」模組之後，添加「設定變數」工具模組。

   + 將「贊助商名稱」作為變數名稱。
   + 將「變數」存留期保留為一個週期。
   + 將欄位映射到「查找贊助商名稱」模組的名稱輸出。

1. 按一下「確定」，然後更名模組「設定贊助商名稱」。

   ![設定Get變數影像7](../12-exercises/assets/set-get-variables-walkthrough-7.png)

1. 接下來，在路由器和發送電子郵件模組之間按一下右鍵，以添加獲取變數工具模組。 在「變數名稱」欄位中輸入「贊助商名稱」。
1. 按一下「確定」。 更名模組「獲取贊助商名稱」。

   ![設定Get變數影像8](../12-exercises/assets/set-get-variables-walkthrough-8.png)

1. 返回「發送電子郵件」模組，並將「獲取贊助商名稱」模組的值映射到內容欄位。 按一下「確定」。

   ![設定Get變數影像8](../12-exercises/assets/set-get-variables-walkthrough-8.png)

   >[!IMPORTANT]
   >
   >在您測試案例之前，建議您限制您處理的專案數量，以避免收到大量電子郵件。

1. 前往您的Workfront試車，找到北星時裝展商展位項目。 這是一個有贊助商的項目。 從URL複製專案ID。

   ![設定Get變數影像10](../12-exercises/assets/set-get-variables-walkthrough-10.png)

1. 在您的案例中，按一下「尋找目前的專案」模組。 按一下綠色的「新增和規則」按鈕，將其他條件新增至搜尋條件。 指定ID必須與您複製的專案ID相等。 按一下「確定」。
1. 儲存您的藍本，然後按一下「執行一次」。
1. 查看執行檢查員和您收到的電子郵件。

   ![設定Get變數影像11](../12-exercises/assets/set-get-variables-walkthrough-11.png)
