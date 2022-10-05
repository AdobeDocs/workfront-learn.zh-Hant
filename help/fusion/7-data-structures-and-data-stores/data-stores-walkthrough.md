---
title: 資料儲存逐步說明
description: 了解如何使用資料存放區，使用將公司名稱同步至公司清單與Workfront [!DNL Adobe Workfront Fusion].
activity: use
doc-type: feature video
team: Technical Marketing
kt: Jira ticket
exl-id: e96fd109-2463-4702-b1bf-b42a6dcd7fc4
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# 資料儲存逐步說明

## 概述

在本練習中，我們使用資料存放區，將公司名稱同步至公司清單與Workfront。

這是Workfront和其他系統公司單向同步的一部分。 目前，它只會在CSV檔案與Workfront之間同步。 但它也會在資料存放區中維護一個表格，以追蹤每個公司的Workfront ID(WFID)和CSV檔案(CID)中的公司ID。 這將允許我們在未來某個時刻實現雙向同步。

![融合場景的影像](assets/data-structures-and-data-stores-2.png)

## 資料儲存逐步說明

Workfront建議您先觀看練習逐步影片，然後再嘗試在自己的環境中重新建立練習。

>[!VIDEO](https://video.tv.adobe.com/v/335296/?quality=12)

>[!TIP]
>
>如需完成逐步說明，請前往 [資料儲存逐步說明](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/data-stores.html?lang=en) 練習。


## 最後注釋

現在，您已完成了資料結構和資料儲存的學習，您可能會問自己，「您應在何時使用它們？」

資料結構最常用於序列化或剖析資料格式，例如JSON、XML、CSV等。 資料結構可讓您控制資料結構，甚至驗證資料。 使用資料結構的最常見原因是建立有效資料，以傳送至預期JSON或XML的API。 在這些情況下，您會想要使用JSON或XML應用程式以及您的資料結構，以確保資料的格式正確無誤。

資料存放區只應用於儲存需要由多個案例執行存取的永久性資料。 例如，您可以儲存上次記錄的中繼資料，這些記錄是針對需要精確控制處理的進階使用案例所處理。

資料存放區的設計不會用作資料倉庫或記錄。 在Workfront Fusion外無法存取資料存放區，且與資料存放區的互動大多是透過Workfront Fusion案例進行。 因此，無法將資料存放區連接至資料倉庫和記錄使用案例所需的分析或報告工具。 Workfront Fusion在這類使用案例中的作用是填入適當的系統，以組織和儲存資料（例如SQL、MariaDB）。

## 想要進一步了解嗎？ 我們建議下列項目：

[Workfront Fusion檔案](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
