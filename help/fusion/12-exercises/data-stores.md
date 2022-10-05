---
title: 資料儲存
description: 了解如何在兩個系統之間同步公司名稱。 （應介於60到160個字元之間，但為59個字元）
feature: Workfront Fusion
role: User
level: Beginner
kt: 11055
thumbnail: KT11055.png
source-git-commit: c348222464180e994e7b414d1b84e07f58b6b2ae
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---


# 資料儲存

了解如何在兩個系統之間同步公司名稱。

## 練習概觀

這是Workfront和另一個系統公司單向同步的第一部分。 目前，它只會在Fusion資料存放區與Workfront之間同步。 資料存放區中的表格會追蹤每個公司的Workfront ID(WFID)和CSV檔案(CID)中的公司ID。 這允許在未來某個時間點進行雙向同步。

![資料儲存影像1](../12-exercises/assets/data-stores-walkthrough-1.png)

## 遵循步驟

**從Workfront下載檔案。**

1. 在Workfront的「Fusion Excerise Files」資料夾中，選擇「_Companies.csv」，然後按一下「Document Details」（文檔詳細資訊）。
1. 從URL位址複製第一個ID號碼。
1. 在Fusion中，建立名為「使用資料儲存來同步資料」的新案例。
1. 針對觸發程式模組，選取Workfront下載檔案模組。
1. 設定您的Workfront連線，並納入從Workfront URL複製的檔案ID。
1. 將此模組命名為「取得公司檔案」。
1. 現在新增「剖析CSV」模組。
1. 對於「列數」欄位，鍵入2。
1. 從CSV欄位中的下載檔案模組對應資料。
1. 將此模組命名為「剖析公司檔案」。
1. 儲存您的藍本，然後按一下「執行一次」。

   **建立資料儲存和資料結構。**

1. 新增資料存放區搜尋記錄模組。
1. 建立名為「公司同步」的新資料儲存。
1. 在資料存放區中，建立名為「公司同步(struc)」的資料結構。
1. 建立四個欄位。

   + CID - CSV檔案中的公司ID
   + 公司名稱
   + WFID -Workfront公司ID
   + 建立日期 — 確保資料類型為日期

   ![資料儲存影像2](../12-exercises/assets/data-stores-walkthrough-2.png)

1. 按一下資料結構上的「儲存」 ，然後將資料儲存大小設定為1並儲存資料儲存。
1. 繼續在資料存放模組中，設定一個篩選器，其中CID等於剖析CSV模組中公司的ID（欄1）。
1. 按一下「顯示高級設定」並選擇「繼續執行方案或路由，即使此模組返回時沒有結果亦然」選項。

   ![資料儲存影像3](../12-exercises/assets/data-stores-walkthrough-3.png)

1. 將此模組重新命名為「相符公司」。
1. 新增Workfront搜尋記錄模組。
1. 選擇「公司」作為記錄類型。
1. 搜尋條件是Workfront中的公司名稱等於CSV檔案中的公司名稱。
1. 對於輸出，請選取公司名稱和ID。

   ![資料儲存影像4](../12-exercises/assets/data-stores-walkthrough-4.png)

1. 按一下「確定」，將此模組重新命名為「符合公司」。

   **根據公司是否存在於Workfront或資料存放區，建立不同的路徑。**

   **路徑1 — 建立公司。**

1. 在Workfront Search記錄模組的右側新增路由器模組。
1. 將Workfront建立記錄模組新增至頂端路徑。
1. 將記錄類型設定為「公司」。
1. 從要映射的欄位中選擇名稱。 將名稱欄位對應至剖析CSV模組（欄2）的輸出。
1. 將此模組重新命名為「建立公司」。

   ![資料儲存影像5](../12-exercises/assets/data-stores-walkthrough-5.png)

1. 在路由器後面添加篩選器，以僅在未在Workfront中時建立公司。 將其命名為「不在Workfront」。
1. 從Workfront搜尋模組將條件設為ID且不存在。

   ![資料儲存影像6](../12-exercises/assets/data-stores-walkthrough-6.png)

   **準備更新下一個路徑中的資料儲存。**

1. 將設定變數模組新增至頂端路徑的結尾。
1. 將變數名稱設為「Workfront ID」。
1. 從「建立公司」模組將「變數」值設為ID。
1. 將此模組重新命名為「設定Workfront ID」。

   **路由路徑2 — 更新資料儲存。**

1. 在路由路徑2上建立篩選器。 將其命名為「不在資料存放區」。

1. 從資料儲存模組將條件設為索引鍵，且不存在。

   ![資料儲存影像7](../12-exercises/assets/data-stores-walkthrough-7.png)

1. 此路徑中的第一個模組是Get變數模組。
1. 將變數名稱設為「Workfront ID」。
1. 將此模組重新命名為「取得Workfront ID」。
1. 從資料存放區應用程式新增其他模組，新增/取代記錄。
1. 在資料儲存欄位中，選擇公司同步。 這是您先前建立的資料存放區。
1. 將「金鑰」欄位留空。
1. 從剖析CSV模組中的欄1對應CID欄位。
1. 從剖析CSV模組中的欄2對應公司名稱欄位。
1. 從Get Workfront ID模組對應WFID欄位。
1. 對於「建立日期」欄位，使用「日期和時間」頁簽中的formatDate函式，將當前日期格式為MM/DD/YYYY。

   ![資料儲存影像8](../12-exercises/assets/data-stores-walkthrough-8.png)

1. 按一下「確定」，然後將此模組重新命名為「建立公司項目」。

   **路由路徑3 — 在系統之間同步資料儲存。**

1. 首先，在路由路徑3上建立篩選器。 將其命名為「公司存在，而非在資料存放區中」。
1. 從「資料儲存搜尋記錄」模組將「條件」設為「索引鍵」，且不存在。
1. 按一下「新增和」規則按鈕，並指定CSV檔案（欄2）中的公司名稱等於在Workfront搜尋模組中找到的公司名稱。

   ![資料儲存影像9](../12-exercises/assets/data-stores-walkthrough-9.png)

1. 現在，通過克隆路由路徑2末尾的記錄模組來添加/替換另一個記錄模組。
1. 將克隆的模組拖到路由路徑3的末尾處。 刪除原來的空模組。
1. 按一下複製的模組。 除了WFID欄位外，所有欄位應保持相同。 從「相符公司搜尋」模組對應。

   ![資料儲存影像10](../12-exercises/assets/data-stores-walkthrough-10.png)

1. 按一下「確定」，然後將此模組重新命名為「建立公司項目」。
