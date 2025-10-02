---
title: 自訂 [!UICONTROL Brand Connect] 外觀
description: 了解在 [!UICONTROL Workfront DAM] 的 [!UICONTROL Brand Connect] 中如何自訂導覽列和頁尾，以及自訂首頁和登入頁面。
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8980
exl-id: cf286347-46f0-4a7a-9f06-921975f28765
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 100%

---

# 自訂 [!UICONTROL Brand Connect] 外觀

觀看這段影片，您將了解如何：

* 自訂導覽列和頁尾
* 自訂首頁和登入頁面

>[!VIDEO](https://video.tv.adobe.com/v/335242/?quality=12&learn=on&enablevpops=1)

## 其他「[!UICONTROL 外觀]」設定

在「[!UICONTROL 外觀]」選單下的「[!UICONTROL 字體]」選項讓 [!UICONTROL Brand Portal] 中所有文字均使用所選字體的樣式。支援超過 800 種 Google 字體。

![[!UICONTROL 外觀]選單之下的[!UICONTROL 字體]選項將控制此項目的樣式：[!UICONTROL Brand Portal]](assets/02-brand-connect-appearance-font.png)

## 首頁小工具

自訂 [!UICONTROL Brand Connect] 首頁的外觀使符合組織需求。您可以使用小工具來新增例如資料夾和影像投影片一類元素。若您的組織有多個 [!UICONTROL Brand Connects]，其個別擁有自己的首頁，您可以賦予截然不同的外觀。

![螢幕擷圖顯示 [!UICONTROL Brand Connect] 首頁的可用小工具](assets/03-brand-connect-home-page-widgets.png)

可使用的小工具包括：

**A. 輪播** — 在影像投影片中顯示多個資產。每個資產皆可新增說明。按一下「新增」圖示來選取要輪播的影像。

**B. 資料夾** — 顯示包含所選資產的資料夾。按一下「新增」圖示來開啟「[!UICONTROL 資產選擇器]」，讓您可以選取一個資料夾。[!UICONTROL Brand Connect] 的使用者可以看見資料夾中的資產，但唯有擁有權限者可以下載。

**C. Lightbox** — 顯示現有的 [!UICONTROL Lightbox]。[!UICONTROL Brand Connect] 的使用者可以看見在 [!UICONTROL Lightbox] 中的資產，但是唯有擁有權限者可以下載。

**D. 品牌準則** — 在首頁上以取代或附加的方式在頂端導覽列中顯示品牌準則。

**E. 說明** — 用於顯示一小段文字。

**F. 已填寫說明** — 輸入要在灰色背景上顯示的文字複製方塊。

**G. HTML** — 使用 HTML 和 CSS 建立自訂內容。例如，您可以在影片中嵌入連結。請參考這些[應避免使用的 HTML 標籤](https://www.damsuccess.com/hc/en-us/articles/206170043-Brand-Connect-Admin-Guide#html)。

## 新增搜尋列

若您為組織的 [!UICONTROL Brand Connect] 設計一個自訂首頁，使用者必須點選進入「[!UICONTROL 資產]」區域才能進行搜尋。

但系統管理員可以使用 HTML 小工具和以下 HTML 標籤建立搜尋列：

&lt;webdambp.headersearch>&lt;/webdambp.headersearch>
