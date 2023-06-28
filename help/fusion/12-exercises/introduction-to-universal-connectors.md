---
title: 通用聯結器簡介
description: 進一步瞭解如何使用REST通用聯結器及使用傳回的資料。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11042
thumbnail: KT11042.png
exl-id: eb442c3e-26f3-44b7-9937-ed4eeba39fb1
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 0%

---

# 通用聯結器簡介

進一步瞭解如何使用REST通用聯結器及使用傳回的資料。

## 練習概述

在試算表中使用「精靈寶可夢」字元，透過HTTP聯結器呼叫Poke API，以收集和張貼有關該字元的更多資訊。

![通用聯結器簡介（圖1）](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-1.png)

## 要遵循的步驟

**從Workfront下載CSV檔案。**

1. 在Workfront「Fusion練習檔案」資料夾中，選取「_Fusion2020_Shipping Manifest.csv」，然後按一下「檔案詳細資訊」。
1. 從URL位址複製第一個ID號碼。
1. 在Workfront Fusion中建立新情境。 將其命名為「使用通用聯結器」。
1. 從Workfront應用程式的「下載檔案」模組開始。
1. 設定您的Workfront連線，並包含您從Workfront URL複製的檔案ID。
1. 將此模組重新命名為「下載出貨資訊清單」。

   ![通用聯結器簡介Image 9](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-9.png)

   **剖析出貨資訊清單資料。**

1. 新增另一個模組，選取「剖析CSV」。
1. 設定11欄的剖析CSV 。 勾選「CSV包含標題」方塊。 選擇逗號分隔符號型別，並將來自下載檔案模組的資料放入CSV欄位中。

   ![通用聯結器簡介Image 2](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-2.png)

1. 將此模組重新命名為「剖析出貨資訊清單」。
1. 儲存情境並按一下「執行一次」，以便您可以在後續步驟中檢視CSV檔案中的資料。

   **使用通用聯結器取得Pokémon資料。**

1. 新增HTTP提出要求模組。
1. 在URL欄位中使用 `https://pokeapi.co/api/v2/pokemon/[Character]`，其中 [字元] 從「剖析CSV」模組對應到「欄3」。
1. 選取剖析回應核取方塊。
1. 選取「顯示進階設定」，然後核取「將所有狀態評估為錯誤」旁的方塊。
1. 按一下「確定」並將模組重新命名為「取得Pokémon資訊」。

   **您的對應面板應如下所示：**

   ![通用聯結器簡介（圖3）](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-3.png)

   **在本練習的這一部分，您只想處理CSV檔案中的列1。**

1. 在您的「取得Pokémon」資訊模組之前新增篩選器。 將其命名為「Only row 1.」
1. 將條件設定為僅允許識別碼1通過。 ID編號1位於第1列，而ID欄位位於CSV檔案中的第1欄。

   ![通用聯結器簡介（圖4）](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-4.png)

1. 儲存情境。
1. 按一下執行一次，並觀察您在HTTP提出請求模組中所收到的錯誤訊息。

   >[!IMPORTANT]
   >
   >請注意，在輸入資料URL欄位中，字元名稱會大寫。 這無法用於進行API呼叫，因為字元名稱必須是小寫。

   ![通用聯結器簡介（圖5）](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-5.png)

1. 使用HTTP中的對應面板發出請求URL欄位，以發出 [字元] 使用「 」欄位所有小寫字母 **lower** 函式。

   ![通用聯結器簡介Image 6](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-6.png)

   **使用設定多個變數模組，從API對應資訊。**

1. 在取得Pokémon資訊後新增設定多個變數模組。 地圖名稱、高度、重量和功能。
1. 由於「功能」欄位是一個陣列，請記得使用map函式來存取陣列中每個功能的名稱。

   ![通用聯結器簡介Image 7](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-7.png)

   **在不使用篩選器的情況下執行情境以發現另一個錯誤。**

1. 若要處理CSV檔案中的所有列，請刪除名為「僅列1」的篩選器：

   + 按一下篩選圖示可加以編輯。
   + 刪除篩選標籤。
   + 刪除條件。
   + 按一下「確定」。

1. 儲存情境並按一下「執行一次」。
1. 取得Pokémon資訊模組發生錯誤。 您會看到一個超級英雄角色已傳遞到Pokémon API。

   >[!NOTE]
   >
   >在「路由器」逐步解說中，您會看到如何建立處理超級英雄的個別路徑來解決此錯誤。

   ![通用聯結器簡介（圖8）](../12-exercises/assets/introduction-to-universal-connectors-walkthrough-8.png)
