---
title: 了解如何在 [!UICONTROL 增強的Analytics]
description: 了解如何閱讀Workfront的飛行計畫圖。
activity: use
feature: Reports and Dashboards
thumbnail: 335047.png
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8729
exl-id: 1409a1af-3bdb-40f7-af01-f9de2357b602
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# 了解如何在 [!UICONTROL 增強的Analytics]

在此影片中，您將學習：

* 如何閱讀飛行計畫圖

>[!VIDEO](https://video.tv.adobe.com/v/335047/?quality=12&learn=on)

## 飛行計畫圖

![飛行計畫圖的影像，其編號與下面的項目符號匹配](assets/section-2-1.png)

在圖表上，您會看到：

1. 專案名稱位於左側。
1. 日期會顯示在底部。
1. 垂直藍線顯示滑鼠暫留的特定日期。
1. 水準藍線顯示項目的計劃開始和結束日期。
1. 綠線表示專案在Target上。
1. 橘線表示項目處於風險中。
1. 紅線表示項目出現問題。

查看此專案相關資訊有助於您判斷：

* 哪些事件會將專案延長至超過計畫完成日期。
* 當專案開始發生問題時。
* 同一時段內開啟的專案數量。
* 有多少個活動項目。
* 哪些項目需要額外的關注或支援。

## 條件是根據進度狀態

專案條件是專案進展情形的視覺表示。 Workfront會根據專案內工作的進度狀態來決定條件。

![可能的進度狀態的影像](assets/section-2-2.png)

可設定專案的條件：

* **手動**，當專案的條件類型設為手動時，即由有權管理專案的使用者執行。 這允許您獨立於關鍵路徑設定項目的條件。
* **自動**，當專案的條件類型設為「進度狀態」時，即由Workfront顯示。

Workfront建議您將條件類型設為「進度狀態」，以便根據任務進度清楚指出專案的真正進度。

![可能的進度狀態的影像](assets/section-2-3.png)

在此情況下，專案條件可以是：

* **在Target上** — 當關鍵路徑上最後一個任務的進度狀態為「準時」時，項目的條件將為「目標」。 項目正在按計畫完成。
* **風險** — 當關鍵路徑上最後一個任務的進度狀態為「落後」或「處於風險」時，則項目的狀態為「處於風險」。 該項目正按計畫延遲完成，但尚未延遲。
* **麻煩** — 當關鍵路徑上最後一個任務的進度狀態為「延遲」時，則項目的條件為「有故障」。 到期日已過，項目現在已延遲。

>[!NOTE]
>
>您可以根據您的環境自訂條件，因此您可能會找到三個以上的選項，或者名稱可能與上述選項不同。 如需自訂條件的相關資訊，請參閱建立或編輯自訂條件一文。
