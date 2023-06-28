---
title: 資料存放區
description: 瞭解如何在兩個系統之間同步公司名稱。 （應該介於60到160個字元之間，但實際為59個字元）
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11055
thumbnail: KT11055.png
exl-id: e4aa9a97-679a-4575-a2c6-b6ac304ce9c2
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---

# 資料存放區

瞭解如何在兩個系統之間同步公司名稱。

## 練習概述

這是Workfront和另一個系統中公司單向同步的第一部分。 目前，它只會在Fusion資料存放區和Workfront之間同步。 資料存放區中的表格會追蹤CSV檔案(CID)中每個公司的Workfront ID (WFID)和公司ID。 這允許在未來的某個時間點進行雙向同步。

![資料儲存區影像1](../12-exercises/assets/data-stores-walkthrough-1.png)

## 要遵循的步驟

**從Workfront下載檔案。**

1. 在Workfront「Fusion Experience Files」資料夾中，選取「_Companies.csv」並按一下「檔案詳細資訊」。
1. 從URL位址複製第一個ID號碼。
1. 在Fusion中，建立名為「使用資料存放區同步資料」的新情境。
1. 針對觸發程式模組，選取「Workfront下載檔案」模組。
1. 設定您的Workfront連線，並包含從Workfront URL複製的檔案ID。
1. 將此模組命名為「取得公司檔案」。
1. 現在新增剖析CSV模組。
1. 在「欄數」欄位中輸入2。
1. 從CSV欄位中的下載檔案模組對應資料。
1. 將此模組命名為「剖析公司檔案」。
1. 儲存您的情境並按一下「執行一次」。

   **建立資料存放區和資料結構。**

1. 新增資料存放區搜尋記錄模組。
1. 建立名為「Company sync」的新資料存放區。
1. 在資料存放區中，建立名為「Company sync (struc)」的資料結構。
1. 建立四個欄位。

   + cid - CSV檔案中的公司ID
   + 公司名稱
   + WFID - Workfront公司ID
   + 建立日期 — 確保資料型別為date

   ![資料儲存區影像2](../12-exercises/assets/data-stores-walkthrough-2.png)

1. 在資料結構上按一下「儲存」 ，然後將資料儲存大小設定為1並儲存資料儲存區。
1. 繼續在「資料存放區」模組中，設定CID等於「剖析CSV」模組（欄1）中公司ID的篩選器。
1. 按一下顯示進階設定，並選取選項以「即使此模組未傳回任何結果，仍繼續執行案例或路由」。

   ![資料儲存區影像3](../12-exercises/assets/data-stores-walkthrough-3.png)

1. 將此模組重新命名為「相符公司」。
1. 新增Workfront搜尋記錄模組。
1. 選擇「公司」作為記錄型別。
1. 搜尋條件是Workfront中的公司名稱等於CSV檔案中的公司名稱。
1. 針對輸出，選取公司名稱和ID。

   ![資料儲存區影像4](../12-exercises/assets/data-stores-walkthrough-4.png)

1. 按一下「確定」並將此模組重新命名為「相符公司」。

   **根據公司存在於Workfront中還是資料存放區而建立不同的路徑。**

   **路由路徑1 — 建立公司。**

1. 在Workfront搜尋記錄模組右側新增路由器模組。
1. 將Workfront建立記錄模組新增至頂端路徑。
1. 將記錄型別設定為公司。
1. 在欄位中選取名稱以對映。 將名稱欄位對應到剖析CSV模組的輸出（欄2）。
1. 將此模組重新命名為「建立公司」。

   ![資料儲存區影像5](../12-exercises/assets/data-stores-walkthrough-5.png)

1. 在路由器後新增篩選器，以只在Workfront中尚未建立公司時建立。 將其命名為「Not in Workfront」。
1. 將條件設定為Workfront搜尋模組中的ID，且該條件不存在。

   ![資料儲存區影像6](../12-exercises/assets/data-stores-walkthrough-6.png)

   **準備更新下一個路徑中的資料存放區。**

1. 在頂端路徑的結尾新增Set變數模組。
1. 將變數名稱設為「Workfront ID」。
1. 從建立公司模組將變數值設定為ID。
1. 將此模組重新命名為「設定Workfront ID」。

   **路由路徑2 — 更新資料存放區。**

1. 在路由路徑2上建立篩選器。 將其命名為「Not in data store」。

1. 將條件設為資料存放區模組的索引鍵，且該條件不存在。

   ![資料儲存區影像7](../12-exercises/assets/data-stores-walkthrough-7.png)

1. 此路徑中的第一個模組是Get變數模組。
1. 將變數名稱設為「Workfront ID」。
1. 將此模組重新命名為「取得Workfront ID」。
1. 從資料存放區應用程式新增另一個模組，新增/取代記錄。
1. 在「資料存放區」欄位中，選擇「公司同步」。 這是您先前建立的資料存放區。
1. 「金鑰」欄位留空。
1. 從「剖析CSV」模組的「欄1」對應CID欄位。
1. 從「剖析CSV」模組的「欄2」對應公司名稱欄位。
1. 從取得Workfront ID模組對應WFID欄位。
1. 在「已建立日期」欄位中，使用「日期」和「時間」標籤中的formatDate函式，將目前日期的格式設為MM/DD/YYYY。

   ![資料儲存區影像8](../12-exercises/assets/data-stores-walkthrough-8.png)

1. 按一下「確定」並將此模組重新命名為「建立公司專案」。

   **路由路徑3 — 在系統之間同步資料存放區。**

1. 首先，在路由路徑3上建立篩選器。 將其命名為「Company exists， not in data store」。
1. 將條件設定為資料存放區搜尋記錄模組中的索引鍵，該索引鍵不存在。
1. 按一下「新增AND規則」按鈕，並指定CSV檔案（欄2）中的公司名稱等同於Workfront搜尋模組中找到的公司名稱。

   ![資料儲存區影像9](../12-exercises/assets/data-stores-walkthrough-9.png)

1. 現在複製路由路徑2結尾的記錄模組，以新增另一個新增/取代記錄模組。
1. 將複製模組拖曳至路由路徑3結尾處。 刪除原本存在的空白模組。
1. 按一下複製的模組。 除WFID欄位外，所有欄位都應保持不變。 從「相符公司搜尋」模組對其進行對應。

   ![資料儲存區影像10](../12-exercises/assets/data-stores-walkthrough-10.png)

1. 按一下「確定」並將此模組重新命名為「建立公司專案」。
