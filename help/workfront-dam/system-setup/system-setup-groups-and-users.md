---
title: 設定群組和使用者
description: 了解如何在 [!UICONTROL Workfront DAM] 中建立資料夾、群組和使用者。了解使用者角色類型並授予資料夾權限。
activity: use
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
team: Technical Marketing
jira: KT-8967
exl-id: 4ebf675c-b72d-447e-b131-a89acb449e15
doc-type: video
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 95%

---

# 設定群組和使用者

觀看這段影片，您將了解如何：

* 了解群組設定如何影響對於資產的存取權
* 按特定順序建立資料夾、群組和使用者
* 了解使用者角色類型
* 將權限授予資料夾
* 建立和編輯群組
* 新增和編輯使用者

>[!VIDEO](https://video.tv.adobe.com/v/335230/?quality=12&learn=on&enablevpops)

## 群組和使用者檢閱

當您設定 [!UICONTROL Workfront DAM] 系統時，一定要用宏觀角度考慮使用者和群組所扮演的角色。

群組控制對於 [!UICONTROL Workfront DAM] 資產資料夾的存取權。群組設定也可控制使用者對擁有存取許可權的資產進行哪些操作（檢視、下載、編輯等）。

建立群組時，一定要記得該群組的成員需要存取 [!UICONTROL Workfront DAM] 哪些資產資料夾。

使用者是指具有 [!UICONTROL Workfront DAM] 登入權限的個人。使用者無法存取 [!UICONTROL Workfront DAM] 中任何內容，除非他們被指派至一個群組。使用者可以屬於一個以上的群組，依他們的需求決定。

## 預設群組

[!UICONTROL Workfront DAM] 有兩個預設群組。所有使用者會自動納入這些群組，根據其是否具有 [!UICONTROL Workfront DAM] 登入憑證而定。這些群組無法新增或移除使用者：

* **訪客群組** — 用來控制匿名使用者的存取權。這可能是沒有登入憑據的人或目前並未登入的使用者。
* **已登入**&#x200B;群組 — 已登入的所有使用者屬於這個群組。

管理員群組及其設定均是預設存在。您可以將使用者新增到這個群組但是無法調整設定。

## 角色類型

所建立的群組會被指派一個角色類型。角色類型決定使用者登入時可以存取 [!UICONTROL Workfront DAM] 系統的哪個部分：[!UICONTROL Workfront DAM] 本身或是 [!UICONTROL Brand Connect]。

[!UICONTROL Workfront DAM] 授權可以使用三種角色類型：

* **[!UICONTROL Brand Portal]** — 這類使用者僅可存取 [!UICONTROL Brand Connect]，並且檢視及下載已核准的資產。
* **[!UICONTROL 貢獻者]** — 這類使用者可以存取 [!UICONTROL Workfront DAM] 和 [!UICONTROL Brand Connect]。他們擁有資產和資料夾的完整存取權，可以檢視、下載、上傳、編輯、移動和刪除。
* **[!UICONTROL 管理員]** — 系統管理員可以存取 [!UICONTROL Brand Connect] 和 [!UICONTROL Workfront DAM] 中所有內容，並可以建立個別的全域系統設定。他們也可以存取已經過期或被設定為非使用的資產。

<!-- 
Learn more graphic & documentation article link, below
* Understanding the difference between Workfront licenses and Workfront DAM role types
* -->
