---
title: 進階彙總操作示範
description: 瞭解在  [!DNL Adobe Workfront Fusion] 中如何呼叫網頁服務傳回有關多個國家的詳細資料，然後確認人口並依子區域分組。
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
workflow-type: ht
source-wordcount: '278'
ht-degree: 100%

---

# 進階彙總操作示範

要求網頁服務傳回關於多個國家的詳細資料，並確認所有國家的總人口，再以子區域分組。

![影像顯示 Fusion 情境](assets/iteration-and-aggregation-3.png)

## 進階彙總操作示範

Workfront 建議先觀看練習的操作示範影片，然後再嘗試在您自己的環境中重新建立練習。

>[!VIDEO](https://video.tv.adobe.com/v/335281/?quality=12&learn=on)

## 練習 URL

* `https://restcountries.com/v2/lang/es`
* `https://restcountries.com/v2/name/{country name}`

>[!TIP]
>
>有關完成操作示範的逐步說明，請前往[進階資料彙整操作示範](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/exercises/advanced-aggregation.html?lang=zh-Hant)練習。

## 強化彙總原則

一個模組在任何時候輸出多個套件，其後的每個群組將執行每一個套件。

為了防止這種情況，請在可能產生多個套件的模組之後新增一個彙總計算器。

您會看到情境中的區段均有陰影，從「**開始疊代器**」直到「**結束彙總計算器**」。有了陰影，您在 Workfront Fusion 情境中可以輕鬆發現這些區段。

## 換您來操作

>[!NOTE]
>
>您可以選擇實作練習與挑戰，但這不是完成 Fusion 培訓的必要條件。

本實作練習以您在操作示範中學到的知識為基礎，但未提供解決方案。

建立一個新情境，把行銷專案組合中各項專案的任務之所有記錄時數加總。然後傳送一封電子郵件，表示「您的 {Project Name} 專案團隊已記錄 {summed hours}，而總規劃時數為 {planned hours}，所以計劃目前進度為 {percentage}」。

**挑戰：**&#x200B;看看您是否執行相同操作，但僅限今年記錄的時數。

## 想要瞭解更多嗎？我們建議參閱以下資訊：

[Workfront Fusion 文件](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=zh-Hant)
