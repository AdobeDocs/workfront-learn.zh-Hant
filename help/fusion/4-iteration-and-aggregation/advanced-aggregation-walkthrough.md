---
title: 進階彙總逐步說明
description: 瞭解如何呼叫Web服務，傳回多個國家/地區的詳細資訊並識別人口（依子區域分組），所有這些都在 [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9040
exl-id: c79250d0-7341-4a25-83dc-de99ce5c6dc4
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# 進階彙總逐步說明

呼叫網路服務可傳回多個國家/地區的詳細資訊，並識別所有國家/地區的總人口（依子區域分組）。

![Fusion情境的影像](assets/iteration-and-aggregation-3.png)

## 進階彙總逐步說明

Workfront建議您先觀看練習逐步解說影片，然後再嘗試在您自己的環境中重新建立練習。

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12&learn=on)

## 練習URL

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`

>[!TIP]
>
>如需完成逐步解說的說明，請前往 [進階彙總逐步說明](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/advanced-aggregation.html?lang=en) 練習。

## 強化彙總原則

每當模組輸出多個套件組合時，之後的每個模組都會執行每個套件組合。

若要避免此問題，請在可能產生多個套裝的模組之後新增彙總。

在情境中，您會看到任何區段周圍的陰影，從 **開頭迭代器** 至 **結束彙總**. 這有助於在Workfront Fusion情境中輕鬆發現這些區段。

## 輪到你了

>[!NOTE]
>
>練習練習和挑戰是選用的，並非完成Fusion訓練的必要條件。

此練習練習是以您在逐步解說中所學知識為基礎，但並未提供解決方案。

建立新情境，以加總行銷投資組合中專案中所有已登入任務的時數。 然後傳送一封電子郵件，說明「您的{Project Name}專案團隊已記錄總{planned hours}計畫時數中的{summed hours}，使您置於 {percentage} 計畫的一部分。」

**挑戰：** 檢視您是否可以執行相同的操作，但僅針對今年記錄的小時數。

## 想要瞭解更多？ 我們建議採取下列步驟：

[Workfront Fusion檔案](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
