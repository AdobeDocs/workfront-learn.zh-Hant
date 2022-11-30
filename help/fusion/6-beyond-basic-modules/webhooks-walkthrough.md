---
title: Webhook逐步說明
description: 了解如何使用網頁連結建立應用程式，判斷客戶是否年紀夠大，足以購買酒精，全部在 [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9051
exl-id: 7870c9db-d538-440a-8972-e7bc5ac5af93
source-git-commit: 0618bf27478744e0e9976015a24c5ec8519efbb7
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Webhook逐步說明

## 總覽

此情境會建立便利店應用程式，方便客戶判斷客戶是否年齡夠大，足以購買酒精。 收銀員只需將客戶的姓名和出生日期，以及經驗證的客戶代號寄至已提供的URL。 輸入後，即會觸發我們的情境，以計算適當的回應並傳回給要求者。

![使用開關模組的影像](assets/beyond-basic-modules-5.png)

## Webhook逐步說明

Workfront建議您先觀看練習逐步影片，然後再嘗試在自己的環境中重新建立練習。

>[!VIDEO](https://video.tv.adobe.com/v/335292/?quality=12)

>[!TIP]
>
>如需完成逐步說明，請前往 [Webhook逐步說明](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/webhooks.html?lang=en) 練習。

## Postman設定

若要繼續進行逐步練習，您需要下載免費的Postman應用程式。 請依照下列步驟，導覽至Postman的正確區域以進行練習。

1. 建立工作區，然後開啟它。
1. 按一下「新增」標籤，然後建立名為「飲用年齡」的新集合。
1. 再按一下「新增」標籤，然後建立名為「GET出生日期」的新GET請求。
1. 將請求動作從GET變更為POST。
1. 前往「POSTURL」欄位下方的「內文」子標籤區域。
1. 在「授權」子標籤下選擇表單資料。
1. 為Name、Bartidate和clientToken建立三個索引鍵。

![使用開關模組的影像](assets/beyond-basic-modules-6.png)

## 該你了

>[!NOTE]
>
>實踐練習和挑戰是可選的，不是完成融合培訓的必要條件。

本練習以您在逐步說明中學到的內容為基礎，但並未提供解決方案。

建立正在等待建立新更新的Workfront Webhook，然後記錄日期、進行更新的人員姓名，以及更新的內容。 給自己發電子郵件。

**提示**:使用Workfront Watch事件觸發模組建立Webhook。 此外，在Workfront中，更新稱為附註。

**挑戰**:您能否找到並新增進行更新的URL，以方便存取？


## 想要進一步了解嗎？ 我們建議下列項目：

[Workfront Fusion檔案](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
