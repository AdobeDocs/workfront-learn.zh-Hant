---
title: 建立矩陣報表
description: 瞭解矩陣報表何時有用，以及如何在Workfront中建立矩陣報表。
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
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# 建立矩陣報表

在本影片中，您將瞭解：

* 矩陣報表何時有用
* 以及如何建立矩陣報表

>[!VIDEO](https://video.tv.adobe.com/v/335156/?quality=12&learn=on)

## 活動：建立矩陣報表

建立矩陣報表，顯示每個狀態有多少請求，並按請求佇列排序。 這可讓您快速瞭解需要完成的工作量，以及您跟進工作的程度。

您希望請求佇列出現在列分組中。 狀態會顯示為欄群組。 將報表命名為「依狀態的要求與要求佇列」。

## 答案

1. 選取 **[!UICONTROL 報表]** 從 **[!UICONTROL 主要功能表]**.
1. 按一下 **[!UICONTROL 新報告]** 選項並選取 **[!UICONTROL 問題]**.
1. 前往 **[!UICONTROL 群組]** 標籤並按一下 **[!UICONTROL 切換至矩陣群組]**.
1. 對象 [!UICONTROL 列群組]，選取 **[!UICONTROL 專案]** > **[!UICONTROL 名稱]**.
1. 對象 [!UICONTROL 欄分組]，選取 **[!UICONTROL 問題]** > **[!UICONTROL 狀態]**.

   ![建立新問題報告分組的畫面影像](assets/matrix-report-groupings.png)

1. 前往 **[!UICONTROL 篩選器]** 標籤。
1. 若要確定您只看到作用中請求佇列中的請求，請新增下列篩選規則：

   * [!UICONTROL 專案] > [!UICONTROL 狀態等同於] > [!UICONTROL 等於] > [!UICONTROL 目前]
   * [!UICONTROL 佇列定義] > [!UICONTROL 為公開] > [!UICONTROL 不等於] > [!UICONTROL 無] （這就是我們如何知道專案實際上是一個請求佇列，透過將佇列定義指派給其中一個公用選項。）

1. 按一下 **[!UICONTROL 儲存+關閉]**. 當系統提示您輸入報表名稱時，請輸入「按狀態的請求和請求佇列」。

   ![建立新問題報告篩選器的畫面影像](assets/matrix-report-filters.png)
