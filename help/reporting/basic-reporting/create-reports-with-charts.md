---
title: 建立附有圖表的報告
description: 圖表透過可自訂的篩選器、分組和棧疊欄格式來組織資料深入分析，讓分析更清晰、更易於操作，藉此增強資料視覺化。
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335153.png
jira: KT-8860
last-substantial-update: 2025-05-06T00:00:00Z
exl-id: ea3b360b-1fbd-4d1a-b505-b75759d24e41
doc-type: video
source-git-commit: cc423944628d01e16d390842ecb25696505f923c
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 39%

---

# 建立附有圖表的報告

影片說明如何使用圖表來有效地視覺化資料，尤其是追蹤專案任務時。&#x200B;URL 它示範如何在Workfront中建立兩種型別的報表：

**依專案報告的延遲任務：**

* 從清單報告開始，並套用篩選器以僅顯示目前專案中未完成、延遲的任務。&#x200B;URL
* 依專案名稱將任務分組，並建立圓形圖以視覺化跨專案延遲任務的分佈。&#x200B;URL
* 將圖表設定為預設標籤以方便存取。&#x200B;URL

**按專案和進度狀態報告的任務：**

* 複製第一個報告，並為任務進度狀態新增另一個分組。
* 移除篩選器以包含所有任務，在專案執行期間顯示其進度。
* 使用棧疊柱狀圖可顯示每個專案的任務總數，棧疊代表不同的進度狀態。
* 視需要自訂顏色並儲存報表。

影片重點說明圓形圖和棧疊直條圖等圖表如何提供任務分佈和專案效能的深入分析，以協助使用者比較專案並以視覺化方式瞭解任務進度。&#x200B;URL

>[!VIDEO](https://video.tv.adobe.com/v/3450025/?captions=chi_hant&quality=12&learn=on&enablevpops=0)

## 關鍵重點

* **圖表可增強資料清晰度**：使用圖表（例如圓形圖或直條圖）視覺化資料，與清單報告相比，更容易瞭解任務分佈和專案進度。&#x200B;URL
* **篩選特定深入分析**：套用篩選器（例如目前專案中未完成、延遲的工作）有助於將重點放在相關資料上以進行目標分析。&#x200B;URL
* **分組為更好的組織**：依專案名稱或進度狀態將任務分組會有效地組織資料，以便能夠跨專案進行有意義的比較。&#x200B;URL
* **圖表自訂選項**：使用者可以選取圖表型別（例如，圓形、欄、長條）並自訂顏色，以符合偏好設定或品牌化。&#x200B;URL
* **詳細深入分析的棧疊直條圖**：棧疊直條圖提供專案中任務進度的完整檢視，在單一視覺化中顯示任務總計及其狀態。


## 「建立附有圖表的報告」活動

### 活動 1：將圖表新增至報告中

臨近季末，您想瞭解最近完成的專案是否控制在預算範圍內。建立一份報告，比較專案的規劃成本與實際成本。您只想查看上一季度完成的專案。使用自訂顏色新增組合欄圖表。

### 解答 1

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
1. 針對[!UICONTROL 左(Y)軸]，選擇[!UICONTROL 計畫成本]。
1. 針對[!UICONTROL 底部(X)軸]，請選擇[!UICONTROL 名稱]。
1. 按一下&#x200B;**[!UICONTROL 組合圖表]**&#x200B;按鈕，並在[!UICONTROL 值]欄位中選取&#x200B;**[!UICONTROL 實際成本]**。
1. 在&#x200B;**[!UICONTROL 圖表型別]**&#x200B;欄位中，選取「線條」。
1. 按一下顏色方塊以變更[!UICONTROL 實際成本]顏色。 選取顏色。
1. 按一下「**[!UICONTROL 儲存並關閉]**」。系統提示輸入報告名稱時，請命名為「上一季已完成的專案之規劃成本與實際成本比較」。

   ![影像顯示將圖表新增至報告中的畫面](assets/chart-report-chart.png)
