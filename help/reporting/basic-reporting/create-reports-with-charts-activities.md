---
title: 使用圖表活動建立報表
description: 練習使用圖表建立報告，並附有逐步指示。
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335153.png
jira: KT-8860
hidefromtoc: true
source-git-commit: 915b28bbbf138fa84dce6d1915387fbe22c63362
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 81%

---

# 使用圖表活動建立報表

練習使用圖表建立報告，並附有逐步指示。

## 活動1：新增圖表至報表

臨近季末，您想瞭解最近完成的專案是否控制在預算範圍內。建立一份報告，比較專案的規劃成本與實際成本。您只想查看上一季度完成的專案。使用自訂顏色新增組合欄圖表。

## 答案1

1. 在&#x200B;**[!UICONTROL 主選單]**&#x200B;中選取「**[!UICONTROL 報告]**」。
1. 按一下「**[!UICONTROL 新增報告]**」選單並選取「**[!UICONTROL 專案]**」。
1. 在「**[!UICONTROL 欄 (視圖)]**」標籤中，按一下「**[!UICONTROL 新增欄]**」。
1. 選取「[!UICONTROL 專案]」>「[!UICONTROL 規劃成本]」，並使用「**[!UICONTROL 總和]**」將這一欄加總。
1. 再按一下「**[!UICONTROL 新增欄]**」。
1. 選取「[!UICONTROL 專案]」>「[!UICONTROL 實際成本]」，並使用「**[!UICONTROL 總和]**」將這一欄加總。

   ![影像顯示在報告中新增欄的畫面](assets/chart-report-columns.png)

1. 在「**[!UICONTROL 分組]**」標籤中，設定報告依照「[!UICONTROL 專案]」>「[!UICONTROL 名稱]」分組。

   ![影像顯示在報告中新增分組的畫面](assets/chart-report-groupings.png)

1. 在「**[!UICONTROL 篩選器]**」標籤中，新增兩個篩選規則：

   * 「[!UICONTROL 專案]」>「[!UICONTROL 狀態等同於]」>「[!UICONTROL 完成]」
   * 「[!UICONTROL 專案]」>「[!UICONTROL 實際完成日期]」>「[!UICONTROL 上一季]」

   ![影像顯示在報告中新增篩選器的畫面](assets/chart-report-filters.png)

1. 在「**[!UICONTROL 圖表]**」標籤中，圖表類型請選擇「**[!UICONTROL 欄]**」。
1. 對「[!UICONTROL 左 (Y) 軸]」，選擇「[!UICONTROL 專案]」>「[!UICONTROL 規劃成本]」。
1. 對「[!UICONTROL 底部 (X) 軸]」，選擇「[!UICONTROL 專案]」>「[!UICONTROL 名稱]」。
1. 按一下「**[!UICONTROL 組合圖表]**」按鈕並在「**[!UICONTROL 價值]**」欄位中選取「[!UICONTROL 專案]」>「[!UICONTROL 實際成本]」。
1. 按一下顏色方塊旁邊的箭頭來變更「[!UICONTROL 實際成本]」的顏色。選取其中一個出現的顏色，或是按一下右下角的方塊來開啟調色盤。
1. 按一下「**[!UICONTROL 儲存並關閉]**」。當系統提示您輸入報表名稱時，請將其稱為「按上季度完成的專案列出的計畫與實際成本」。

   ![影像顯示在報告中新增圖表的畫面](assets/chart-report-chart.png)
