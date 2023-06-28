---
title: Webhook逐步解說
description: 瞭解如何使用webhook建立應用程式，以判斷客戶是否達到購買酒精的年齡 [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9051
exl-id: 7870c9db-d538-440a-8972-e7bc5ac5af93
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 0%

---

# Webhook逐步解說

此情境會建立便利商店應用程式，方便他們輕鬆判斷客戶是否年事已至購買酒精。 出納只需要將客戶的名稱和出生日期，以及經過驗證的使用者端權杖，張貼至提供的URL。 輸入後，就會觸發我們的情境以計算適當的回應，並將其傳回給請求者。

![使用交換器模組的影像](assets/beyond-basic-modules-5.png)

## Webhook逐步解說

Workfront建議您先觀看練習逐步解說影片，然後再嘗試在您自己的環境中重新建立練習。

>[!VIDEO](https://video.tv.adobe.com/v/335292/?quality=12&learn=on)

>[!TIP]
>
>如需完成逐步解說的說明，請前往 [Webhook逐步解說](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/webhooks.html?lang=en) 練習。

## Postman設定

若要進行逐步解說練習，您需要下載免費的Postman應用程式。 請依照下列步驟，導覽至Postman的右側區域以進行練習。

1. 建立工作區，然後將其開啟。
1. 按一下「新增」標籤，並建立名為「飲酒年齡」的新系列。
1. 再次按一下「新增」索引標籤，然後建立名為GET生日的新增GET請求。
1. 將請求動作從「GET」變更為「POST」。
1. 前往「POSTURL」欄位下方的「內文」子標籤區域。
1. 選擇「授權」子標籤下方的表單資料。
1. 為Name、Birthdate和clientToken建立三個金鑰。

![使用交換器模組的影像](assets/beyond-basic-modules-6.png)

## 輪到你了

>[!NOTE]
>
>練習練習和挑戰是選用的，並非完成Fusion訓練的必要條件。

此練習練習是以您在逐步解說中所學知識為基礎，但並未提供解決方案。

建立正在等待建立新更新的Workfront webhook，然後記錄日期、進行更新的人員姓名以及更新的內容。 將此資訊以電子郵件寄給您自己。

**提示**：使用Workfront Watch事件觸發模組建立您的webhook。 此外，在Workfront中，更新稱為附註。

**挑戰**：您可以找到並新增進行更新的URL以方便存取嗎？


## 想要瞭解更多？ 我們建議採取下列步驟：

[Workfront Fusion檔案](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
