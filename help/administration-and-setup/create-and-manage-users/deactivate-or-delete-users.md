---
title: 何時及如何停用或刪除使用者
description: 瞭解停用和刪除使用者之間的差異。 然後根據您組織的需求管理使用者設定檔。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner
thumbnail: 10037.jpeg
jira: KT-10037
exl-id: 89b7d083-97d3-4783-a61d-35226d6582c0
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# 何時及如何停用或刪除使用者

當使用者離開組織或不再使用 [!DNL Workfront]，您會想要停用其登入資訊。 刪除使用者設定檔應僅在特定情況下完成。

## 停用

停用使用者會將授權從使用者的設定檔中移除，因此他們無法再登入或存取 [!DNL Workfront]. 他們的授權可指派給其他使用者。

無法指派新工作給已停用的使用者，但他們將保留指派給任何現有工作。

例如，自由職業者對於特定專案的工作已完成，因此您想要停用其登入，直到下次需要他們時。

## 刪除

在極少數的情況下（例如意外輸入或測試使用者），使用者登入可能需要從刪除 [!DNL Workfront]. 刪除使用者會刪除該使用者與中專案的關聯 [!DNL Workfront] — 工作指派、附註、時數、檔案、它們建立的物件等。

此 **僅限** 時間 [!DNL Workfront] 如果使用者從未被指派工作，或絕對沒有使用Workfront專案的記錄，建議刪除使用者。

[!DNL Workfront] **強烈** 建議停用使用者而非刪除使用者。 停用會將使用者資訊保留在 [!DNL Workfront]，這可作為精確報告、專案管理等工作之用。 如果您對是否應該停用或刪除使用者有任何疑問，請諮詢您的 [!DNL Workfront] 顧問或 [!DNL Workfront] 客戶支援。

![顯示選項的其他選單 [!DNL Users] 頁面](assets/admin-fund-adding-users-11.png)

### 停用或刪除使用者

1. 選取 **[!UICONTROL 使用者]** 從 [!UICONTROL 主要功能表].
1. 核取使用者名稱旁的方塊以選取使用者。
1. 按一下 **[!UICONTROL 更多]** 下拉式功能表。
1. 選取 **[!UICONTROL 停用]** 或 **[!UICONTROL 刪除]**.
