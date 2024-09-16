---
title: 請求佇列常見問題的解答
description: 針對  [!DNL  Workfront] 中請求佇列的常見問題獲得解答。
feature: Work Management
type: Tutorial
role: Admin, User
level: Beginner
last-substantial-update: 2024-09-16T00:00:00Z
recommendations: noDisplay,noCatalog
jira: KT-10101
exl-id: bfa3ae5f-9618-444c-9eb8-5d82db9a77c7
source-git-commit: e9a4f2bcd39e2598ff540bb4f300e891e817e939
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 50%

---

# 請求佇列常見問題的解答

**為什麼我可以看到請求佇列，但我的使用者看不到？**

在您的請求佇列/專案的「[!UICONTROL 佇列詳細資料]」標籤中，確認您的使用者符合「誰可以對此佇列新增請求」欄位的條件。

請觀看這段影片，瞭解更多詳細資訊：

>[!VIDEO](https://video.tv.adobe.com/v/3434156/?quality=12&learn=on)

**我授予使用者存取佇列的權限，但現在他們也可以看見請求佇列專案。為什麼？**

在「誰可以新增要求至此佇列？」 清單中，如果您選擇「擁有此專案檢視存取許可權的人員」，則任何您授予檢視許可權以使用請求佇列的人，也能夠檢視專案清單中的請求佇列。 若要避免此問題，請使用「此專案公司的人員」或「此專案群組的人員」選項。

**我可以將請求轉換成專案嗎？**

是。您可以根據需要將問題轉換成任務或專案。

這些教學課程會示範如何：

* [將問題/請求轉換為專案](/help/manage-work/issues-requests/create-a-project-from-a-request.md)

* [將問題/請求轉換為任務](/help/manage-work/issues-requests/convert-issues-to-other-work-items.md)

**在哪裡可以找到進行編輯的請求佇列？**

您可以使用導覽列的「[!UICONTROL 搜尋]」欄位或是瀏覽「[!UICONTROL 專案]」區域的清單。

如果您從請求佇列中開啟請求，可以按一下階層連結區域中的專案名稱。

**我可以把請求自訂表單中的資訊轉移到專案自訂表單嗎？**

是。在您建立自訂表單時，請同時選取「[!UICONTROL 專案]」和「[!UICONTROL 問題]」作為物件類型。您也可以編輯專案自訂表單，以包含問題物件型別，反之亦然。

將自訂表單附加到請求上。當您將請求轉換成專案時，自訂表單會自動附加到新的專案上，而任何欄位所包含的值將會同時出現在請求和專案自訂表單上。

**我正在查看專案或任務報告。我如何找出這個物件來自哪項請求？**

您可以存取「**[!UICONTROL 已轉換的問題]**」和「**[!UICONTROL 已轉換問題的建立者]**」欄位來源中的欄位，把該資訊新增到專案和任務報告中。

請觀看這段影片，瞭解更多詳細資訊：

>[!VIDEO](https://video.tv.adobe.com/v/3434176/?quality=12&learn=on)


**在報告中篩選請求佇列的最佳方法是什麼？**

若您的專案篩選器包含「**佇列 >> 是公開的 >> 等於 >> 無**」，則您的報告只會顯示「**不是**」請求佇列的專案。

若您的專案篩選器包含「**佇列 >> 是公開的 >> 不等於 >> 無**」，則您的報告只會顯示「**是**」請求佇列的專案。

請觀看這段影片，瞭解更多詳細資訊：

>[!VIDEO](https://video.tv.adobe.com/v/3434329/?quality=12&learn=on)

**建立「要求佇列」的自訂狀態是好辦法嗎？**

有些客戶會建立等同於目前的「請求佇列」自訂狀態。 接著，他們可以執行顯示所有請求佇列的報表，或輕鬆從報表中排除請求佇列。 雖然這比使用&#x200B;**Queue>>Is Public>>Not Equal>>None**&#x200B;更方便使用，但缺點在於建立請求佇列的人可能會忘記使用它，因為「目前」狀態也同樣有效，而且這也是他們將在大部分訓練教材中看到的內容。 因此，許多客戶選擇不使用請求佇列的自訂狀態。

不過，如果您已在組織中使用請求佇列狀態，而您只是想要確定它是否正常使用（或修正未正確使用的情況），您可以建立上方影片中說明的&#x200B;**作用中請求佇列**&#x200B;報告，並變更&#x200B;**專案>>狀態等於與>>等於>>目前**&#x200B;到&#x200B;**專案>>狀態>>等於>>目前**&#x200B;的篩選器。 這將會顯示所有使用目前狀態（而非您想要它們使用的請求佇列狀態）的使用中請求佇列。 選取所有顯示的專案，並大量編輯以變更狀態至「請求佇列」。

## 有關此主題的推薦教學課程

* [瞭解請求佇列](/help/manage-work/request-queues/understand-request-queues.md)
* [建立請求佇列](/help/manage-work/request-queues/create-a-request-queue.md)
* [了解請求流程設定](/help/manage-work/request-queues/understand-settings-for-a-flow-request.md)
* [建立請求流程](/help/manage-work/request-queues/create-a-request-flow.md)
* [建立系統管理員意見回饋請求佇列](/help/manage-work/request-queues/create-a-system-admin-feedback-request-queue.md)
