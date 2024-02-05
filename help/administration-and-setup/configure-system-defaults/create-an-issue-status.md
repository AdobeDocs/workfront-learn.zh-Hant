---
title: 建立問題狀態
description: 瞭解如何建立問題狀態來滿足貴組織工作流程的需求。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10019
exl-id: 1689080d-1d3c-4fad-a353-64fb3b0d5851
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '284'
ht-degree: 100%

---

# 建立問題狀態

[!DNL Workfront] 建議您先修改系統中現有問題的狀態，然後再開始建立新狀態。這樣可以限制所需維護的狀態數量。

1. 在&#x200B;**[!UICONTROL 主選單]**&#x200B;中按一下「**[!UICONTROL 設定]**」。
1. 展開左側選單面板中的「**[!UICONTROL 專案偏好設定]**」區段。
1. 選取「**[!UICONTROL 狀態]**」。
1. 選取「**[!UICONTROL 問題]**」標籤。
1. 確認右上角的欄位設定為「[!UICONTROL 系統狀態]」。這樣可以確保在您的 [!DNL Workfront] 執行個體中全域均可使用新狀態。
1. 選取「**[!UICONTROL 主清單]**」來查看所有問題狀態。您可以在這裡建立或修改狀態。
1. 按一下「**[!UICONTROL 新增新狀態]**」。
1. 根據貴組織的需要填寫欄位 — 名稱、說明、顏色、等同於、索引鍵等。
1. 勾選可以使用此狀態的問題類型之方塊。
1. 按一下「**[!UICONTROL 儲存]**」。

![「[!UICONTROL 狀態]」頁面上的「新增狀態」視窗](assets/admin-fund-create-issue-status.png)

## 問題狀態和群組管理員

群組管理員可以為其管理的群組建立和自訂問題狀態。這樣一來，他們的群組因此享有一些自主權，擁有工作推展所需要的狀態。同時也不再需要冗長的全系統適用狀態清單。

如果系統管理員已為群組管理員設定自訂化功能，則群組管理員可以編輯現有狀態。

系統管理員在「[!UICONTROL 狀態]」視窗的右上角選取群組名稱，即可對群組狀態進行管理。

![「[!UICONTROL 狀態]」頁面上的群組清單選單](assets/admin-fund-change-group-master-list.png)

群組管理員可以按一下「[!UICONTROL 設定]」區域中的「[!UICONTROL 群組]」區段，按一下群組名稱來開啟群組，然後在左側面板選單上選取「[!UICONTROL 狀態]」。請務必選取「問題」標籤。

![[!UICONTROL 狀態]區段，位於[!UICONTROL 群組]頁面](assets/admin-fund-group-issue-statuses.png)

<!---
For detailed information on how managing statuses can be done by group administrators, see these articles:
Create and customize group statuses
Group administrators
--->

<!---
learn more URLs
Issue statuses
Create and customize system-wide statuses
--->
