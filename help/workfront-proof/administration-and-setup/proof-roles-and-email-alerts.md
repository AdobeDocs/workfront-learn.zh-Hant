---
title: 校訂角色與電子郵件警報
description: 瞭解在  [!DNL  Workfront] 中如何啟用正確的校訂角色和電子郵件警報，讓校訂收件者可以存取校訂以及看見所執行工作之情況。
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
ht-degree: 100%

---

# 校訂角色與電子郵件警報

校訂角色與電子郵件警報協助推動校訂工作流程，確保收件者均有適當的校訂存取權，並能看見所執行工作的情況。

我們來回顧一些基本的校訂術語：

* **校訂角色 —** 定義使用者可以對校訂做什麼 (例如註解、標註記號、核准等)。
* **電子郵件警報 —**&#x200B;當校訂上有活動時，會傳送電子郵件給校訂工作流程中的人員。

![影像顯示「[!UICONTROL 新增校訂]」視窗，其中突顯標示「[!UICONTROL 校訂角色]」和「[!UICONTROL 電子郵件警報]」欄。](assets/proof-roles-and-email-alerts.png)

您的校訂系統管理員可以為組織的校訂使用者設定預設的校訂角色和電子郵件警報。此外，這些資訊可以內建到校訂工作流程範本中 (亦稱為自動化工作流程範本)。

但是，有時您可能需要在上傳校訂時手動設定這些資訊。

[!DNL Workfront] 提供指派校訂角色給校訂收件者時的一般建議：

* **檢閱者和核准者 —** 這些使用者可以在校訂上留下註解也可以對校訂做出決定 (例如核准或拒絕)。檢閱過程中主要的內部和外部利害關係人請使用這個校訂角色。
* **檢閱者 —** 您的校訂工作流程中有些人員只需要留下註解，這是適合他們的角色。檢閱者角色也可以指派給主要負責上傳校訂或具有校訂所有者身分，但除此以外並未參與校訂流程的 [!DNL Workfront] 使用者。
* **唯讀 —** 適合只需要檢視校訂的收件者。[!UICONTROL 唯讀]提供檢視權限，但不允許留下註解。

[!DNL Workfront] 提供指派電子郵件警報給校訂收件者時的一般建議：

* **最終決定 —**&#x200B;當最後一個人做出校訂決定時，便會傳送一封電子郵件。把這個角色指派給監視校訂工作流程的人員。可能是校訂管理員、校訂所有者、校訂建立者、專案經理人或其他 [!DNL Workfront] 使用者。[!DNL Workfront] 建議使用基本工作流程時採用此警報，讓監視校訂的人員知道所有決定均已完成。
* **決定 —** 當每個校訂工作流程的利害關係人做出校訂決定時，便會傳送警報。使用自動化工作流程而且有數個決定時，這是非常合適的選項。把這個角色指派給監視校訂工作流程的人員。可能是校訂管理員、校訂所有者、校訂建立者、專案經理人或其他 [!DNL Workfront] 使用者。
* **停用 —** 對訪客校訂使用者請使用這個角色，限制他們收到校訂相關電子郵件的數量。收件者仍會收到關於新增校訂、新版本和校訂延遲的通知，加上 [!DNL Workfront] 使用者收到在校訂註解中使用 @username 傳來的直接訊息，而訪客收件者則是收到使用 @emailaddress 傳來的訊息。

## 換您來操作

1. 登入 Workfront 並建立您之前不曾建立過的將使用校訂的使用者。根據人員在校訂工作流程中扮演的角色，在其使用者設定中設定校訂權限設定檔。
1. 對於已建立的使用者，若有需求，請編輯其設定來調整所選取的校訂權限設定檔。
1. 存取校訂設定區域並前往「使用者」標籤。檢查使用者的個人設定，包括語言、時區、日期格式、預設校訂角色和預設電子郵件警報。若有使用者在全域系統預設值設定之前便已建立，則這項檢查十分重要。

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
