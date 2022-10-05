---
title: 中的群組和使用者 [!UICONTROL Workfront DAM]
description: 了解如何在中建立資料夾、群組和使用者 [!UICONTROL Workfront DAM]. 了解使用者角色類型，並授予資料夾權限。
activity: use
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
team: Technical Marketing
kt: 8967
exl-id: 4ebf675c-b72d-447e-b131-a89acb449e15
source-git-commit: a0aa8328842d2db1235edc42664eb0b18f4038e4
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# 系統設定：群組和使用者

在此影片中，您將學習如何：

* 了解群組設定如何影響資產的存取權
* 以特定順序建立資料夾、群組和使用者
* 了解使用者角色類型
* 將權限授予資料夾
* 建立和編輯群組
* 新增和編輯使用者

>[!VIDEO](https://video.tv.adobe.com/v/335230/?quality=12)

## 群組和使用者檢閱

當您設定 [!UICONTROL Workfront DAM] 系統中，必須從全局角度考慮用戶和組的角色。

群組可控制中資產資料夾的存取權 [!UICONTROL Workfront DAM]. 群組設定也可控制使用者可以對資產執行的動作（檢視、下載、編輯等） 他們有權存取。

建立群組時，請務必記住群組成員需要存取的資產資料夾 [!UICONTROL Workfront DAM].

使用者是指已登入 [!UICONTROL Workfront DAM]. 使用者無法存取 [!UICONTROL Workfront DAM] 除非它們被指派給群組。 使用者可以屬於多個群組，視其需求而定。

## 預設群組

有兩個預設群組隨附 [!UICONTROL Workfront DAM]. 所有使用者都會根據是否已自動加入這些群組 [!UICONTROL Workfront DAM] 登入憑證。 您無法從以下群組新增或移除使用者：

* **來賓組** — 用於控制匿名用戶的訪問。 可能是沒有登入憑證的使用者，或目前未登入的使用者。
* **已記錄**-In組 — 登錄的所有用戶都屬於此組。

預設也存在管理員群組及其設定。 您可以新增使用者至此群組，但無法調整設定。

## 角色類型

建立群組時，會為群組指派角色類型。 角色類型決定 [!UICONTROL Workfront DAM] 系統用戶登錄時獲得的 —  [!UICONTROL Workfront DAM] 本身或 [!UICONTROL Brand Connect].

有三種可用的角色類型 [!UICONTROL Workfront DAM] 許可證：

* **[!UICONTROL Brand Portal]** — 這些使用者只能存取 [!UICONTROL Brand Connect]，供使用者檢視及下載已核准資產。
* **[!UICONTROL 貢獻者]** — 這些用戶可以訪問 [!UICONTROL Workfront DAM] 和 [!UICONTROL Brand Connect]. 他們擁有資產和資料夾的完整存取權限，包括檢視、下載、上傳、編輯、移動和刪除。
* **[!UICONTROL 管理員]** — 系統管理員可存取 [!UICONTROL Brand Connect] 和 [!UICONTROL Workfront DAM]，以及為每個設定全域系統設定的功能。 他們也可以存取已過期或設定為非使用中的資產。

<!-- 
Learn more graphic & documentation article link, below
* Understanding the difference between Workfront licenses and Workfront DAM role types
* -->
