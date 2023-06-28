---
title: 校訂角色和電子郵件警示
description: 瞭解如何啟用適當的校樣角色和電子郵件提醒，以便校樣收件者能夠存取校樣並檢視中進行的工作 [!DNL  Workfront].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: proof-roles-and-email-alerts.png
jira: KT-10177
exl-id: 15bfb18a-5392-4a91-a6a2-223f7ac30dc5
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# 校訂角色和電子郵件警示

校樣角色和電子郵件警報有助於推動校樣工作流程，確保收件者有權存取校樣並檢視正在進行的工作。

讓我們來檢視一些基本的校訂術語：

* **校訂角色 —** 定義使用者可對校樣執行的操作（例如評論、標籤、核准等）。
* **電子郵件警示 —** 當校訂上有活動時，傳送給校訂工作流程中人員的電子郵件。

![的影像 [!UICONTROL 新校訂] 視窗的 [!UICONTROL 校訂角色] 和 [!UICONTROL 電子郵件警示] 欄反白顯示。](assets/proof-roles-and-email-alerts.png)

您的校訂系統管理員可以為貴組織的校訂使用者設定預設校訂角色和電子郵件提醒。 此外，此資訊可內建在校訂工作流程範本（也稱為自動化工作流程範本）中。

不過，上傳校樣時有時需要手動設定此資訊。

[!DNL Workfront] 為校訂收件者指派校訂角色時，提供以下一般建議：

* **檢閱者和核准者 —** 這些使用者既可以對校訂進行評論，也可以對校訂進行決定（例如核准或拒絕）。 在稽核過程中將此校樣角色用於關鍵的內部和外部利益相關者。
* **檢閱者 —** 校訂工作流程中的某些人員只需要發表評論，此角色非常適合他們。 也可以將稽核者角色指派給 [!DNL Workfront] 主要上傳校樣或作為校樣擁有者，但其他方面不屬於校樣流程的使用者。
* **唯讀 —** 適用於只需要檢視證明的收件者。 [!UICONTROL 唯讀] 會提供檢視存取權，不允許評論。

[!DNL Workfront] 為校樣收件者指派電子郵件警報時，提供下列一般建議：

* **最終決定 —** 這會在最後一個人對校樣做出決定時傳送電子郵件。 將此指派給監控校樣工作流程的人員。 這可以是校訂管理員、校訂所有者、校訂建立者、專案管理員或其他 [!DNL Workfront] 使用者。 [!DNL Workfront] 建議使用基本工作流程時發出此警報，讓監控校訂的人員知道已做出所有決定。
* **決策 —** 這會在每個校訂工作流程利害關係人對校訂做出決定時傳送警報。 此選項最適合使用包含數個決策的自動化工作流程。 指派給監控校樣工作流程的人員。 這可以是校訂管理員、校訂所有者、校訂建立者、專案管理員或其他 [!DNL Workfront] 使用者。
* **已停用 —** 對訪客校訂使用者使用此項來限制他們收到的有關校訂的電子郵件數量。 收件者仍會收到有關新校訂、新版本和最新校訂的通知，此外 [!DNL Workfront] 使用者會收到校樣評論中透過@emailaddress使用@username和訪客收件者的直接訊息。

## 輪到你了

1. 登入Workfront並建立將使用您先前未建立之校訂的使用者。 根據此人在校訂工作流程中將扮演的角色，在其使用者設定中設定校訂許可權設定檔。
1. 如有需要，請針對已建立的使用者編輯其設定以調整校樣許可權設定檔選擇。
1. 存取校樣設定區域，然後前往「使用者」標籤。 檢查使用者的個人設定 — 語言、時區、日期格式、預設校樣角色和預設電子郵件警報。 如果這些使用者是在建立全域系統預設值之前建立的，這一點很重要。

<!--
Download the proof role and email alert guides to have on hand as you start uploading proofs and assigning proof recipients.
-->

<!--
## Learn more
* Notifications for proof comments and decisions
-->

<!--
## Guides
* Proof roles
* Email alerts
-->
