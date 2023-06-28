---
title: 新增基本條件式格式
description: 瞭解如何使用欄規則，根據您設定的條件，變更報表或檢視中的文字顏色、格式設定和背景顏色。
activity: use
feature: Reports and Dashboards
thumbnail: 335149.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8855
exl-id: bf9a4cf4-b073-4f7e-8516-e7843f4dc20f
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# 新增基本條件式格式至檢視

條件式格式設定是透過建立欄規則來完成。 欄規則可讓您根據您設定的條件，以特定方式格式化欄。

在本影片中，您將瞭解：

* 檢視中有哪些條件式格式
* 如何建立和修改條件式格式

>[!VIDEO](https://video.tv.adobe.com/v/335149/?quality=12&learn=on)

## 摘要

若要建立條件式格式設定：

1. 選擇要顯示格式設定的欄
1. 決定您要變更格式化的條件
1. 決定哪種格式變更效果最佳

   * 背景顏色
   * 文字色彩
   * 取代文字
   * 顯示圖示

## 活動：新增條件式格式至檢視

使用現有的標準檢視，並在上新增此條件式格式，以建立名為「標準+進度」的任務檢視。 [!UICONTROL 名稱] 欄。

1. 新增欄規則，當任務的進度狀態為「延遲」時，欄位背景會變成紅色。
1. 新增欄規則，當進度狀態為「落後」或「有風險」時，欄位背景變為黃色。

這有助於您找出有問題的任務，而不需在檢視中加入進度狀態列。

## 答案

![建立新欄規則的畫面影像](assets/conditional-formatting-exercise.png)

1. 在工作清單報告中，前往 **[!UICONTROL 檢視]** 下拉式功能表並選取 **[!UICONTROL 新增檢視]**.
1. 將檢視命名為「標準+進度」。
1. 使用提供的預設欄。
1. 選取 [!UICONTROL 任務名稱] 欄。 這是您要套用條件式格式設定的資料欄，因此如果工作的進度狀態不是「準時」，就會顯示為紅色或黃色。
1. 按一下 **[!UICONTROL 進階選項]** （位於report builder視窗的右上角）。
1. 按一下 **[!UICONTROL 為此欄新增規則]**.
1. 透過變更來啟動欄規則 [!UICONTROL 任務] > [!UICONTROL 名稱] 在視窗頂端至 [!UICONTROL 任務] > [!UICONTROL 進度狀態]. 只需按一下 **[!UICONTROL X]** 圖示旁邊 [!UICONTROL 任務] > [!UICONTROL 名稱] 以將其從欄位中刪除。
1. 在欄位中輸入「progress」，然後選取 [!UICONTROL 進度狀態] 在 [!UICONTROL 任務] 欄位來源。
1. 選取 **[!UICONTROL 延遲]** 在右側的欄位中 [!UICONTROL 等於] 限定詞。
1. 選擇紅色背景 [!UICONTROL 文字色彩] 列。
1. 按一下 **[!UICONTROL 新增規則]** 以儲存欄規則。
1. 現在按一下 **[!UICONTROL 新增欄規則]** 以新增另一個規則。
1. 就像之前一樣，刪除 [!UICONTROL 任務] > [!UICONTROL 名稱] 從「條件」欄位。 取代為 [!UICONTROL 進度狀態] 在 [!UICONTROL 任務] 欄位來源。
1. 選取兩者 [!UICONTROL 有風險] 和 [!UICONTROL 滯後] 在「相等」限定詞右側的欄位中。
1. 在「 」中選擇黃色背景 [!UICONTROL 文字色彩] 列。
1. 按一下 **[!UICONTROL 新增規則]** 以儲存欄規則。
1. 按一下 **[!UICONTROL 儲存檢視]** 以儲存檢視。
