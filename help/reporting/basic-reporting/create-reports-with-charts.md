---
title: 使用圖表建立報告
description: 瞭解圖表如何改善資料的視覺效果，以及如何在Workfront中使用圖表工具。
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335153.png
jira: KT-8860
exl-id: ea3b360b-1fbd-4d1a-b505-b75759d24e41
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# 使用圖表建立報告

在本影片中，您將瞭解：

* 圖表如何改善資料的視覺效果
* 如何使用Workfront的圖表工具

>[!VIDEO](https://video.tv.adobe.com/v/335155/?quality=12&learn=on)

## 活動：新增圖表至報表

本季末即將結束，您想要瞭解最近完成的專案是如何受限於其預算的。 建立顯示專案計畫成本與實際成本的報告。 您只想檢視在上一個季度完成的專案。 使用自訂顏色新增組合直條圖。

## 答案

1. 選取 **[!UICONTROL 報表]** 從 **[!UICONTROL 主要功能表]**.
1. 按一下 **[!UICONTROL 新報告]** 功能表並選取 **[!UICONTROL 專案]**.
1. 在 **[!UICONTROL 欄（檢視）]** 標籤，按一下 **[!UICONTROL 新增欄]**.
1. 選取 [!UICONTROL 專案] > [!UICONTROL 計畫成本] 並依照以下說明摘要此欄： **[!UICONTROL 總和]**.
1. 按一下 **[!UICONTROL 新增欄]** 再來一次。
1. 選取 [!UICONTROL 專案] > [!UICONTROL 實際成本] 並依照以下說明摘要此欄： **[!UICONTROL 總和]**.

   ![新增欄至報表的畫面影像](assets/chart-report-columns.png)

1. 在 **[!UICONTROL 群組]** 索引標籤中，將報表設定為分組依據 [!UICONTROL 專案] > [!UICONTROL 名稱].

   ![新增分組至報表的畫面影像](assets/chart-report-groupings.png)

1. 在 **[!UICONTROL 篩選器]** 索引標籤中，新增兩個篩選規則：

   * [!UICONTROL 專案] > [!UICONTROL 狀態等同於] > [!UICONTROL 完成]
   * [!UICONTROL 專案] >[!UICONTROL  實際完成日期] > [!UICONTROL 上個季度]

   ![新增濾鏡至報表的畫面影像](assets/chart-report-filters.png)

1. 在 **[!UICONTROL 圖表]** 索引標籤，選擇 **[!UICONTROL 欄]** 圖表型別。
1. 對於 [!UICONTROL 左(Y)軸]，選擇 [!UICONTROL 專案] > [!UICONTROL 計畫成本].
1. 對於 [!UICONTROL 底部(X)軸]，選擇 [!UICONTROL 專案] > [!UICONTROL 名稱].
1. 按一下 **[!UICONTROL 組合圖表]** 按鈕並選取 [!UICONTROL 專案] > [!UICONTROL 實際成本] 在 **[!UICONTROL 值]** 欄位。
1. 按一下顏色方塊旁的箭頭以變更 [!UICONTROL 實際成本] 顏色。 選取顯示的顏色之一，或按一下右下角的方塊以開啟調色盤。
1. 按一下 **[!UICONTROL 儲存+關閉]**. 當系統提示您輸入報表名稱時，請將其稱為「按上季度完成的專案列出的計畫與實際成本」。

   ![新增圖表至報表的畫面影像](assets/chart-report-chart.png)
