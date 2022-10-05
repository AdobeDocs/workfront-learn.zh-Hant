---
title: 自定義全系統問題狀態
description: 了解如何變更問題狀態名稱、控制用於狀態的問題類型，以及鎖定/解除鎖定群組層級自訂的狀態。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
kt: 10030
exl-id: c8f5677f-8d9d-4d1a-a1e3-d1a438878213
source-git-commit: 02bc5a09a838be6d98c9b746bff731236ee4116f
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# 自定義全系統狀態

[!DNL Workfront] 提供各種預設狀態，以因應貴組織的問題管理工作流程。 您可以重新命名這些狀態，以符合貴組織的術語。 狀態可指派給特定問題類型。

如有需要，可建立其他狀態。 只有系統管理員可以建立系統範圍的狀態。 此外，系統管理員可控制哪些狀態可供群組管理員編輯。

![[!UICONTROL 問題] 標籤 [!UICONTROL 雕像] 頁面 [!UICONTROL 設定]](assets/admin-fund-all-issue-statuses.png)

## 修改現有狀態

[!DNL Workfront] 建議狀態數量下限。 這可讓使用者更輕鬆選擇正確的狀態，並產生更短的狀態清單以供維護。

您可以編輯現有狀態以變更名稱、指派給的問題類型、相關顏色等。

![問題狀態清單 [!UICONTROL 編輯] 突出顯示的選項](assets/admin-fund-edit-issue-status.png)

1. 按一下 **[!UICONTROL 設定]** 在 **[!UICONTROL 主菜單]**.
1. 展開 **[!UICONTROL 專案偏好設定]** 區段。
1. 選擇 **[!UICONTROL 狀態]**.
1. 選取 **[!UICONTROL 問題]** 標籤，確保 [!UICONTROL 系統狀態] 顯示於右上角。
1. 選擇 **[!UICONTROL 主清單]** ，查看所有問題類型的狀態。 您可以在此處建立或修改問題狀態。
1. 將滑鼠指標暫留在您要重新命名的狀態右側，然後按一下 **[!UICONTROL 編輯]**.
1. 為狀態指定新名稱，或視需要變更任何其他資訊。
1. 如果這些設定應套用至 [!DNL Workfront] 例項。
1. 解除鎖定狀態，允許群組管理員僅編輯其群組的狀態。
1. 勾選狀態應套用的問題類型方塊。
1. 按一下 **[!UICONTROL 儲存]**.

![建立新狀態的窗口](assets/admin-fund-edit-issue-status-2.png)

### 狀態分配

並非所有狀態都可指派給所有問題類型。 此 [!UICONTROL 狀態] 頁面中有欄顯示每個狀態可用於的問題類型。

![在「狀態」頁的「問題」頁簽上突出顯示更改順序](assets/admin-fund-issue-type-statuses.png)


要僅查看指定給特定問題類型的狀態，只需按一下窗口頂部的問題類型名稱即可。

![[!UICONTROL 問題] 標籤 [!UICONTROL 狀態] 高亮顯示列的頁面](assets/admin-fund-statuses-issue-type.png)

從這裡，您可以將問題拖放至您希望問題在 [!UICONTROL 狀態] 下拉式功能表。

若要編輯狀態，您必須返回 [!UICONTROL 主清單].
