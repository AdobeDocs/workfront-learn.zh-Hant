---
title: 自訂系統範圍的問題狀態
description: 瞭解如何變更問題狀態名稱、控制使用狀態的問題型別，以及鎖定/解鎖群組層級自訂的狀態。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10030
exl-id: c8f5677f-8d9d-4d1a-a1e3-d1a438878213
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# 自訂系統範圍狀態

[!DNL Workfront] 提供各種預設狀態，以配合您組織的問題管理工作流程。 這些狀態可重新命名以符合貴組織的術語。 可將和狀態指派給特定問題型別。

如有需要，可建立其他狀態。 只有系統管理員可以建立系統範圍的狀態。 此外，系統管理員可控制群組管理員可編輯哪些狀態。

![[!UICONTROL 問題] 定位於 [!UICONTROL 雕像] 第頁於 [!UICONTROL 設定]](assets/admin-fund-all-issue-statuses.png)

## 修改現有狀態

[!DNL Workfront] 建議狀態數下限。 這可讓使用者更輕鬆地選擇正確的狀態，並導致要維護較短的狀態清單。

您可以編輯現有狀態以變更名稱、指派給它的問題型別、相關顏色等。

![問題狀態清單，具有 [!UICONTROL 編輯] 醒目提示選項](assets/admin-fund-edit-issue-status.png)

1. 按一下 **[!UICONTROL 設定]** 在 **[!UICONTROL 主要功能表]**.
1. 展開 **[!UICONTROL 專案偏好設定]** 區段。
1. 選取 **[!UICONTROL 狀態]**.
1. 選取 **[!UICONTROL 問題]** 標籤並確認 [!UICONTROL 系統狀態] 會在右上角顯示。
1. 選取 **[!UICONTROL 主清單]** 以檢視所有問題型別的狀態。 您可在此處建立或修改問題狀態。
1. 將游標停留在您要重新命名的狀態右側，然後按一下 **[!UICONTROL 編輯]**.
1. 視需要為狀態指定新名稱或變更任何其他資訊。
1. 若這些設定應套用至您的中的所有使用者，請鎖定狀態。 [!DNL Workfront] 執行個體。
1. 解鎖狀態以允許群組管理員僅編輯其群組的狀態。
1. 核取狀態應套用至的問題型別方塊。
1. 按一下&#x200B;**[!UICONTROL 儲存]**。

![建立新狀態的視窗](assets/admin-fund-edit-issue-status-2.png)

### 狀態指派

並非所有狀態都可指派給所有問題型別。 此 [!UICONTROL 狀態] 頁面有欄顯示每個狀態可以使用的問題型別。

![在「狀態」頁面的「問題」標籤上反白顯示的變更順序](assets/admin-fund-issue-type-statuses.png)


若要只檢視指派給特定問題型別的狀態，只需按一下視窗頂端的問題型別名稱。

![[!UICONTROL 問題] 索引標籤/ [!UICONTROL 狀態] 反白欄的頁面](assets/admin-fund-statuses-issue-type.png)

從這裡，您可以將問題拖放至您希望它們在 [!UICONTROL 狀態] 下拉式功能表。

若要編輯狀態，您必須返回 [!UICONTROL 主清單].
