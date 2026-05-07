---
title: 設定中繼資料對應
description: 了解如何設定 [!UICONTROL Workfront DAM] 的中繼資料對應。
activity: use
team: Technical Marketing
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
jira: KT-10088
exl-id: 3869db93-9fbc-4689-b838-0f4400a436c3
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T22:32:59.006Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 276
ht-degree: 100%

---

# 設定中繼資料對應

關於資產的 [!DNL Workfront] 相關資訊可以與資產一起從 [!DNL Workfront] 轉移到 [!UICONTROL Workfront DAM]。 在 [!DNL Workfront]「[!UICONTROL 設定]」區域的中繼資料對應選項允許上述資訊轉移。

關於設定中繼資料對應的最佳實務建議，請與您的 [!DNL Workfront] 顧問討論。

您必須是 [!DNL Workfront] 管理員和 [!UICONTROL Workfront DAM] 管理員才能設定中繼資料對應。 在開始之前，您必須連接您的 [!DNL Workfront] 和 [!UICONTROL Workfront DAM] 帳戶。

## 連接帳戶

1. 登入 [!DNL Workfront]。
1. 開啟專案、任務或問題，然後按一下「**[!UICONTROL 文件]**」標籤。
1. 按一下「**[!UICONTROL 新增]**」按鈕然後從下拉式選單選取「**[!UICONTROL 從 Workfront DAM]**」
1. 在所出現的 [!UICONTROL Workfront DAM] 授權方塊中輸入您的登入名稱和密碼。
1. 接下來，按一下「**[!UICONTROL 是]**」，把 [!DNL Workfront] 存取權授予 [!UICONTROL DAM] 帳戶。
1. 如有需要，請重新整理頁面，更新對 [!UICONTROL Workfront DAM] 的存取權。

建立此連線後，現在您可以開始在兩個系統之間對應中繼資料。 在開始對應之前，請確認您已經在 [!UICONTROL Workfront DAM] 中建立所需的中繼資料欄位。

## 設定對應

1. 登入 [!DNL Workfront]。
1. 從[!UICONTROL 主選單]選取「**[!UICONTROL 設定]**」。
1. 展開左側面板選單中的「**[!UICONTROL 文件]**」區段。
1. 然後按一下「**[!UICONTROL 中繼資料對應]**」。
1. 在 Workfront 欄位中，輸入要對應的 [!DNL Workfront] 欄位的欄位來源。
1. 然後選取對應的或目標 **[!UICONTROL Workfront DAM]** 中繼資料欄位。
1. 按一下「**[!UICONTROL 新增對應]**」按鈕。
1. 您會在視窗底部的圖表中看到「[!UICONTROL Workfront 欄位來源]」和「[!UICONTROL Workfront DAM 目標欄位]」。
1. 所需的全部中繼資料欄位均重複上述步驟。

![螢幕擷圖顯示[!UICONTROL 中繼資料對應]畫面，位於 [!DNL Workfront]](assets/01-metadata-mapping.png)
