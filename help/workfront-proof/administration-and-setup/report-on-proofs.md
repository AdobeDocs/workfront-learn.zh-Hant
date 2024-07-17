---
title: 關於校訂的報告
description: 瞭解如何使用報告功能來管理校訂進度。
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: report-on-proofs.png
jira: KT-10233
exl-id: 9a1a9e16-61cc-4f95-977a-8870b7fd0dda
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 100%

---

# 關於校訂的報告

您可以利用 [!DNL Workfront] 的數位校訂功能來管理專案和相關的檢閱工作流程，全部都有 [!DNL Workfront] 中完成。利用報告類型、欄位來源以及顯示檢閱與核准資訊的欄位名稱，取得有關所做校訂工作的重要分析。

我們建議與您的 [!DNL Workfront] 顧問一起合作，建立符合組織需求的報告。有些報告必須熟悉 [!DNL Workfront] 文字模式報告功能方能使用。

從這些基本的標準報告開始，幫助您的團隊管理在 [!DNL Workfront] 中進行檢閱與核准流程的校訂。

## [!UICONTROL 校訂核准]

此報告類型可協助您追蹤未完成的校訂核准，以確保在截止之前完成。

![從「[!UICONTROL 新增報告]」下拉式選單選取「[!UICONTROL 校訂核准]」](assets/proof-system-setups-proof-approval-report.png)

檢視和篩選選項包括「[!UICONTROL 決定日期]」、「[!UICONTROL 校訂核准]」、「[!UICONTROL 核准者階段]」、「[!UICONTROL 工作流程範本]」和「[!UICONTROL 請求者資訊]」。您可以利用文字模式報告來建立分組，依文件名稱來整理清單。請參閱「[瞭解分組的基本文字模式](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/basic-text-mode-for-groupings.html?lang=zh-Hant)」。

在編寫校訂核准報告時，請確認您取得的資訊與最新版本的校訂相關。[!DNL Workfront] 建議篩選器應包含這個欄位來源和欄位名稱：

「**[!UICONTROL 校訂核准] >> [!UICONTROL 是目前文件版本]**」

![報告建立工具的篩選器標籤](assets/proof-system-setups-proof-approval-report-is-current-version.png)

當您所要報告的校訂含有多個版本時，這項功能十分實用，報告僅列出需要核准的每份校訂的最新版本。這樣便會把您不再需要處理的早期版本篩除。

## [!UICONTROL 文件版本]

此報告類型允許您在 [!DNL Workfront] 中管理和追蹤版本。

![從「[!UICONTROL 新增報告]」下拉式選單中選取「[!UICONTROL 文件版本]」](assets/proof-system-setups-document-version-report.png)

檢視選項包括來自「[!UICONTROL 文件版本]」、「[!UICONTROL 文件]」、「[!UICONTROL 輸入者]」、「[!UICONTROL 校訂核准狀態]」、「[!UICONTROL 校訂建立者]」以及「[!UICONTROL 文件提供者]」的資訊。

您可以依據「[!UICONTROL 文件版本]」、「[!UICONTROL 輸入者]」、「[!UICONTROL 校訂核准狀態]」或「校訂所有者資訊」來進行分組。

篩選器包括「[!UICONTROL 文件版本]」、「[!UICONTROL 存取層級]」、「[!UICONTROL 文件]」、「[!UICONTROL 輸入者]」、「[!UICONTROL 校訂核准狀態]」以及「[!UICONTROL 校訂建立者]」和「文件提供者」的資訊。

報告上每份文件，其視圖上有這一欄時，您可以顯示目前使用中的校訂階段的名稱。

「**[!UICONTROL 文件版本] >> [!UICONTROL 使用中校訂階段]**」

![報告建立工具的篩選器標籤](assets/proof-system-setups-active-proof-stages.png)

如果目前沒有進行中的階段，則該欄留白。

在報告中也可以使用這個「欄位來源 >> 欄位名稱」作為篩選器。

使用「[!UICONTROL 校訂建立者]」欄位來源，報告關於建立校訂之使用者的資訊。選擇「[!UICONTROL 名稱]」欄位來源，在視圖中顯示校訂建立者的名稱。

「**[!UICONTROL 校訂建立者] >> [!UICONTROL 名稱]**」

這個「欄位來源 >> 欄位名稱」的組合也可以用作篩選器。

![報告建立工具的篩選器標籤](assets/proof-system-setups-proof-creator-name.png)

<!--
Learn More Icon
Learn how to create reports in [!DNL Workfront] with the Report Creation class.
Access to proofing functionality
-->
