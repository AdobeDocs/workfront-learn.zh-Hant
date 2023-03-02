---
title: 配置全局預設項目設定
description: 了解如何變更自訂狀態、設定全域專案偏好設定，以及建立全域預設設定的排程。
feature: System Setup and Administration
role: Admin
level: Intermediate
activity: deploy
type: Tutorial
team: Technical Marketing
thumbnail: 335065.png
kt: 8753
exl-id: b961ba8c-9597-4ed4-a6d7-79689c8e290d
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# 配置全局預設項目設定

<!---
21.4 updates have been made
--->

在此影片中，您將學習如何：

* 變更自訂狀態
* 設定全局項目首選項
* 建立和使用排程

>[!VIDEO](https://video.tv.adobe.com/v/335065/?quality=12)

## 全局和組項目、任務和問題設定

當您開啟 [!UICONTROL 專案] 設定 [!DNL Workfront]，您會注意到上面寫著「[!UICONTROL 系統項目首選項]」（位於窗口頂部的搜索欄）。 這可讓您知道這些設定會影響 [!DNL Workfront] 系統 — 它是全局配置。

![[!UICONTROL 專案偏好設定] 頁面 [!UICONTROL 設定]](assets/admin-fund-system-project-preferences-1.png)

開啟 [!UICONTROL 工作與問題] 設定。

![[!UICONTROL 任務和問題首選項] in [!UICONTROL 設定]](assets/admin-fund-task-issue-preferences-2.png)

但是，可能不是每個組 [!DNL Workfront] 需要相同的項目、任務和問題首選項。 例如，行銷群組希望新專案的狀態為「計畫」，而專案管理員群組則偏好「請求」狀態。

[!DNL Workfront] 允許組管理員調整其組的特定項目、任務和問題首選項。 可調整的偏好設定由 [!DNL Workfront] 系統管理員使用鎖定/解除鎖定進行切換。

首先，導覽至 [!UICONTROL 設定] 區域：

1. 選擇 **[!UICONTROL 設定]** 在 **[!UICONTROL 主菜單]**.
1. 展開 **[!UICONTROL 專案偏好設定]** 的上界。
1. 選擇 **[!UICONTROL 專案]** 或 **[!UICONTROL 工作與問題]**，視您要修改的設定而定。

鎖定偏好設定，以防止群組管理員調整其群組的設定。

![鎖定的首選項消息](assets/admin-fund-preferences-locked-3.png)

解除鎖定偏好設定，讓群組管理員可加以自訂。

![未鎖定首選項消息](assets/admin-fund-preferences-unlocked-4.png)

某些設定無法解鎖，並保持全局系統設定。

![鎖定的首選項消息](assets/admin-fund-preferences-always-locked-5.png)

### 設定組和子組首選項

對於系統管理員解除鎖定的任何設定，組管理員可以對其管理的組以及這些組下嵌套的任何子組進行調整。 此外，組管理員可以控制其子組管理員可以修改的設定。

1. 選擇 **[!UICONTROL 設定]** 在 **[!UICONTROL 主菜單]**.
1. 按一下 **[!DNL Groups]** 的上界。
1. 按一下組或子組名稱以開啟它。
1. 選擇 **[!UICONTROL 專案偏好設定]** 或 **[!UICONTROL 任務和問題首選項]** 的上界。
1. 進行已解鎖的每個首選項所需的更改。
1. 選擇 **[!UICONTROL 儲存]**.

![[!UICONTROL 專案狀態] 一節 [!UICONTROL 群組] 頁面](assets/admin-fund-group-preferences.png)

如果您的組織未使用群組管理員，系統管理員可以管理不同群組的偏好設定。

<!---
learn more URLs and guides
Create or edit a group status 
Group administrators 
Configure system-wide project preferences 
Configure project preferences for a group 
Configure task and issue preferences for a group 
Create and modify a group’s schedule 
--->
