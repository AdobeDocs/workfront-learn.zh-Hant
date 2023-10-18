---
title: 設定群組和使用者
description: 瞭解如何在中建立資料夾、群組和使用者 [!UICONTROL WORKFRONT DAM]. 瞭解使用者角色型別並授予檔案夾許可權。
activity: use
feature: Digital Content and Documents
type: Tutorial
role: Admin
level: Intermediate
team: Technical Marketing
jira: KT-8967
exl-id: 4ebf675c-b72d-447e-b131-a89acb449e15
doc-type: video
source-git-commit: 6c31f8d2e98ad8cd1880cd03ec0b0e6c0fd9ec09
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# 設定群組和使用者

在本影片中，您將瞭解如何：

* 瞭解群組設定如何影響對資產的存取
* 以特定順序建立資料夾、群組和使用者
* 瞭解使用者角色型別
* 授予檔案夾的許可權
* 建立和編輯群組
* 新增和編輯使用者

>[!VIDEO](https://video.tv.adobe.com/v/335230/?quality=12&learn=on)

## 群組和使用者檢閱

當您設定 [!UICONTROL WORKFRONT DAM] 系統，考量使用者和群組在大局中扮演的角色很重要。

群組控制對資產資料夾的存取 [!UICONTROL WORKFRONT DAM]. 群組設定也可控制使用者可以對資產執行的動作（檢視、下載、編輯等） 他們具有存取許可權。

建立群組時，請務必牢記該群組的成員需要在哪些資產資料夾中存取 [!UICONTROL WORKFRONT DAM].

使用者是已登入的個人 [!UICONTROL WORKFRONT DAM]. 使用者無法存取中的任何內容 [!UICONTROL WORKFRONT DAM] 除非已指派給群組。 使用者可以根據自己的需求，屬於多個群組。

## 預設群組

隨附有兩個預設群組 [!UICONTROL WORKFRONT DAM]. 所有使用者都會根據是否具備下列條件，自動屬於這些群組 [!UICONTROL WORKFRONT DAM] 登入認證。 您無法從這些群組新增或移除使用者：

* **來賓群組** — 用來控制匿名使用者的存取權。 可能是沒有登入憑證的人或目前未登入的使用者。
* **已記錄**-In group — 所有登入的使用者都屬於此群組。

依預設，管理員群組及其設定也存在。 您可以將使用者新增至此群組，但無法調整設定。

## 角色型別

建立群組時，會為其指派角色型別。 角色型別決定了 [!UICONTROL WORKFRONT DAM] 系統使用者登入時取得 —  [!UICONTROL WORKFRONT DAM] 本身或 [!UICONTROL Brand Connect].

可用的角色型別有三種 [!UICONTROL WORKFRONT DAM] 授權：

* **[!UICONTROL Brand Portal]** — 這些使用者只能存取 [!UICONTROL Brand Connect]，使用者可在此檢視及下載已核准的資產。
* **[!UICONTROL 投稿人]** — 這些使用者可以存取 [!UICONTROL WORKFRONT DAM] 和 [!UICONTROL Brand Connect]. 使用者擁有資產和資料夾的完整存取權，包括檢視、下載、上傳、編輯、移動和刪除。
* **[!UICONTROL 管理員]** — 系統管理員可以存取中的所有專案 [!UICONTROL Brand Connect] 和 [!UICONTROL WORKFRONT DAM]，並可建立每個的全域系統設定。 他們也可以存取已過期或已設定為非使用中的資產。

<!-- 
Learn more graphic & documentation article link, below
* Understanding the difference between Workfront licenses and Workfront DAM role types
* -->
