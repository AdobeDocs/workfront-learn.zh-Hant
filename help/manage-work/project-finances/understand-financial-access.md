---
title: 了解財務訪問
description: 金融存取權限可讓管理員控制哪些人可以查看及編輯Workfront中追蹤的金融資訊。
feature: Work Management
thumbnail: understand-financial-access.png
type: Tutorial
role: User
level: Intermediate
kt: 10067
exl-id: 1c3d724a-8ff0-466f-9416-cff3da59c8ea
source-git-commit: d0c842ad8bf6f52161f003a62237fbcd35d23176
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 5%

---

# 了解財務訪問

如果貴組織要擷取任何財務資料， [!DNL Workfront]，身為系統管理員，您有責任保護及管理誰有權檢視及編輯該資訊。

用戶要查看或編輯財務資訊需要兩項操作：

1. 必須在 [!UICONTROL 存取層級].
2. 必須逐個對象授予使用這些訪問權限的權限。

例如，用戶有權在其訪問級別查看財務資料，但他們只能查看與他們共用的任務上的財務資料，並且在共用該任務時啟用了財務查看。

因此，使用 [!UICONTROL 存取層級] 根據這些對象的個別共用選項查看某些對象而不是其他對象的財務資訊的權限。 但是，除非用戶在任何對象中都有權查看其財務資訊，否則任何用戶都不能查看這些對象 [!UICONTROL 存取層級].

## [!UICONTROL 存取層級] 設定

首先授予對金融資料的整體存取權 [!DNL Workfront] 授權類型。

**[!UICONTROL 計畫] 許可證可以：**

* 管理計費記錄
* 管理並查看職責開單和成本費率
* 管理和查看用戶開單和成本費率
* 管理費用
* 查看和編輯財務

**[!UICONTROL 工作] 許可證可以：**

* 管理費用
* 查看財務

**[!UICONTROL 檢閱] 許可證可以：**

* 查看財務

**權限可由 [!UICONTROL 存取層級]. 金融資料存取的三個選項是：**

* [!UICONTROL 無權存取]  — 用戶將看不到財務資訊。
* [!UICONTROL 檢視]  — 用戶可以查看和共用資訊。
* [!UICONTROL 編輯]  — 用戶可以建立、編輯、刪除和共用資訊。 （僅適用於計畫許可證。）

![在訪問級別顯示一般財務資料選項的影像](assets/setting-up-finances-8.png)

請務必注意， [!UICONTROL 檢視] 和 [!UICONTROL 編輯] 選項有 [!UICONTROL 計畫] 授權。 按一下 [!UICONTROL 檢視] 按鈕（下）:

**[!UICONTROL 檢視]**

* 檢視角色帳單與成本費率
* 檢視使用者帳單與成本費率

![在訪問級別顯示「財務資料」視圖選項的影像](assets/setting-up-finances-9.png)

**[!UICONTROL 編輯]**

這兩個選項可在 [!UICONTROL 編輯] 選項，以及：

* 編輯角色帳單與成本費率
* 編輯使用者帳單與成本費率

![在訪問級別顯示「財務資料」編輯選項的影像](assets/setting-up-finances-10.png)

>[!NOTE]
>
>有權添加費用的用戶還可以查看他們添加的費用，以及直接報告添加的費用。
