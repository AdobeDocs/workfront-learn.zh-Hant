---
title: 自訂外觀 [!UICONTROL Brand Connect]
description: 瞭解如何自訂導覽列和頁尾，以及自訂中的首頁和登入頁面 [!UICONTROL Brand Connect] 的 [!UICONTROL WORKFRONT DAM].
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8980
exl-id: cf286347-46f0-4a7a-9f06-921975f28765
doc-type: video
source-git-commit: 6c31f8d2e98ad8cd1880cd03ec0b0e6c0fd9ec09
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---

# 自訂外觀 [!UICONTROL Brand Connect]

在本影片中，您將瞭解如何：

* 自訂導覽列和頁尾
* 自訂首頁和登入頁面

>[!VIDEO](https://video.tv.adobe.com/v/335242/?quality=12&learn=on)

## 其他 [!UICONTROL 外觀] 設定

此 [!UICONTROL 字型] 下的選項 [!UICONTROL 外觀] 功能表會設定整個文字的樣式 [!UICONTROL Brand Portal] 以選取的字型顯示。 支援800多種Google字型。

![此 [!UICONTROL 字型] 下的選項 [!UICONTROL 外觀] 功能表樣式 [!UICONTROL Brand Portal]](assets/02-brand-connect-appearance-font.png)

## 首頁Widget

客製化您的外觀 [!UICONTROL Brand Connect] 首頁以符合您的組織。 使用Widget，您可以新增資料夾和影像滑桿等元素。 如果您的組織有多個 [!UICONTROL Brand Connected]，每個都有自己的首頁，您可以提供不同的外觀。

![您可用的介面工具集熒幕擷圖 [!UICONTROL Brand Connect] homepage](assets/03-brand-connect-home-page-widgets.png)

這些Widget可供使用：

**A.輪播** — 在影像滑桿中顯示多個資產。 您可以為每個資產新增說明。 按一下「新增」圖示，選取要顯示在轉盤中的影像。

**B.資料夾** — 顯示包含所選資產的資料夾。 按一下「新增」圖示以開啟 [!UICONTROL 資產選擇器] 以便您選取資料夾。 您可以看到資料夾中的資產 [!UICONTROL Brand Connect] 使用者，但只能由具有許可權的使用者下載。

**C.燈箱** — 顯示現有 [!UICONTROL Lightbox]. 中的資產 [!UICONTROL Lightbox] 將會顯示給 [!UICONTROL Brand Connect] 使用者，但只能由具有許可權的使用者下載。

**D.品牌指引** — 在首頁上顯示品牌指引，而非/另外在頂端導覽列中顯示。

**E.說明** — 用於顯示短文字。

**F.已填說明** — 輸入要顯示在灰色背景上的文字複製區塊。

**G.HTML** — 使用HTML和CSS建立自訂內容。 例如，您可以將連結內嵌至視訊。 有一些是 [HTML標籤以避免](https://www.damsuccess.com/hc/en-us/articles/206170043-Brand-Connect-Admin-Guide#html).

## 新增搜尋列

如果您為貴組織的網站設計自訂首頁 [!UICONTROL Brand Connect]，使用者必須按一下 [!UICONTROL 資產] 執行搜尋的區域。

但系統管理員可以使用HTMLWidget和此HTML標籤建立搜尋列：

&lt;webdambp.headersearch>&lt;/webdambp.headersearch>
