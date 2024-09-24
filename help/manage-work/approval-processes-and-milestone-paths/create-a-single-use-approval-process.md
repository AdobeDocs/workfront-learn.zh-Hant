---
title: 建立全域和單一使用核准流程
description: 了解如何在 Workfront 中針對專案、任務或問題建立單次的核准流程。
activity: use
feature: Approvals
thumbnail: 335225.jpeg
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-8962
last-substantial-update: 2024-09-24T00:00:00Z
recommendations: noDisplay,noCatalog
exl-id: 85d28b54-72a6-4dd1-bac8-8e7ffb3e2b76
doc-type: video
source-git-commit: b0114985964736fb7bb234c581cb56930714915c
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 42%

---

# 建立全域和單一使用核准流程

專案、任務和問題的核准流程使專案經理人能夠在繼續下一步之前，獲得專家確認工作已完成。專案經理可以針對每種情況建立核准流程（這稱為單次使用核准流程），或從清單中選擇之前為滿足一般需求而建立的可能許多核准流程（這些流程稱為全域或現有核准流程）。

在任一情況下，當物件狀態變更為核准流程中指定的狀態時，核准者都會以各種方式收到通知，以便檢閱工作並予以核准或拒絕。由於整個專案可能會因為等待核准而暫停，核准者應提前意識到可能輪到他們負責核准。如果核准者因任何原因不在辦公室，他們可以將核准工作委派給符合資格的替補人員。如需詳細資訊請參閱「[委派任務、問題和核准](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)」。

在本影片中，您將會瞭解如何針對專案、任務或問題建立全域核准流程和單一使用核准流程。

>[!VIDEO](https://video.tv.adobe.com/v/335225/?quality=12&learn=on)

>[!TIP]
>
>您可以將專案或任務的單次核准流程新增至專案範本。

>[!NOTE]
>
>您可以按照影片中針對任務所述的相同方式設定專案和問題的單次核准流程。

## 如何在請求佇列中套用自動問題核准

如果您想要在請求佇列中設定自動問題核准，這些只能使用全域問題核准流程完成，並套用到[!UICONTROL 佇列主題]。

在建立或編輯[!UICONTROL 佇列主題]時，請在&#x200B;**[!UICONTROL 預設核准]**&#x200B;欄位中選取全域核准程式。

![顯示如何在佇列主題](assets/automatic-issue-approval-1.png)中選取預設核准流程的影像

您可能需要編輯問題核准程式，以確保&#x200B;**[!UICONTROL 先前的狀態]**&#x200B;不是核准被拒絕時問題設定的狀態。 這是因為先前狀態為&#x200B;**[!UICONTROL 新]**，而且此狀態也會觸發核准程式，因此是在核準時將設定的狀態。 為了避免問題核准遭到拒絕時產生混淆，最好將狀態設定為&#x200B;**[!UICONTROL 無法解決]**&#x200B;之類的專案，或為此目的建立的自訂狀態。

![影像顯示變更問題拒絕時要使用的狀態](assets/automatic-issue-approval-2.png)


## 有關此主題的推薦教學課程

* [委派任務、問題與核准](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [附加和編輯現有核准流程](/help/manage-work/approval-processes-and-milestone-paths/attach-and-edit-existing-approval-processes.md)
* [瞭解特定群組的核准流程](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [建立請求流程](/help/manage-work/request-queues/create-a-request-flow.md)

