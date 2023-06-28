---
title: Webhook
description: 瞭解如何建立、觸發及管理webhook啟動的情境。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11053
thumbnail: KT11053.png
exl-id: d6a62a26-a8ab-477c-a8f2-98f3b9ff5edf
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# Webhook

瞭解如何建立、觸發及管理webhook啟動的情境。

## 練習概述

此情境的目的是建立應用程式以銷售至便利商店，方便他們輕鬆判斷客戶是否年邁到可以購買酒精。 出納只需將客戶的姓名和出生日期張貼至他們已提供的URL。 該貼文將觸發案例，案例將計算答案並傳回給請求者。

1. 此案例包含三個Webhook。
1. 觸發模組是自訂webhook，可監聽貼文。
1. 當收到貼文時，會將其輸出到下一個模組之一。
1. 下一個模組會傳回對請求者的回應。

   ![Webhooks影像1](../12-exercises/assets/webhooks-walkthrough-1.png)

## 要遵循的步驟

**設定觸發器webhook。**

1. 建立新情境並將其命名為「使用Webhook」。
1. 對於觸發器，從Webhook應用程式新增「自訂webhook」模組。
1. 按一下新增以建立新的Webhook。
1. 輸入「飲酒年齡應用程式」的Webhook名稱。
1. 將IP限制保留空白，這表示任何人都可以將資料傳送至其中。
1. 按一下儲存。


   ![Webhook影像2](../12-exercises/assets/webhooks-walkthrough-2.png)

1. 返回Webhook對應面板，已為此特定webhook建立URL。 按一下「將地址複製到剪貼簿」以複製該URL。
1. 按一下「確定」。
1. 按一下「執行一次」。
1. 使用Postman中的URL將名稱和出生日期傳送至您的自訂webhook。 如需設定Postman的指示，請參閱 [Webhook逐步解說](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/beyond-basic-modules/webhooks-walkthrough.html?lang=en) 教學課程。

   **Webhooks模組面板應如下所示：**

   ![Webhooks影像3](../12-exercises/assets/webhooks-walkthrough-3.png)

   **webhook現在處於聆聽資料以判斷資料結構的狀態。**

1. 您可以定義預期獲得的裝載資料結構（稍後將討論資料結構）。 如果您未定義資料結構，Fusion會在傳送貼文時自動決定資料結構。
1. 在Postman端，您想要傳送至複製的URL。 貼文應包含基本表單資料。 在此範例中，您需要三個欄位：Name、Birthdate和clientToken。

   ![Webhooks影像4](../12-exercises/assets/webhooks-walkthrough-4.png)

1. 在您按一下「從Postman傳送」後，應該會看到該貼文已被接受的指示。
1. 這是您的案例顯示已成功確定資料結構的點。
1. 您可以透過開啟執行檢查器來檢視是否已收到資料。

   ![Webhooks影像5](../12-exercises/assets/webhooks-walkthrough-5.png)

   **設定使用者端Token的路由。**

1. 將路由器新增至觸發模組。
1. 在上層路徑中，新增Webhook回應模組。 當使用者端Token不符時，這將是我們的路徑。
1. 將狀態設定為401。
1. 將內文設為{&quot;error&quot;： &quot;Failed to authenticate request. 請檢查您的clientToken&quot;}。

   ![Webhooks影像6](../12-exercises/assets/webhooks-walkthrough-6.png)

1. 在路由器與Webhook回應模組之間建立篩選器。 將其命名為「使用者端權杖不符合」。
1. 對於Condition，請使用觸發程式模組的clientToken欄位，並與5121933號進行數值「不等於」比較。

   ![Webhooks影像7](../12-exercises/assets/webhooks-walkthrough-7.png)

1. 在底部路徑中，新增另一個Webhook回應模組。 當使用者端Token不符時，這將是我們的路徑。
1. 將狀態設定為200。
1. 在設定Body時，使用對應面板功能來測試以檢視人員是否為21歲或以上。 如果是，則傳回「您夠大可以喝酒了！」，否則傳回「您不走運……」

   ![Webhooks影像9](../12-exercises/assets/webhooks-walkthrough-9.png)

1. 在路由器與下方路徑的Webhook回應模組之間建立篩選器。 將其命名為「使用者端權杖不符合」。
1. 對於Condition，請使用觸發模組的clientToken欄位，並與5121933數進行數值「等於」比較。


   ![Webhooks影像8](../12-exercises/assets/webhooks-walkthrough-8.png)

1. 按一下「執行一次」下的「排程」按鈕以啟動您的情境，這樣每當有新貼文時，系統就會收到該貼文、沿著任一路徑瀏覽並產生回應。
