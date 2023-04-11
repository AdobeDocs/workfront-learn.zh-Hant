---
title: 進階匯總逐步說明
description: 了解如何呼叫網站服務，傳回多個國家/地區的詳細資訊，並識別依子地區分組的人口，全部位於 [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9040
exl-id: c79250d0-7341-4a25-83dc-de99ce5c6dc4
doc-type: video
source-git-commit: 57b112921738c01fe4222e50403c8953c412a0f7
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# 進階匯總逐步說明

呼叫網站服務，傳回多個國家的詳細資訊，並識別依子區域分組的所有國家/地區總人口。

![融合場景的影像](assets/iteration-and-aggregation-3.png)

## 進階匯總逐步說明

Workfront建議您先觀看練習逐步影片，然後再嘗試在自己的環境中重新建立練習。

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12&learn=on)

## 練習URL

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`

>[!TIP]
>
>如需完成逐步說明，請前往 [進階匯總逐步說明](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/advanced-aggregation.html?lang=en) 練習。

## 聚集原理的強化

每當模組輸出多個套件組合時，之後的每個模組都會執行每個套件組合。

為避免此情況，請在可能產生多個套件組合的模組之後新增匯總器。

您會在藍本中的任何區段周圍看到陰影，來自 **起始迭代器** 到 **終止匯總**. 這有助於在您的Workfront Fusion案例中輕鬆找出這些區段。

## 該你了

>[!NOTE]
>
>實踐練習和挑戰是可選的，不是完成融合培訓的必要條件。

本練習以您在逐步說明中學到的內容為基礎，但並未提供解決方案。

建立新案例以加總行銷產品組合中專案中所有登入工作的小時數。 然後發送一封電子郵件，說明「您的{Project Name}項目團隊已記錄了總計{計畫時數}計畫小時數的{Summaud小時數}，使您的計畫百分比達到{%}。」

**挑戰：** 查看您是否可以執行相同操作，但僅記錄今年的小時數。

## 想要進一步了解嗎？ 我們建議下列項目：

[Workfront Fusion檔案](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
