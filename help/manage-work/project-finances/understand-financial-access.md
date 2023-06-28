---
title: 瞭解財務存取權
description: 瞭解財務存取權如何讓管理員控制誰可以檢視和編輯Workfront中追蹤的財務資訊。
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-financial-access.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10067
exl-id: 1c3d724a-8ff0-466f-9416-cff3da59c8ea
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 5%

---

# 瞭解財務存取權

如果貴組織要透過擷取任何財務資料 [!DNL Workfront]，作為系統管理員，您有責任保護和管理誰有權檢視及編輯該資訊。

若要讓使用者檢視或編輯財務資訊，必須執行下列兩個動作：

1. 存取許可權必須在 [!UICONTROL 存取層級].
2. 必須依物件授予物件使用這些存取許可權的許可權。

例如，使用者可能有權在其存取層級中檢視財務資料，但他們只能檢視與其共用的任務的財務資料，並且該任務共用中啟用了財務檢視。

因此，使用者可能使用 [!UICONTROL 存取層級] 視這些物件的個別共用選項而定，可檢視財務資料以檢視某些物件的財務資料，而非其他物件的財務資料。 但是，除非使用者在下列專案中擁有許可權，否則他們無法檢視任何物件的財務： [!UICONTROL 存取層級].

## [!UICONTROL 存取層級] 設定

財務資料的整體存取權首先由 [!DNL Workfront] 授權型別。

**[!UICONTROL 計畫] 授權可以：**

* 管理付費記錄
* 管理和檢視角色帳單和成本費率
* 管理和檢視使用者帳單和成本費率
* 管理費用
* 檢視和編輯財務

**[!UICONTROL 工作] 授權可以：**

* 管理費用
* 檢視財務

**[!UICONTROL 檢閱] 授權可以：**

* 檢視財務

**許可權可由以下修改 [!UICONTROL 存取層級]. 財務資料存取的三個選項為：**

* [!UICONTROL 無存取權]  — 使用者將無法檢視財務資訊。
* [!UICONTROL 檢視]  — 使用者可以檢閱和共用資訊。
* [!UICONTROL 編輯]  — 使用者可以建立、編輯、刪除和共用資訊。 （僅適用於Plan授權。）

![顯示存取層級中一般財務資料選項的影像](assets/setting-up-finances-8.png)

請務必注意 [!UICONTROL 檢視] 和 [!UICONTROL 編輯] 選項有其他設定 [!UICONTROL 計畫] 授權。 按一下 [!UICONTROL 檢視] 這些選項的按鈕：

**[!UICONTROL 檢視]**

* 檢視角色帳單與成本費率
* 檢視使用者帳單與成本費率

![顯示存取層級中財務資料檢視選項的影像](assets/setting-up-finances-9.png)

**[!UICONTROL 編輯]**

這兩個選項可在 [!UICONTROL 編輯] 選項，以及：

* 編輯角色帳單與成本費率
* 編輯使用者帳單與成本費率

![顯示存取層級中財務資料編輯選項的影像](assets/setting-up-finances-10.png)

>[!NOTE]
>
>有權新增費用的使用者也可以檢視他們新增的費用，以及他們的直接報告新增的費用。
