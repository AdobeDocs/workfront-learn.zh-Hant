---
title: 瞭解如何在中管理資產 [!UICONTROL WORKFRONT DAM]
description: 瞭解如何在中管理資產 [!UICONTROL WORKFRONT DAM] 以改善工作流程。
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8996
exl-id: a09d0b0e-2631-414e-87e6-385ddbeb5cd2
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# 投稿人：資產管理

在本影片中，您將瞭解如何：

* 使用資產上的「編輯」功能表
* 設定到期日
* 檢視通知
* 建立個別通知設定
* 上傳資產版本
* 建立新資料夾
* 將中繼資料範本套用至資料夾
* 建立檔案夾許可權

>[!VIDEO](https://video.tv.adobe.com/v/335256/?quality=12&learn=on)

## 資產版本的運作方式

工作流程的一部分可能包括管理資產的多個版本（或倒圓角、校樣、反複專案，無論您將其命名為）。 您可以透過以下方式管理所有版本 [!UICONTROL WORKFRONT DAM].

當一個與現有檔案同名的檔案上傳到同一個資料夾時，系統允許自動進行資產版本控制。 請洽詢您的系統管理員，檢視此功能是否已開啟。

如果開啟自動版本控制，則只有當資產載入到儲存原始資產的資料夾中時，才會進行版本設定。 兩個資產的檔案名稱必須相同。 如果資產載入到不同的資料夾，資產會以新檔案的形式進入。
如果未開啟版本控制，則無論檔案放在哪個資料夾中，與現有檔案同名的檔案都會上傳為新檔案。 這可能會導致同一資料夾中有兩個同名資產。

您也可以手動上傳特定資產的版本。 按一下資產上的編輯圖示，然後選取 **[!UICONTROL 上傳新版本]**.

如果您將具有版本的資產發佈至Brand Connect，Brand Connect使用者只會看到資產的最新版本。

## 資料夾和資產狀態與有效期

狀態是另一種管理資料夾和資產存取許可權的方式。 [!UICONTROL WORKFRONT DAM]. 狀態可用來隱藏特定資產或資料夾，使其不顯示 [!UICONTROL Brand Connect] 將資產或資料夾設為使用者或過期，只有系統管理員才能存取。

* **[!UICONTROL 作用中]** — 用於資產和資料夾。 資產和資料夾具有 [!UICONTROL 作用中] 所有具有許可權的使用者皆可看到狀態，且狀態可發佈至 [!UICONTROL Brand Connect]. [!UICONTROL 作用中] 以綠色圓點標示在資產或資料夾上。
* **[!UICONTROL 非使用中]** — 用於資產和資料夾。 資產和資料夾具有 [!UICONTROL 非使用中] 狀態可見於 [!UICONTROL WORKFRONT DAM] 使用者，但未顯示在 [!UICONTROL Brand Connect]. [!UICONTROL 非使用中] 以紅色圓點標示在資產或資料夾上。
* **[!UICONTROL 未過期]** — 僅用於資產。 這是所有資產的預設狀態。 未過期的資產，也 [!UICONTROL 作用中] 在中可見 [!UICONTROL Brand Connect].
* **[!UICONTROL 已過期]** — 僅用於資產。 具有的資產 [!UICONTROL 已過期] 除系統管理員外，任何使用者都無法下載狀態。 過期的資產可見/不可見 [!UICONTROL Brand Connect]，視系統設定而定。
