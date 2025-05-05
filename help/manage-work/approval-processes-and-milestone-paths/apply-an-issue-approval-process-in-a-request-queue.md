---
title: 在請求佇列中套用問題核准流程
description: 實作預設核准流程以簡化請求工作流程，確保已核准的請求會適當地將其狀態變更為「新增」。 選取狀態變更為「無法解決」以解決拒絕請求的混淆。
activity: use
feature: Approvals
thumbnail: 335225.jpeg
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-17578
last-substantial-update: 2025-03-26T00:00:00Z
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: 3fc3a58c829769ca06ffb93971ac75516dfbd5f2
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 6%

---

# 在請求佇列中套用問題核准流程

>[!PREREQUISITES]
>
>* [建立請求流程](https://experienceleague.adobe.com/zh-hant/docs/workfront-learn/tutorials-workfront/manage-work/request-queues/create-a-request-flow)
>* [建立全域和單次使用的核准程式](https://experienceleague.adobe.com/zh-hant/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)


此影片說明建立請求佇列時，套用預設核准程式的程式。&#x200B;URL 建立請求時，其狀態會從「新增 — 未決核准」開始，並傳送核准通知給指定的核准者。&#x200B;URL 如果核准，狀態會變更為「新增」，允許指派的個人開始工作。&#x200B;URL 如果遭拒絕，由於核准流程設定中的常見錯誤，狀態可能會錯誤地恢復為「新」。&#x200B;URL
影片重點說明當狀態設為「新增」（新請求的預設值）時，會觸發核准流程。&#x200B;URL 若遭拒絕，系統預設會將狀態變更為上一個狀態，對於新請求而言並不理想。&#x200B;URL 相反地，應該選擇不同的狀態，例如「將不會解析」。&#x200B;URL 影片還指出，預設不會提供「已拒絕」狀態，但系統管理員可視需要建立一個狀態。&#x200B;URL

>[!VIDEO](https://video.tv.adobe.com/v/3455013/?quality=12&learn=on&enablevpops)

## 關鍵重點

* **預設核准流程：**&#x200B;建立請求佇列時，您可以套用預設核准流程，自動指派核准工作流程給每個請求。
* **核準時狀態變更：**&#x200B;已核准的請求會將其狀態從「新增 — 未決核准」變更為「新增」，允許指派的個人開始處理這些請求。
* **拒絕處理的常見錯誤：**&#x200B;如果要求被拒絕，由於核准程式中的預設系統設定，狀態將恢復為「新」。
* **已拒絕要求的建議狀態：**&#x200B;最好選擇其他狀態（例如「將不會解決」），而不是回覆成先前的狀態（「新增」），以避免混淆。
* **自訂狀態選項：**&#x200B;預設不會提供「已拒絕」狀態，但系統管理員可視需要建立狀態，以更清楚說明核准程式。


## 有關此主題的推薦教學課程

* [委派任務、問題與核准](/help/manage-work/approval-processes-and-milestone-paths/delegate-approvals.md)
* [瞭解特定群組的核准流程](/help/administration-and-setup/approval-processes-and-milestone-paths/group-specific-approval-processes.md)
* [建立請求流程](/help/manage-work/request-queues/create-a-request-flow.md)
* [建立全域和單次使用的核准程式](https://experienceleague.adobe.com/zh-hant/docs/workfront-learn/tutorials-workfront/manage-work/approval-processes-and-milestone-paths/create-a-single-use-approval-process)
