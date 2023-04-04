---
title: 自訂外觀 [!UICONTROL Brand Connect]
description: 了解如何自訂導覽列和頁尾，以及自訂首頁和登入頁面(位於 [!UICONTROL Brand Connect] for [!UICONTROL Workfront DAM].
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8980
exl-id: cf286347-46f0-4a7a-9f06-921975f28765
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---

# 自訂 [!UICONTROL Brand Connect]

在此影片中，您將學習如何：

* 自訂導覽列和頁尾
* 自訂首頁和登入頁面

>[!VIDEO](https://video.tv.adobe.com/v/335242/?quality=12&learn=on)

## 其他 [!UICONTROL 外觀] 設定

此 [!UICONTROL 字型] 選項 [!UICONTROL 外觀] 菜單樣式整個文本 [!UICONTROL Brand Portal] 中的所有字元。 支援超過800種Google字型。

![此 [!UICONTROL 字型] 選項 [!UICONTROL 外觀] 菜單樣式 [!UICONTROL Brand Portal]](assets/02-brand-connect-appearance-font.png)

## 首頁介面工具集

自訂您 [!UICONTROL Brand Connect] 首頁以符合您的組織。 使用小工具，可以添加資料夾和影像滑塊等元素。 如果貴組織有多個 [!UICONTROL 品牌連線]，每個都有其專屬的首頁，您可以提供不同的外觀。

![可用小部件的螢幕截圖 [!UICONTROL Brand Connect] homepage](assets/03-brand-connect-home-page-widgets.png)

這些小部件可用：

**A.轉盤** — 在影像滑桿中顯示多個資產。 您可以新增說明至每個資產。 按一下「新增」圖示，選取要在輪播中顯示的影像。

**B.資料夾** — 顯示包含選定資產的資料夾。 按一下「新增」圖示以開啟 [!UICONTROL 資產選擇器] 以便選取資料夾。 資料夾中的資產對 [!UICONTROL Brand Connect] 但只能由具有權限的使用者下載。

**C.燈箱** — 顯示現有 [!UICONTROL Lightbox]. 資產 [!UICONTROL Lightbox] 將顯示為 [!UICONTROL Brand Connect] 但只能由具有權限的使用者下載。

**D.品牌准則** — 在首頁上顯示「品牌准則」，而非/不在頂端導覽列中。

**E.說明** — 用於顯示短文本。

**F.填寫的說明** — 輸入要在灰色背景中顯示的文本複製塊。

**G.HTML** — 使用HTML和CSS來建立自訂內容。 例如，您可以內嵌視訊的連結。 有些 [HTML標籤以避免](https://www.damsuccess.com/hc/en-us/articles/206170043-Brand-Connect-Admin-Guide#html).

## 新增搜尋列

如果您為組織的 [!UICONTROL Brand Connect]，使用者必須按一下 [!UICONTROL 資產] 區域來執行搜尋。

但系統管理員可以使用HTMLWidget和此HTML標籤建立搜索欄：

&lt;webdambp.headersearch>&lt;/webdambp.headersearch>
