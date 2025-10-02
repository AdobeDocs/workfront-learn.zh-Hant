---
title: 以貢獻者身分瞭解資產管理
description: 瞭解如何在 [!UICONTROL Workfront DAM] 中管理資產以改善工作流程。
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8996
exl-id: a09d0b0e-2631-414e-87e6-385ddbeb5cd2
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 100%

---

# 以貢獻者身分瞭解資產管理

觀看這段影片，您將瞭解如何：

* 使用資產的「編輯」選單
* 設定過期日
* 檢視通知
* 建立個人通知設定
* 上傳資產版本
* 建立新資料夾
* 套用中繼資料範本至資料夾
* 建立資料夾權限

>[!VIDEO](https://video.tv.adobe.com/v/335256/?quality=12&learn=on&enablevpops=1)

## 資產版本如何運作

您的工作流程可能包括管理資料的多個版本，或是回合、校訂、疊代，無論您使用哪種名稱。您可以透過 [!UICONTROL Workfront DAM] 管理所有版本。

當與現有檔案同名的檔案上傳到同一資料夾時，系統允許進行自動資產版本控制。請諮詢您的系統管理員確認這項功能是否開啟。

如果已開啟自動版本控制，唯有資產載入到保存原始資產的資料夾時，才會進行版本控制。兩個資源必須具有相同的檔名。若是資產載入到不同的資料夾，便會成為新檔案。如果未開啟版本控制，無論檔案放在哪個資料夾，與現有檔案同名的檔案將視為新檔案上傳。這可能造成同一資料夾中出現兩個同名的資產。

您也可以手動上傳特定資產的版本。按一下資產上的編輯圖示，然後選取「**[!UICONTROL 上傳新版本]**」。

如果您將含有多個版本的資產發佈到 Brand Connect，則 Brand Connect 使用者只會看到該資產的最新版本。

## 資料夾和資產狀態與期限

狀態是管理 [!UICONTROL Workfront DAM] 資料夾與資產之存取權的另一種方式。您可以使用狀態來隱藏某些資產或資料夾，避免 [!UICONTROL Brand Connect] 使用者看見，或是讓一個資產或資料夾過期，使得唯有系統管理員才能存取。

* **[!UICONTROL 使用中]** — 用於資產和資料夾。在「[!UICONTROL 使用中]」狀態的資產和資料夾，具有權限的全部使用者皆可看見，而且可以發佈到 [!UICONTROL Brand Connect]。「[!UICONTROL 使用中]」的資產或資料夾會用綠色圓點表示。
* **[!UICONTROL 非使用中]** — 用於資產和資料夾。[!UICONTROL Workfront DAM] 使用者可以看到，但是 [!UICONTROL Brand Connect] 的使用者看不到「[!UICONTROL 非使用中]」狀態的資產和資料夾。「[!UICONTROL 非使用中]」的資產或資料夾會用紅色圓點表示。
* **[!UICONTROL 未過期]** — 僅用於資產。這是所有資產的預設狀態。同時具有「[!UICONTROL 使用中]」狀態的未過期資產，也可以在 [!UICONTROL Brand Connect] 中看到。
* **[!UICONTROL 已過期]** — 僅用於資產。除了系統管理員以外，任何使用者皆無法下載具有「[!UICONTROL 已過期]」狀態的資產。已過期的資產在 [!UICONTROL Brand Connect] 中可見/不可見，取決於系統設定。
