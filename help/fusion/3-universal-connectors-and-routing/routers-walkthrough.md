---
title: 路由器逐步
description: 了解如何使用路由器將Pokemon與超英雄捆綁在一起，沿正確的路徑傳遞 [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 9013
exl-id: 6c111e5b-1c8f-43fd-9e2d-16599de2a337
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 0%

---

# 路由器逐步

## 總覽

使用路由器將Pokemon與超級英雄捆綁在正確的路徑上，然後為每個字元建立任務。

![融合場景的影像](assets/universal-connectors-and-routing-2.png)

## 路由器逐步

Workfront建議您先觀看練習逐步影片，然後再嘗試在自己的環境中重新建立練習。

>[!VIDEO](https://video.tv.adobe.com/v/335272/?quality=12)

## 練習URL

* 超級英雄API網站： `https://www.superheroapi.com/`
* 練習的第一個URL: `https://www.superheroapi.com/api/{access-token}/{character-id}/appearance`
* 練習的第二個URL: `https://www.superheroapi.com/api/{access-token}/{character-id}/powerstats`

如果您無法存取自己的超級英雄代號，可以使用此共用代號：10110256647253588。 請考慮您呼叫超級英雄API的次數，讓此共用代號可持續適用於所有人。

>[!TIP]
>
>如需完成逐步說明，請前往 [路由器逐步](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/routers.html?lang=en) 練習。


## 在對應面板中搜尋項目

對應面板頂端的「搜尋項目」欄位可協助您快速尋找面板中的欄位，即使欄位已巢狀內嵌於陣列中亦然。 搜尋不區分大小寫。

![第一個搜索面板的影像](assets/universal-connectors-and-routing-3.png)

![第二個搜索面板的影像](assets/universal-connectors-and-routing-4.png)

## 使用API的秘訣與技巧

到目前為止，您已使用非常簡單的API（應用程式寫程式介面），它不需要額外的身份驗證即可提取方案中需要的資訊。 以下提供一些秘訣，協助您導覽使用API和通用連接器。

## 步驟1:決定API的類型

Workfront和許多軟體系統都使用REST(Representational State Transfer)API來建置，這是目前最簡單、最標準的API類型。 不過，還有其他一些項目，例如：

* SOAP（簡單物件存取通訊協定）(Workfront的校樣API是以SOAP為基礎)
* FTP（檔案傳輸通訊協定）
* SFTP（安全檔案傳輸通訊協定）
* 若要進一步了解，請對API類型和感興趣的關鍵字進行網頁搜尋。

>[!NOTE]
>
>當連線至大型平台（例如Salesforce）時，這些平台的不同區域將提供不同的API。 請確定找到適合您要連線之服務的選項。

## 步驟2:決定API所需的驗證類型

API驗證是用來控制服務存取權的身分識別形式，例如當您嘗試透過Workfront Fusion連線時。 它有助於向其他系統證明您有權訪問該系統。 OAuth 2是目前最常用的驗證類型。 透過網際網路搜尋深入了解API驗證。

使用API時，驗證可能是最困難的方面。 Workfront Fusion通用連接器最有價值的功能之一，是Workfront Fusion可在使用基本驗證等常見驗證方法（例如OAuth 2、API金鑰等）時，為您處理驗證作業。 當您使用適當的Workfront Fusion模組為驗證方法（例如OAuth 2）建立連線後，每當您想執行案例時，Workfront Fusion會持續產生API金鑰和/或權杖。

了解Workfront在Experience League的增強驗證概觀文章中提供的不同驗證類型。

## 步驟3:閱讀API檔案並尋找所需的端點

當API與其他系統互動時，此通訊的接觸點會視為端點。 端點是API傳送請求和資源所在的位置。

使用通用連接器與API互動時，您需要了解API支援的端點，以及每個請求需要哪些資料。 API檔案應說明API的端點，以及如何執行常見操作，例如建立、讀取、更新或刪除。 執行這些呼叫需要一些實務，尤其是如果您是初次進行API呼叫或使用新API時。

進一步了解Workfront Fusion Universal Connectors，以及如何設定這些連接器以連線您在Experience League時所需的API。

## 最後注釋

您可以在Experience League中查看預先建立的應用程式連接器的完整清單。 如果您想要向Workfront Fusion產品團隊建議新的應用程式連接器，請將您的想法提交至Innovation Lab。 如果您之前沒有提交過，請進一步了解創新實驗室，以及如何投票支援創意並參與每年兩次的排行榜。 如果您已擁有創新實驗室的存取權，請登入並提交您的想法。

## 該你了

>[!NOTE]
>
>練習是可選的，不必完成融合培訓。

本練習以您在逐步說明中學到的內容為基礎，但並未提供解決方案。

在為Pokemon字元設定多個變數模組中，建立名為「Stat(Level)」的變數。 將Pokemon統計資料的名稱對應至此變數。 使用陣列值功能來更改陣列的顯示方式，使每個Stat都成為新行，如下所示。

**提示：** 只有6個不同的Pokemon統計資料具有對應的層級。

![統計資料的影像](assets/universal-connectors-and-routing-5.png)

**挑戰：** 查看您是否可以使用陣列公式來獲取功能，以便以與上面相同的方式顯示不同的行，而不是以逗號分隔的值字串。 螢幕截圖中有提示。

![陣列名稱的影像](assets/universal-connectors-and-routing-6.png)

## 想要進一步了解嗎？ 我們建議下列項目：

[Workfront Fusion檔案](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
