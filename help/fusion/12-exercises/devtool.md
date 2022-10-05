---
title: 開發工具
description: 使用DevTool增強案例疑難排解功能，並簡化複雜設定。
feature: Workfront Fusion
role: User
level: Beginner
kt: 11057
thumbnail: KT11057.png
source-git-commit: c348222464180e994e7b414d1b84e07f58b6b2ae
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---


# 開發工具

增強使用開發工具疑難排解案例並輕鬆進行複雜設定的能力。

## 練習概觀

安裝及使用Workfront開發工具中的不同區域，以深入探討所提出的請求/回應和進階情境設計秘訣。

>[!NOTE]
>
>Workfront Fusion Dev工具僅可在使用 [Chrome開發人員工具](https://developer.chrome.com/docs/devtools/).

![Devtool影像1](../12-exercises/assets/devtool-walkthrough-1.png)

## 遵循步驟

**安裝開發工具。**

1. 下載測試驅動器中Fusion Exerice Files資料夾中的「workfront-fusion-devtool.zip」文檔。
1. 將Zip檔案解壓縮至資料夾。
1. 在Chrome中開啟標籤，然後輸入 **chrome://extensions**.
1. 使用右上角的開關，開啟「開發人員」模式，然後按一下左上角顯示的「載入未封裝」按鈕。 選取包含開發工具的資料夾（您會在此解壓縮工具）。

   ![Devtool影像2](../12-exercises/assets/devtool-walkthrough-2.png)

1. 解壓縮後，開發工具會出現在您其他擴充功能中。

   ![Devtool影像3](../12-exercises/assets/devtool-walkthrough-3.png)

   **使用即時資料流。**

1. 首先，開啟「使用資料存放區同步資料」案例。
1. 鍵入F12或函式F12開啟開發工具。 或者，您也可以按一下Chrome位址列中的三點功能表，並導覽至開發人員工具。

   ![Devtool影像4](../12-exercises/assets/navigate-to-devtools.png)

1. 按一下「Workfront Fusion」標籤，然後從左側清單中選取「Live Stream」。
1. 按一下「執行一次」 ，即可查看事件發生時的顯示。
1. 按一下事件，即可查看請求標題、請求內文、回應標題和回應內文右側的標籤。

   ![Devtool影像4](../12-exercises/assets/devtool-walkthrough-4.png)

   **使用案例偵錯工具**

1. 選取方案偵錯器，然後按一下模組以查看該模組之操作的相關資訊。

   ![Devtool影像5](../12-exercises/assets/devtool-walkthrough-5.png)

1. 導覽至「歷史記錄」標籤。 按一下執行的詳細資訊，檢查特定執行的模組操作詳細資訊。

   ![Devtool Image 6](../12-exercises/assets/devtool-walkthrough-6.png)

   **使用工具**

1. 返回方案設計器，並在開發工具中選擇工具。 這會顯示可用的工具。

   ![Devtool Image 7](../12-exercises/assets/devtool-walkthrough-7.png)

+ 聚焦模組 — 使用模組ID快速尋找並開啟模組。
+ 依對應尋找模組 — 使用關鍵字搜尋案例，以尋找模組中的對應值和/或索引鍵。
+ 取得應用程式中繼資料 — 假設您已選取應用程式的中繼資料。
+ 複製映射 — 將映射從一個模組複製到另一個模組。 您也可以在設計工具中複製模組。
+ 複製篩選器 — 複製篩選器。 篩選器一律會指派給其正確的模組。
+ 交換連線 — 此工具會從選取的模組取用連線，並在案例中將相同的連線設定至相同應用程式的所有模組。 如果您必須在整個完成的案例中變更連線，這個功能會很好用。 使用此工具，避免丟失所有映射並節省時間。
+ 交換變數 — 在整個案例或單一模組中尋找指定變數的所有出現次數，並以新模組取代。 不支援萬用字元。 如果您不小心將值對應到整個案例，這可協助您輕鬆交換正確的值。
+ 交換應用程式 — 將指定的應用程式交換為另一個應用程式。
+ Base 64 — 將輸入的資料編碼為Base64或將Base64解碼。 當您想在編碼請求中搜尋特定資料時，這個功能會很實用。
+ 複製模組名稱 — 將所選模組名稱複製到剪貼簿。
+ 重新映射源 — 將映射源從一個模組更改為另一個模組。 首先，您需要將要用作源模組的模組添加到方案中的路由。
+ 移轉OS — 專門將Google工作表（舊版）模組升級至最新Google工作表版本。 它會在案例路由中模組的舊版本後面添加新版本的模組。
