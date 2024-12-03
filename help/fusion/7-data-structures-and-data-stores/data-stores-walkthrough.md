---
title: 資料儲存區操作示範
description: 瞭解在使用  [!DNL Adobe Workfront Fusion] 時如何利用資料儲存區將一份公司清單上的公司名稱與 Workfront 進行同步。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9055
exl-id: e96fd109-2463-4702-b1bf-b42a6dcd7fc4
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: f033b210268e8979ee15abe812e6ad85673eeedb
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 100%

---

# 資料儲存區操作示範

在此練習中，我們使用資料儲存區將一份公司清單上公司名稱與 Workfront 同步。

這是 Workfront 和其他一些系統之間所進行的公司資料單向同步。目前只會進行 CSV 檔案與 Workfront 之間的同步。但是這項同步功能也會在資料儲存區中維護一份表格，追蹤每家公司的 Workfront ID (WFID) 與 CSV 檔案中的公司 ID (CID)。我們日後有機會可以利用這份表格進行雙向同步。

![影像顯示 Fusion 情境](assets/data-structures-and-data-stores-2.png)

## 資料儲存區操作示範

Workfront 建議先觀看練習的操作示範影片，然後再嘗試在您自己的環境中重新建立練習。

>[!VIDEO](https://video.tv.adobe.com/v/335296/?quality=12&learn=on)



## 最後提醒

現在您已經瞭解資料結構和資料儲存區，您可能會問自己：「應該在什麼時候使用？」

我們最常使用資料結構來進行資料格式序列化或剖析，例如 JSON、XML、CSV 等格式。您可以利用資料結構來控制資料的結構甚至驗證資料。使用資料結構的最常見原因是為了建立有效的資料並傳送給預期收到 JSON 或 XML 的 API。在這些情況下，您會想要把資料結構搭配 JSON 或 XML 應用程式一起使用，以確保資料格式正確。

資料儲存區僅可用於儲存超過一個情境執行需要存取的永久性資料。例如，您可以儲存關於所處理的最後一筆記錄的中繼資料，以供在處理時要求精準控制的進階使用案例使用。

資料儲存區的設計並不適用於資料倉儲或記錄。在 Workfront Fusion 以外無法存取資料儲存區，而與資料儲存區的大部 分互動均是透過 Workfront Fusion 情境進行。因此，您無法把資料儲存區連接到資料倉儲與記錄使用案例預期會使用的分析或報告工具。Workfront Fusion 在這類使用案例中的角色，是為適用於整理和儲存資料的系統 (例如 SQL、MariaDB) 填入資料。

## 想要瞭解更多嗎？我們建議參閱以下資訊：

[Workfront Fusion 文件](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=zh-Hant)
