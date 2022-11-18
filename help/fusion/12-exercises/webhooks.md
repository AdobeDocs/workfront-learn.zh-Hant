---
title: Webhook
description: 了解如何建立、觸發和管理Webhook啟動的案例。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11053
thumbnail: KT11053.png
exl-id: d6a62a26-a8ab-477c-a8f2-98f3b9ff5edf
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# Webhook

了解如何建立、觸發和管理Webhook啟動的案例。

## 練習概觀

此情境的目的是建立應用程式以銷售給便利店，讓他們可輕鬆判斷客戶是否年紀夠大，足以購買酒精。 收銀員只需將客戶的姓名和出生日期發佈到已提供的URL。 該貼文會觸發情境，據此計算答案並傳回給要求者。

1. 此案例包含三個Webhook。
1. 觸發程式模組是自訂網頁連結，可監聽貼文。
1. 收到貼文時，會將貼文輸出至下一個模組。
1. 下一個模組會傳回回應給要求者。

   ![Webhook映像1](../12-exercises/assets/webhooks-walkthrough-1.png)

## 遵循步驟

**設定觸發網頁鈎。**

1. 建立新案例，並將其命名為「使用WebHook」。
1. 針對觸發器，從Webhooks應用程式新增自訂Webhook模組。
1. 按一下「新增」以建立新的Webhook。
1. 輸入「飲用年齡應用程式」的Webhook名稱。
1. 將IP限制保留為空白，這表示任何人都可以將資料傳入其中。
1. 按一下儲存。


   ![Webhook映像2](../12-exercises/assets/webhooks-walkthrough-2.png)

1. 返回Webhooks映射面板後，已為此特定Webhook建立URL。 按一下「將地址複製到剪貼簿」以複製該URL。
1. 按一下「確定」。
1. 按一下「執行一次」 。
1. 使用Postman中的URL將名稱和出生日期傳送至自訂網頁連結。 如需設定Postman的指示，請參閱 [Webhook逐步說明](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/beyond-basic-modules/webhooks-walkthrough.html?lang=en) 教學課程。

   **Webhooks模組面板應如下所示：**

   ![Webhooks影像3](../12-exercises/assets/webhooks-walkthrough-3.png)

   **Webhook現在處於接聽資料以判斷資料結構的狀態。**

1. 您可以定義預期要取得之裝載的資料結構（稍後將討論資料結構）。 如果您未定義資料結構，則會在傳送貼文時自動決定資料結構。
1. 在Postman端，您要傳送至複製的URL。 貼文應包含基本表單資料。 在此範例中，您需要三個欄位：名稱、出生日期和clientToken。

   ![Webhooks影像4](../12-exercises/assets/webhooks-walkthrough-4.png)

1. 按一下「從Postman傳送」後，應會收到貼文已接受的指示。
1. 這是您的案例顯示資料結構已成功判斷的點。
1. 通過開啟執行檢查器，可以看到資料已接收。

   ![Webhooks影像5](../12-exercises/assets/webhooks-walkthrough-5.png)

   **設定客戶端令牌的路由。**

1. 將路由器添加到觸發模組。
1. 在上方路徑中，新增Webhook回應模組。 當用戶端Token不相符時，這會是我們的路徑。
1. 將狀態設為401。
1. 將內文設為{&quot;error&quot;:&quot;無法驗證請求。 請檢查您的clientToken&quot;}。

   ![Webhooks Image 6](../12-exercises/assets/webhooks-walkthrough-6.png)

1. 在路由器和Webhook響應模組之間建立篩選器。 將其命名為「用戶端代號不符合」。
1. 對於「條件」，請使用觸發模組的clientToken欄位，並與數字5121933進行數值「不等於」比較。

   ![Webhooks Image 7](../12-exercises/assets/webhooks-walkthrough-7.png)

1. 在底部路徑中，新增另一個Webhook回應模組。 當用戶端Token不符時，這會是我們的路徑。
1. 將狀態設為200。
1. 設定內文時，請使用對應面板函式來測試人員是否為21歲或以上。 如果是，則返回「你夠大喝了！」，否則返回「你不走運……」

   ![Webhooks Image 9](../12-exercises/assets/webhooks-walkthrough-9.png)

1. 在路由器和下路的Webhook響應模組之間建立篩選器。 將其命名為「用戶端代號不匹配」。
1. 對於「條件」，請使用觸發模組中的clientToken欄位，並與數字5121933進行數值「等於」比較。


   ![Webhooks Image 8](../12-exercises/assets/webhooks-walkthrough-8.png)

1. 按一下「執行一次」下的「排程」按鈕，即可啟動您的案例，如此一來，每當有新貼文將收到時，請向下任一路徑，然後產生回應。
