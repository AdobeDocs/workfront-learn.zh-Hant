---
title: 有關請求佇列的常見問題解答
description: 取得有關中請求佇列的常見問題解答 [!DNL  Workfront].
feature: Work Management
type: Tutorial
role: Admin, User
level: Beginner
last-substantial-update: 2023-07-18T00:00:00Z
jira: KT-10101
exl-id: bfa3ae5f-9618-444c-9eb8-5d82db9a77c7
source-git-commit: ec82cd0aafb89df7b3c46eb716faf3a25cd438a2
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# 有關請求佇列的常見問題解答

**為什麼我可以看到請求佇列，但我的使用者卻看不到？**

在 [!UICONTROL 佇列詳細資訊] 索引標籤中，確定您的使用者符合「誰可以新增請求至此佇列？」的標準。 欄位。

**我為使用者提供佇列的存取權，但現在他們也可以檢視請求佇列專案。 為什麼?**

這與您授予他們請求佇列存取權的方式有關。

如果您使用 [!UICONTROL 共用] 工具從「請求佇列」專案登入頁面，則您已授予這些使用者在專案清單中檢視專案的存取權。

但是，如果您只想授予他們提交請求至佇列的存取權，請前往佇列設定，並在「誰可以新增請求至此專案」底下選取適當的選項。

**我可以將請求轉換為專案嗎？**

是. 您可以視需要將問題轉換為任務或專案。

如需詳細資訊，請參閱本文： [轉換問題](https://experienceleague.adobe.com/docs/workfront/using/manage-work/issues/convert-issues/convert-issues-overview.html?lang=en).

**我可以在哪裡找到要編輯的請求佇列？**

您可以使用 [!UICONTROL 搜尋] 欄位，或尋找列在 [!UICONTROL 專案] 區域。

如果您從請求佇列中開啟請求，可以按一下階層連結區域中的專案名稱。

**可以將資訊從請求自訂表單傳輸到專案自訂表單嗎？**

是. 建立自訂表單時，請選取兩者 [!UICONTROL 專案] 和 [!UICONTROL 問題] 作為物件型別。 將自訂表單附加至請求。 將請求轉換為專案時，自訂表單將自動附加到新專案，並且任何欄位中包含的值將顯示在請求和專案自訂表單中。

**我正在檢視專案或任務報告。 我如何找出此物件源自哪個請求？**

您可以存取以下欄位： **[!UICONTROL 轉換的問題]** 和 **[!UICONTROL 轉換的問題建立者]** 欄位來源，將該資訊新增至您的專案與任務報表。

**篩選報表中請求佇列的最佳方式為何？**

如果您的專案篩選器包括 **佇列>>是公用>>等於>>無** 您的報告只會顯示符合以下條件的專案： **NOT** 請求佇列。

如果您的專案篩選器包括 **佇列>>是公用>>不等於>>無** 您的報告將僅顯示滿足以下條件的專案： **為** 請求佇列。
