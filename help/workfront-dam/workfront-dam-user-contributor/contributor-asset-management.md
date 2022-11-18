---
title: 了解如何在 [!UICONTROL Workfront DAM]
description: 了解如何在 [!UICONTROL Workfront DAM] 來改善工作流程。
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8996
exl-id: a09d0b0e-2631-414e-87e6-385ddbeb5cd2
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# 貢獻者：資產管理

在此影片中，您將學習如何：

* 使用資產上的「編輯」功能表
* 設定到期日
* 檢視通知
* 建立個別通知設定
* 上傳資產版本
* 建立新資料夾
* 將中繼資料範本套用至資料夾
* 建立資料夾權限

>[!VIDEO](https://video.tv.adobe.com/v/335256/?quality=12)

## 資產版本如何運作

工作流程的一部分可能包括管理資產的多個版本（或四捨五入、校樣、反覆項目，無論您稱之為什麼）。 您可以透過 [!UICONTROL Workfront DAM].

系統可在與現有檔案同名的檔案上傳至相同資料夾時，自動控制資產版本。 請向系統管理員確認此功能是否已開啟。

如果開啟自動版本控制，只有當資產載入至保存原始資產的資料夾時，資產才會進行版本。 兩個資產的檔案名稱必須相同。 如果資產載入至不同的資料夾，資產會以新檔案形式傳入。
如果未開啟版本控制，則與現有檔案同名的檔案將作為新檔案上傳，而不管其放入哪個資料夾。 這可能會導致相同資料夾中有兩個名稱相同的資產。

您也可以手動上傳特定資產的版本。 按一下資產上的編輯圖示，然後選取 **[!UICONTROL 上傳新版本]**.

如果您將資產的版本發佈至Brand Connect,Brand Connect使用者只會看見資產的最新版本。

## 資料夾和資產狀態和到期日

狀態是管理資料夾和資產存取權限的另一種方式 [!UICONTROL Workfront DAM]. 狀態可用來隱藏特定資產或資料夾，以防止 [!UICONTROL Brand Connect] 使用者或將資產或資料夾過期，讓除系統管理員以外的任何人都無法存取。

* **[!UICONTROL 作用中]** — 用於資產和資料夾。 具有 [!UICONTROL 作用中] 所有具有權限的使用者皆可看到狀態，並可發佈至 [!UICONTROL Brand Connect]. [!UICONTROL 作用中] 在資產或資料夾上以綠色圓點表示。
* **[!UICONTROL 非作用中]** — 用於資產和資料夾。 具有 [!UICONTROL 非作用中] 狀態顯示為 [!UICONTROL Workfront DAM] 但在 [!UICONTROL Brand Connect]. [!UICONTROL 非作用中] 在資產或資料夾上以紅點表示。
* **[!UICONTROL 未到期]** — 僅用於資產。 這是所有資產的預設狀態。 未到期資產亦包括 [!UICONTROL 作用中] 在 [!UICONTROL Brand Connect].
* **[!UICONTROL 過期]** — 僅用於資產。 具有 [!UICONTROL 過期] 除系統管理員外，任何用戶都無法下載狀態。 過期的資產會顯示/不顯示在 [!UICONTROL Brand Connect]，具體取決於系統配置。
