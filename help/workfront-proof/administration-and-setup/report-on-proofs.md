---
title: 校樣報告
description: 了解如何使用報表功能來管理校樣進度。
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: report-on-proofs.png
kt: 10233
exl-id: 9a1a9e16-61cc-4f95-977a-8870b7fd0dda
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# 校樣報告

[!DNL Workfront]數位校對功能可讓您集中管理專案和相關的審核工作流程 —  [!DNL Workfront]. 深入了解正在使用報表類型、欄位來源和欄位名稱（顯示審核和核准資訊）進行的校對工作。

建議您使用 [!DNL Workfront] 顧問，以建立符合貴組織需求的報表。 有些報表需要熟悉 [!DNL Workfront]的文本模式報告。

從這些基本的標準報表開始，協助您的團隊管理進行審核和核准程式的校樣。 [!DNL Workfront].

## [!UICONTROL 校訂核准]

此報表類型可協助您追蹤未結的校樣核准，以確保符合期限。

![選擇 [!UICONTROL 證明核准] 從 [!UICONTROL 新增報表] 下拉式功能表](assets/proof-system-setups-proof-approval-report.png)

檢視和篩選選項包括 [!UICONTROL 決定日期], [!UICONTROL 證明批准], [!UICONTROL 核准者階段], [!UICONTROL 工作流程範本]，和 [!UICONTROL 請求者資訊]. 使用文本模式報告，可以建立按文檔名稱組織清單的分組。

撰寫校樣核准報表時，請務必取得與最新版本校樣相關的資訊。 [!DNL Workfront] 建議在篩選器中包含此欄位來源和欄位名稱：

**[!UICONTROL 證明核准]>>[!UICONTROL 是當前文檔版本]**

![Report Builder中的「篩選器」索引標籤](assets/proof-system-setups-proof-approval-report-is-current-version.png)

如果您報告的校樣有多個版本，這個功能會很實用，因此報表只會列出需要核准的每個校樣的最新版本。 這會篩選掉您不再需要使用的舊版。

## [!UICONTROL 文件版本]

此報表類型可讓您管理及追蹤 [!DNL Workfront].

![選擇 [!UICONTROL 文檔版本] 從 [!UICONTROL 新增報表] 下拉式功能表](assets/proof-system-setups-document-version-report.png)

檢視選項包含 [!UICONTROL 檔案版本], [!UICONTROL 檔案], [!UICONTROL 輸入], [!UICONTROL 證明批准狀態], [!UICONTROL 證明建立者]，和 [!UICONTROL 檔案提供者].

分組可依 [!UICONTROL 檔案版本], [!UICONTROL 輸入], [!UICONTROL 證明批准狀態]，或證明擁有者資訊。

篩選器包括 [!UICONTROL 檔案版本], [!UICONTROL 存取層級], [!UICONTROL 檔案], [!UICONTROL 輸入], [!UICONTROL 證明批准狀態], [!UICONTROL 證明建立者]，以及檔案提供者資訊。

您可以顯示校對階段的名稱，該測試階段目前對報表上具有此欄的每個檔案都有效，並以檢視顯示：

**[!UICONTROL 文檔版本] >> [!UICONTROL 活動校樣階段]**

![Report Builder中的「篩選器」索引標籤](assets/proof-system-setups-active-proof-stages.png)

如果當前沒有活動階段，則列為空。

此欄位來源>>欄位名稱也可作為報表中的篩選器。

使用 [!UICONTROL 校樣建立者] 欄位來源，報告建立校樣的使用者的相關資訊。 選擇 [!UICONTROL 名稱] 欄位來源，在視圖中顯示校樣建立者的名稱。

**[!UICONTROL 校樣建立者] >> [!UICONTROL 名稱]**

此欄位源>>欄位名稱組合也可作為篩選器使用。

![Report Builder中的「篩選器」索引標籤](assets/proof-system-setups-proof-creator-name.png)

<!--
Learn More Icon
Learn how to create reports in [!DNL Workfront] with the Report Creation class.
Access to proofing functionality
-->
