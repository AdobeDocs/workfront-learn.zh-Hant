---
title: 何時以及如何停用或刪除使用者
description: 瞭解停用和刪除使用者之間的差異。 然後根據貴組織的需求管理使用者設定檔。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner
thumbnail: 10037.jpeg
jira: KT-10037
exl-id: 89b7d083-97d3-4783-a61d-35226d6582c0
TQID: https://experienceleague.adobe.com/bOJ2ng-HrOD5SA9-uAItNK1rFF90zSnuxjeSiyh9LXk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 281
ht-degree: 87%

---

# 何時以及如何停用或刪除使用者

當使用者離開組織或不再使用 [!DNL Workfront]，您想要停用其登入憑證。 唯有特定情況下才能刪除使用者設定檔。

## 停用

停用使用者會移除使用者設定檔中的授權，他們便無法再登入或存取 [!DNL Workfront]。 他們的授權便可以指派給另一位使用者。

停用的使用者無法獲得指派新工作，但是他們仍然有現有的工作指派。

例如，自由工作者已經完成特定專案的工作，所以您要停用其登入權限，直到下次需要再度合作為止。

## 刪除

在極少數情況下 (例如意外進入或測試使用者)，可能需要刪除 [!DNL Workfront] 中的使用者登入憑證。 刪除使用者會把使用者與 [!DNL Workfront] 中各項目的關聯也一起刪除，包括工作指派、備註、時數、文件、所建立的物件等。

[!DNL Workfront] 建議刪除使用者的&#x200B;**唯一**&#x200B;情況，是使用者如果不曾被指派任何工作，或從無任何 Workfront 項目的歷史記錄的時候。

[!DNL Workfront] **強烈**&#x200B;建議停用使用者而非刪除使用者。 停用會保留[!DNL Workfront]中的使用者資訊，這些資訊可能是精確報告、專案管理等所需。若您有關於是否應該停用或刪除使用者的疑問，請洽詢您的[!DNL Workfront]顧問或[!DNL Workfront]客戶支援。

![[!DNL Users]頁面上「更多」選單顯示選項](assets/admin-fund-adding-users-11.png)

### 停用或刪除使用者

1. 在[!UICONTROL 主選單]中選取「**[!UICONTROL 使用者]**」。
1. 勾選使用者名稱旁邊的方塊即可選取使用者。
1. 按一下「**[!UICONTROL 更多]**」下拉式選單。
1. 選取「**[!UICONTROL 停用]**」或「**[!UICONTROL 刪除]**」。
