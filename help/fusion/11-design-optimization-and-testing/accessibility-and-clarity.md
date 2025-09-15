---
title: 容易取得而且資訊明確
description: 了解一些基本的最佳實務，讓情境資訊變得容易閱讀、共用和理解。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11037
recommendations: noDisplay,catalog
exl-id: ba2c5c64-ab4d-42d3-8a69-6b9df1373b29
source-git-commit: dfcca5f02a6d9f7ee44a1e894106ae48259eea91
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 99%

---

# 容易取得而且資訊明確

在 Workfront Fusion 培訓初期，您已學習一些讓情境變得容易閱讀、共用和理解的基本最佳實務。這些做法能夠讓工作變得更輕鬆，未來的 Workfront Fusion 使用者或是針對 Workfront Fusion 執行個體進行疑難排解或提供支援的任何人均會受益。在設計情境時遵守以下準則，讓其他人也能繼續享受這個好處。

## 標籤和備註

一般來說，Workfront Fusion 的主要目標是實現簡單的情境設計。以下方法可以協助您實現容易理解的設計。

* 所有模組都必須命名。在模組上按一下右鍵並選取「重新命名」。模組標籤應使用簡短而且容易理解的字句說明模組所執行的工作。例如「Create Mktg Proj w/ Ch Template」。
  ![影像顯示具有錯誤處理功能之情境](assets/design-optimization-and-testing-1.png)
* 路由路徑也要加上標籤。即使某個路徑並未在路由器之後直接使用篩選器，您也可以在不填寫篩選邏輯的情況下套用標籤。這樣做能讓其他人了解哪個套件經由哪一條路徑傳遞及其原因。要為沒有篩選器的路由路徑建立標籤，請在路徑上按一下右鍵，新增標籤並按一下「儲存」。
  ![影像顯示具有錯誤處理功能之情境](assets/design-optimization-and-testing-2.png)
* 如果模組標籤或路由路徑標籤敘述太短，無法說清楚實際的工作內容，則可以在情境中適合的地方新增備註。在整個設計和疊代過程中，您可以在隨時新增備註。

不過，如果在做好發行準備時在情境設計的末端新增備註，可能最容易閱讀和理解。從情境設計的末端 (最遠的右下角) 反向新增備註。這樣一來，開啟備註面板時，情境開始時適用的備註將會位在清單的頂端。

儲存或關閉備註面板之後，備註會進行排序，將最近建立的排在頂端。在下圖中，第一個建立的備註出現在清單的底端。我們刻意從上面路徑的右下角開始建立備註，最後到達觸發程序；本質上就是一組資料通過情境時的相反方向。這樣一來，備註出現的順序，便是情境針對那一組資料執行作業的順序。

![影像顯示具有錯誤處理功能之情境](assets/design-optimization-and-testing-3.png)

## Workfront Fusion 範本

將模組和路由路徑標籤作業簡化的好方法就是使用範本。最佳實務範本可以加快建立常見使用案例情境的速度。

### 範本範例

在開始執行情境時，先檢查是否有可以協助作業的可用範本。例如，您要建立一個從 Workfront 下載 CSV 文件便會啟動的情境，然後進行解析。

按一下「範本」區域，看看是否有任何公開的範本符合需求。

![影像顯示具有錯誤處理功能之情境](assets/design-optimization-and-testing-4.png)

按一下「團隊範本」標籤，看看團隊成員所建立的範本是否可以派上用場。

如果您找到想要使用的範本，按一下其名稱來開啟範本。

![影像顯示具有錯誤處理功能之情境](assets/design-optimization-and-testing-5.png)

接著到右上角按一下「選項」，並選取「建立情境」。

![影像顯示具有錯誤處理功能之情境](assets/design-optimization-and-testing-6.png)

### 建立範本

您可以在「團隊範本」區域建立範本。您和您的團隊均可使用您建立的範本，但是若您按一下「發佈」按鈕，則可以與團隊以外的人員共用範本。

![影像顯示具有錯誤處理功能之情境](assets/design-optimization-and-testing-7.png)

建置範本時，您可以加入一個精靈，引導使用範本的人員建置自己的情境以及在適當時候變更連線、對應資料和其他面板欄位。

勾選「在精靈中使用」核取方塊新增相關指示，讓使用您的範本建置情境的人可以使用。這些資訊將出現的「說明」欄位。若要允許使用者在使用範本時看到這段文字，請啟用「使用為預設值」。

![影像顯示具有錯誤處理功能之情境](assets/design-optimization-and-testing-8.png)

## 想要了解更多嗎？我們建議參閱以下資訊：

[Workfront Fusion 文件](https://experienceleague.adobe.com/zh-hant/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
