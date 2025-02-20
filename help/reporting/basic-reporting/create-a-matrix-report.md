---
title: 建立矩陣報告
description: 瞭解矩陣報告的適用時機以及在 Workfront 中如何建立矩陣報告。
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335156.png
jira: KT-8861
exl-id: e893d94a-e808-4bc1-bc6e-f46a5582b55d
doc-type: video
source-git-commit: 6afb57b983b094f9bc0c082a160453ecb394ca8e
workflow-type: ht
source-wordcount: '268'
ht-degree: 100%

---

# 建立矩陣報告

觀看這段影片，您將會瞭解：

* 矩陣報告的適用時機
* 以及如何建立矩陣報告

>[!VIDEO](https://video.tv.adobe.com/v/335156/?quality=12&learn=on)

## 建立矩陣報告活動

[按一下這裡](/help/assets/create-matrix-report-activities.pdf)下載此頁面的 PDF 版本。

### 活動 1：建立矩陣報告

建立一份矩陣報告，顯示每個狀態的請求數量，並依請求佇列排序。您可以透過這份報告迅速掌握即將到來的工作量，以及您目前是否跟上進度。

您想要讓請求佇列依列分組顯示。而狀態依欄分組顯示。將報告命名為「依狀態和請求佇列排序的請求」。

### 解答 1

1. 在&#x200B;**[!UICONTROL 主選單]**&#x200B;中選取「**[!UICONTROL 報告]**」。
1. 按一下「**[!UICONTROL 新增報告]**」選項並選取「**[!UICONTROL 問題]**」。
1. 前往「**[!UICONTROL 分組]**」標籤並按一下「**[!UICONTROL 切換至矩陣分組]**」。
1. 對於「[!UICONTROL 列分組]」，請選取「**[!UICONTROL 專案]**」>「**[!UICONTROL 名稱]**」。
1. 對於「[!UICONTROL 欄分組]」，選取「**[!UICONTROL 問題]**」>「**[!UICONTROL 狀態]**」。

   ![影像顯示建立新問題報告分組的畫面](assets/matrix-report-groupings.png)

1. 前往「**[!UICONTROL 篩選器]**」標籤。
1. 為了確保您只看到使用中之請求佇列中的請求，請新增以下篩選規則：

   * 「[!UICONTROL 專案]」>「[!UICONTROL 狀態等同於]」>「[!UICONTROL 等於]」>「[!UICONTROL 目前]」
   * 「[!UICONTROL 佇列定義]」>「[!UICONTROL 是公開的]」>「[!UICONTROL 不等於]」>「[!UICONTROL 無]」(這是我們確認專案確實是請求佇列的方法，依照指派給其中一個公開選項的佇列定義。)

1. 按一下「**[!UICONTROL 儲存並關閉]**」。系統提示輸入報告名稱時，請輸入「依狀態和請求佇列排序的請求」。

   ![影像顯示建立新問題報告篩選器的畫面](assets/matrix-report-filters.png)
