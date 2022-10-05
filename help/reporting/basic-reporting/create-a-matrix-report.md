---
title: 建立矩陣報表
description: 此影片會說明矩陣報表何時有用，以及如何在 [!DNL  Workfront].
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335156.png
kt: 8861
exl-id: e893d94a-e808-4bc1-bc6e-f46a5582b55d
source-git-commit: f4000878d453c58fabf34308a8e3ab31d9667a1f
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---

# 建立矩陣報表

在此影片中，您將學習：

* 矩陣報表可能有用時
* 以及如何建立矩陣報表

>[!VIDEO](https://video.tv.adobe.com/v/335156/?quality=12)

## 活動：建立矩陣報表

建立矩陣報表，依請求佇列排序，顯示每個狀態中有多少個請求。 這可以快速了解工作量，以及您如何跟上進度。

您希望請求佇列在列群組中顯示。 狀態顯示為列分組。 將報表命名為「依狀態和請求佇列的請求」。

## 回答

1. 選擇 **[!UICONTROL 報表]** 從 **[!UICONTROL 主菜單]**.
1. 按一下 **[!UICONTROL 新增報表]** 選項，然後選取 **[!UICONTROL 問題]**.
1. 前往 **[!UICONTROL 分組]** 按一下 **[!UICONTROL 切換到矩陣分組]**.
1. 針對 [!UICONTROL 列分組]，選取 **[!UICONTROL 專案]** > **[!UICONTROL 名稱]**.
1. 針對 [!UICONTROL 欄分組]，選取 **[!UICONTROL 問題]** > **[!UICONTROL 狀態]**.

   ![建立新問題報告分組的螢幕影像](assets/matrix-report-groupings.png)

1. 前往 **[!UICONTROL 篩選器]** 標籤。
1. 若要確定您在使用中的請求佇列中只看到請求，請新增下列篩選規則：

   * [!UICONTROL 專案] > [!UICONTROL 狀態等於] > [!UICONTROL 等於] > [!UICONTROL 目前]
   * [!UICONTROL 隊列定義] > [!UICONTROL 為公用] > [!UICONTROL 不等於] > [!UICONTROL 無] （這是我們如何得知專案實際上是請求佇列，由「佇列定義」指派給其中一個公用選項。）

1. 按一下 **[!UICONTROL 儲存+關閉]**. 提示輸入報表名稱時，請輸入「依狀態和請求佇列的請求」。

   ![建立新問題報告篩選器的螢幕影像](assets/matrix-report-filters.png)
