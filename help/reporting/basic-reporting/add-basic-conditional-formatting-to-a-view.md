---
title: 新增基本條件式格式
description: 了解如何根據您設定的條件，使用欄規則來變更報表或檢視中的文字顏色、格式和背景顏色。
activity: use
feature: Reports and Dashboards
thumbnail: 335149.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8855
exl-id: bf9a4cf4-b073-4f7e-8516-e7843f4dc20f
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# 新增基本條件式格式至檢視

條件式格式設定是透過建立欄規則來完成。 欄規則可讓您根據您設定的准則，以特定方式設定欄格式。

在此影片中，您將學習：

* 檢視中有什麼條件式格式
* 如何建立和修改條件式格式

>[!VIDEO](https://video.tv.adobe.com/v/335149/?quality=12&learn=on)

## 活動：新增條件式格式至檢視

使用現有的「標準」視圖建立名為「標準+進度」的任務視圖，並在 [!UICONTROL 名稱] 欄。

1. 新增欄規則，當任務的進度狀態為「延遲」時，欄位背景會變成紅色。
1. 新增欄規則，當進度狀態為「背後」或「處於風險」時，欄位背景會變黃色。

這將幫助您找出問題任務，而不將進度狀態欄納入您的視圖。

## 回答

![建立新列規則的螢幕影像](assets/conditional-formatting-exercise.png)

1. 在任務清單報表中，轉至 **[!UICONTROL 檢視]** 下拉式功能表，然後選取 **[!UICONTROL 新建視圖]**.
1. 將檢視命名為「標準+進度」。
1. 使用提供的預設列。
1. 選取 [!UICONTROL 任務名稱] 欄。 這是您要將條件式格式應用到的列，因此，如果任務的進度狀態不是「準時」，它將顯示為紅色或黃色。
1. 按一下 **[!UICONTROL 進階選項]** 的上角。
1. 按一下 **[!UICONTROL 為此欄新增規則]**.
1. 透過變更 [!UICONTROL 任務] > [!UICONTROL 名稱] 在視窗頂端 [!UICONTROL 任務] > [!UICONTROL 進度狀態]. 只需按一下 **[!UICONTROL X]** 表徵圖 [!UICONTROL 任務] > [!UICONTROL 名稱] 從欄位中刪除它。
1. 在欄位中輸入「progress」，然後選取 [!UICONTROL 進度狀態] 在 [!UICONTROL 任務] 欄位來源。
1. 選擇 **[!UICONTROL 延遲]** 在欄位的右側 [!UICONTROL 等於] 限定符。
1. 在 [!UICONTROL 文字顏色] 行。
1. 按一下 **[!UICONTROL 新增規則]** 以儲存欄規則。
1. 現在按一下 **[!UICONTROL 新增欄規則]** 來新增其他規則。
1. 和以前一樣，刪除 [!UICONTROL 任務] > [!UICONTROL 名稱] 從條件欄位。 替換為 [!UICONTROL 進度狀態] 在 [!UICONTROL 任務] 欄位來源。
1. 同時選擇 [!UICONTROL 風險] 和 [!UICONTROL 背後] 在等於限定符右側的欄位中。
1. 在 [!UICONTROL 文字顏色] 行。
1. 按一下 **[!UICONTROL 新增規則]** 以儲存欄規則。
1. 按一下 **[!UICONTROL 保存視圖]** 以儲存檢視。
