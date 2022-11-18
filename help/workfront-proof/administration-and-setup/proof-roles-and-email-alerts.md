---
title: 校樣角色和電子郵件警報
description: 了解如何啟用適當的校樣角色和電子郵件警報，讓校樣收件者能存取校樣，並洞察正在進行的工作 [!DNL  Workfront].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: proof-roles-and-email-alerts.png
kt: 10177
exl-id: 15bfb18a-5392-4a91-a6a2-223f7ac30dc5
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 0%

---

# 校樣角色和電子郵件警報

校樣角色和電子郵件警報有助於推動校樣工作流程，確保收件者有權存取校樣，並能夠洞察所完成的工作。

讓我們回顧一下一些基本的證明術語：

* **證明角色 —** 定義使用者可以對校樣執行的動作（例如注釋、標籤、核准等）。
* **電子郵件警報 —** 當校樣上有活動時，會在校樣工作流程中傳送電子郵件給人員。

![的影像 [!UICONTROL 新校樣] 窗口 [!UICONTROL 證明角色] 和 [!UICONTROL 電子郵件警報] 欄。](assets/proof-roles-and-email-alerts.png)

您的校樣系統管理員可以為貴組織的校樣使用者設定預設校樣角色和電子郵件警報。 此外，此資訊可內建在校樣工作流程範本中（也稱為自動化工作流程範本）。

不過，有時候您在上傳校樣時可能需要手動設定此資訊。

[!DNL Workfront] 為校樣收件者指派校樣角色時，會提供下列一般建議：

* **審核者與核准者 —** 這些使用者可以對校樣發表評論，並對校樣做出決策（例如核准或拒絕）。 在審核流程中，將此證明角色用於關鍵內部和外部利益相關方。
* **審閱者 —** 您的校樣工作流程中，有些人只需要發表意見，此角色最適合他們。 審核者角色也可指派給 [!DNL Workfront] 主要上傳校樣或作為校樣擁有者，但不屬於校樣程式的使用者。
* **只讀 —** 非常適合只需要查看校樣的收件者。 [!UICONTROL 唯讀] 提供檢視存取權，不允許留言。

[!DNL Workfront] 在將電子郵件警報指派給校樣收件者時，提供下列一般建議：

* **最終決定 —** 當最後一個人決定校樣時，這會傳送電子郵件。 將此項目指派給監控校樣工作流程的人員。 這可以是校樣管理員、校樣擁有者、校樣建立者、專案管理員或其他 [!DNL Workfront] 使用者。 [!DNL Workfront] 在使用基本工作流程時建議使用此警報，以便監控校樣的人員知道已做出所有決策。
* **決策 —** 這會在每個校對工作流程利害關係人決定校樣時傳送警報。 使用自動化工作流程並執行數個決策時，此選項最合適。 指派給監控校樣工作流程的人員。 這可以是校樣管理員、校樣擁有者、校樣建立者、專案管理員或其他 [!DNL Workfront] 使用者。
* **禁用 —** 將此功能用於來賓校樣使用者，以限制他們收到有關校樣的電子郵件數量。 收件者仍會收到新校樣、新版本和延遲校樣的通知，以及 [!DNL Workfront] 使用者會使用校樣註解和訪客收件者(@username)，接收校樣註解中的直接@emailaddress訊。

## 該你了

1. 登入Workfront，並建立將使用您先前未建立之校對的使用者。 根據人員將在校樣工作流程中扮演的角色，在其使用者設定中設定校樣權限設定檔。
1. 對於已建立的使用者，視需要編輯其設定以調整和校樣權限設定檔選取項目。
1. 訪問校對設定區域，然後轉到「用戶」頁簽。 檢查用戶的個人設定 — 語言、時區、日期格式、預設校樣角色和預設電子郵件警報。 如果這些用戶是在建立全局系統預設值之前建立的（這些設定在此學習路徑的第1節中討論），則這一點很重要。

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
