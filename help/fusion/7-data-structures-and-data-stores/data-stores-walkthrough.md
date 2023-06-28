---
title: 資料存放區逐步解說
description: 瞭解如何使用資料存放區，透過在公司清單與Workfront之間同步公司名稱 [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9055
exl-id: e96fd109-2463-4702-b1bf-b42a6dcd7fc4
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# 資料存放區逐步解說

在本練習中，我們將使用資料存放區，在公司清單與Workfront之間同步公司名稱。

這是Workfront和其他系統中公司單向同步處理的一部分。 目前，它只會在CSV檔案和Workfront之間同步。 但是它也會在資料存放區中維護一個表格，以追蹤CSV檔案中每個公司的Workfront ID (WFID)和公司ID (CID)。 這將允許我們在未來某個時間點使其成為雙向同步。

![Fusion情境的影像](assets/data-structures-and-data-stores-2.png)

## 資料存放區逐步解說

Workfront建議您先觀看練習逐步解說影片，然後再嘗試在您自己的環境中重新建立練習。

>[!VIDEO](https://video.tv.adobe.com/v/335296/?quality=12&learn=on)

>[!TIP]
>
>如需完成逐步解說的說明，請前往 [資料存放區逐步解說](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/data-stores.html?lang=en) 練習。


## 最終備註

既然您已瞭解完資料結構和資料存放區，您可能會問自己：「您何時應該使用它們？」

資料結構最常用於序列化或剖析資料格式，例如JSON、XML、CSV等。 資料結構可讓您控制資料結構，甚至驗證資料。 使用資料結構的最常見原因是建立有效的資料，以傳送至預期JSON或XML的API。 在這些情況下，您需要使用JSON或XML應用程式以及您的資料結構，以確保資料格式正確。

資料存放區應僅用於儲存需要由多個情境執行存取的永久性資料。 例如，您可以針對需要精確控制處理的進階使用案例，儲存上次處理記錄的中繼資料。

資料存放區並非設計用作資料倉儲或記錄。 無法在Workfront Fusion外部存取資料存放區，且大多數與資料存放區的互動是透過Workfront Fusion案例進行。 因此，無法將資料存放區連線到資料倉儲和記錄使用案例應有的分析或報告工具。 在像這樣的使用案例中，Workfront Fusion的角色是填入適合組織和儲存資料（例如SQL、MariaDB）的系統。

## 想要瞭解更多？ 我們建議採取下列步驟：

[Workfront Fusion檔案](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
