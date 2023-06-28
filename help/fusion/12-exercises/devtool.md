---
title: 開發工具
description: 使用DevTool增強疑難排解情境和簡化複雜設定的能力。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11057
thumbnail: KT11057.png
exl-id: 13080212-26cf-4e5f-8f0b-fc59a6f66eb1
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# 開發工具

使用開發工具增強疑難排解情境和簡化複雜設定的能力。

## 練習概述

安裝並使用Workfront開發工具中的不同區域，以更深入地研究提出的請求/回應和進階情境設計技巧。

>[!NOTE]
>
>Workfront Fusion Dev工具只能在使用的 [Chrome開發人員工具](https://developer.chrome.com/docs/devtools/).

![Devtool影像1](../12-exercises/assets/devtool-walkthrough-1.png)

## 要遵循的步驟

**安裝開發工具。**

1. 下載在測試磁碟機的Fusion Experience Files資料夾中找到的「workfront-fusion-devtool.zip」檔案。
1. 將Zip檔案解壓縮至資料夾。
1. 在Chrome中開啟索引標籤並輸入 **chrome://extensions**.
1. 使用右上方的開關開啟開發人員模式，然後按一下左上方的「載入已解壓縮」按鈕。 選取包含開發工具的資料夾（這是您解壓縮該工具的位置）。

   ![Devtool影像2](../12-exercises/assets/devtool-walkthrough-2.png)

1. 解壓縮後，開發工具會出現在其他擴充功能中。

   ![Devtool影像3](../12-exercises/assets/devtool-walkthrough-3.png)

   **使用即時資料流。**

1. 首先，請開啟「使用資料存放區來同步資料」情境。
1. 輸入F12或函式F12以開啟「開發」工具。 或者，您可以按一下Chrome位址列中的三個點選單，並導覽至開發人員工具。

   ![Devtool影像4](../12-exercises/assets/navigate-to-devtools.png)

1. 按一下Workfront Fusion索引標籤，然後從左側的清單中選取「即時資料流」。
1. 按一下「執行一次」 ，即可在事件發生時檢視事件。
1. 按一下事件，即可在右側檢視「請求標頭」、「請求內文」、「回應標頭」和「回應內文」的標籤。

   ![Devtool影像4](../12-exercises/assets/devtool-walkthrough-4.png)

   **使用案例偵錯工具**

1. 選取「案例偵錯器」 ，然後按一下模組以檢視有關該模組操作的資訊。

   ![Devtool影像5](../12-exercises/assets/devtool-walkthrough-5.png)

1. 切換作業選項至「歷史記錄」標籤。 按一下執行上的詳細資訊，即可檢查特定執行的模組作業詳細資訊。

   ![Devtool影像6](../12-exercises/assets/devtool-walkthrough-6.png)

   **使用工具**

1. 返回情境設計工具，然後在開發工具中選取工具。 這會顯示可用的工具。

   ![Devtool影像7](../12-exercises/assets/devtool-walkthrough-7.png)

+ 焦點模組 — 使用模組ID快速找到並開啟模組。
+ 透過對應尋找模組 — 使用關鍵字搜尋案例，以尋找模組中的對應值和/或索引鍵。
+ 取得應用程式中繼資料 — 在情景中檢視所選應用程式的中繼資料。
+ Copy Mapping — 將對應從一個模組複製到另一個模組。 您也可以在設計工具中複製模組。
+ 複製篩選器 — 複製篩選器。 篩選器一律指派給右側的模組。
+ 交換連線 — 工具會從選取的模組取得連線，並在案例中設定與相同應用程式之所有模組的相同連線。 如果您必須在整個完成案例中變更連線，這會很有幫助。 使用此工具可避免遺失所有對應，並節省時間。
+ 交換變數 — 在整個情境或一個模組中尋找指定變數的所有相符專案，並將其取代為新的專案。 不支援萬用字元。 如果您不小心將值對應到整個情境中，這可協助您輕鬆交換正確的值。
+ 交換應用程式 — 將指定的應用程式交換為另一個應用程式。
+ Base 64 — 將輸入的資料編碼為Base64或解碼Base64。 當您想要搜尋已編碼請求中的特定資料時，這個用法就很實用。
+ 複製模組名稱 — 將選取的模組名稱複製到剪貼簿。
+ 重新對應來源 — 將對應來源從一個模組變更為另一個模組。 您必須先新增模組，以作為案例中路由的來源模組。
+ 移轉作業系統 — 專門將Google Sheets （舊版）模組升級至最新Google Sheets版本。 它會在案例路由中的舊版模組之後新增模組版本。
