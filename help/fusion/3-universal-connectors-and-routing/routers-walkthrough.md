---
title: 路由器逐步說明
description: 瞭解如何使用路由器將「精靈寶可夢」與「超級英雄」的套件組合傳至中的正確路徑 [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9013
exl-id: 6c111e5b-1c8f-43fd-9e2d-16599de2a337
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 0%

---

# 路由器逐步說明

使用路由器將「精靈寶可夢」與「超級英雄」組合傳至正確的路徑，然後為每個字元建立任務。

![Fusion情境的影像](assets/universal-connectors-and-routing-2.png)

## 路由器逐步說明

Workfront建議您先觀看練習逐步解說影片，然後再嘗試在您自己的環境中重新建立練習。

>[!VIDEO](https://video.tv.adobe.com/v/335272/?quality=12&learn=on)

## 練習URL

* Superhero API網站： `https://www.superheroapi.com/`
* 練習的第一個URL： `https://www.superheroapi.com/api/{access-token}/{character-id}/appearance`
* 練習的第二個URL： `https://www.superheroapi.com/api/{access-token}/{character-id}/powerstats`

如果您無法存取自己的超級英雄Token，可以使用此共用Token：10110256647253588。 請考慮您呼叫Superhero API的次數，讓此共用Token繼續對每個人都有效。

>[!TIP]
>
>如需完成逐步解說的說明，請前往 [路由器逐步說明](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/routers.html?lang=en) 練習。


## 在對映面板中搜尋專案

對應面板頂端的「搜尋專案」欄位可協助您快速找到面板中的欄位，即使這些欄位巢狀內嵌在陣列中亦然。 搜尋不區分大小寫。

![第一個搜尋面板的圖片](assets/universal-connectors-and-routing-3.png)

![第二個搜尋面板的影像](assets/universal-connectors-and-routing-4.png)

## 使用API的秘訣與技巧

到目前為止，您已經使用非常簡單的API （應用程式設計介面），不需要額外的驗證即可提取案例中所需的資訊。 以下提供一些秘訣，協助您導覽如何使用API和通用聯結器。

## 步驟1：判斷API的型別

Workfront和許多軟體系統都是使用REST （代表性狀態轉移） API建置，這是現今最簡單且最標準的API型別。 不過，也有其他幾個專案，例如：

* SOAP （簡單物件存取通訊協定） (Workfront的校訂API以SOAP為基礎)
* FTP （檔案傳輸通訊協定）
* SFTP （安全檔案傳輸通訊協定）
* 若要深入瞭解，請搜尋感興趣的API型別和關鍵字。

>[!NOTE]
>
>當連線到大型平台（例如Salesforce）時，這些平台的不同區域將提供不同的API。 請確定您找到要連線之服務的合適對象。

## 步驟2：決定API所需的驗證型別

API驗證是一種身分識別形式，用來控制對服務的存取，例如當您嘗試透過Workfront Fusion連線時。 它可協助您向其他系統證明您有權存取該系統。 OAuth 2是現今最常用的驗證型別。 透過網際網路搜尋深入瞭解API驗證。

驗證可能是使用API時最困難的方面。 Workfront Fusion通用聯結器最有價值的功能之一是，Workfront Fusion可在使用基本驗證等常見驗證方法（例如OAuth 2、API金鑰等）時為您處理驗證。 一旦您針對您的驗證方法（例如OAuth 2）使用適當的Workfront Fusion模組建立連線後，Workfront Fusion將在您每次想要執行案例時持續產生API金鑰和/或代號。

瞭解Workfront在有關Experience League的增強型驗證概觀文章中提供的各種驗證型別。

## 步驟3：閱讀API檔案並尋找所需的端點

當API與另一個系統互動時，此通訊的接觸點被視為端點。 端點是API傳送請求以及資源所在的位置。

使用通用聯結器與API互動時，您需要瞭解API支援的端點以及每個請求所需的資料。 API檔案應該說明API的端點，以及如何執行建立、讀取、更新或刪除等常見操作。 執行這些呼叫需要一些實務，尤其是當您不熟悉API呼叫或使用新API時。

進一步瞭解Workfront Fusion Universal聯結器，以及如何設定它們以與您在Experience League上所需的API連線。

## 最終備註

您可以在Experience League中檢視我們預先建立的應用程式聯結器的完整清單。 如果您想向Workfront Fusion產品團隊建議新的應用程式聯結器，請將您的想法提交至Innovation Lab。 如果您以前沒有提交過，請深入瞭解創新實驗室，以及如何投票支援想法並參與每年兩次的排行榜優先排序。 如果您已經擁有創新實驗室的存取權，請登入並提交您的想法。

## 輪到你了

>[!NOTE]
>
>練習練習和挑戰是選用的，並非完成Fusion訓練的必要條件。

此練習練習是以您在逐步解說中所學知識為基礎，但並未提供解決方案。

在「神奇寶貝字」字元的「設定多個變數」模組中，建立名為「Stat (Level)」的變數。 將「神奇寶貝統計資料」的名稱對應至此變數。 使用陣列值功能來變更陣列的顯示方式，讓每個Stat都是一行新值，如下所示。

**提示：** 只有6個不同的精靈統計有對應的層級。

![統計資料的影像](assets/universal-connectors-and-routing-5.png)

**挑戰：** 檢視您是否可以使用陣列公式讓功能以相同的方式顯示為不同的列，而不是以逗號分隔的值字串。 底下熒幕擷圖中有提示。

![陣列名稱的影像](assets/universal-connectors-and-routing-6.png)

## 想要瞭解更多？ 我們建議採取下列步驟：

[Workfront Fusion檔案](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
