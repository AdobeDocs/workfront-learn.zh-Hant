---
title: 使用基於使用者的萬用字元建立篩選器
description: 瞭解如何使用基於使用者的萬用字元，以及如何建置基於已登入使用者的篩選器。
activity: use
feature: Reports and Dashboards
thumbnail: 336810.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9081
exl-id: 46c83acd-6e43-42aa-875f-ae24b09a7fee
doc-type: video
source-git-commit: 88c2161e897f23587ccc1d0e867b6f8961927a0f
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 48%

---

# 使用基於使用者的萬用字元建立篩選器

觀看這段影片，您將瞭解如何：

* 瞭解為何要使用萬用字元
* 使用基於使用者的萬用字元建立篩選器

>[!VIDEO](https://video.tv.adobe.com/v/336810/?quality=12&learn=on)

>[!TIP]
>
>建立搜尋任務或問題指派資料的篩選器時，請使用「指派使用者>>ID」欄位來源和名稱。此選項會檢視所有   指派給任務或問題的使用者，而不僅僅是「所有者」或主要受指派人。

>[!TIP]
>
>即使是建立自己使用的篩選器，亦請使用 $$USER.ID (而不是您的名稱)。如此一來，如果有人看到您正在執行的篩選器並說「請和我共用」，則篩選器已設定，因此每個使用它的人都會看到自己的資訊。

>[!TIP]
>
>使用基於使用者的萬用字元時，您一定要使用「等於」篩選限定詞。


## 使用以使用者為基礎的萬用字元活動建立篩選器

[按一下這裡](/help/assets/create-filters-with-user-based-wildcards-activities.pdf)以下載此頁面的 PDF 版本。

### 活動1

您這週有一些額外的時間，所以您想檢視您的團隊中是否有任何人可以協助處理他們的任務。 建立任務篩選器以尋找本週到期但尚未完成的任務。

### 答案1

您是協助隊友的絕佳人選！ 設定如下圖所示的濾鏡，您會找到工作：

* 尚未完成（表示他們沒有等於[!UICONTROL 完成]的[!UICONTROL 完成]狀態或狀態）；
* 位於狀態為[!UICONTROL 目前]的專案中（畢竟，您不想為尚未啟動的專案尋找任務）；
* 已指派給您的主團隊中某名成員，主團隊的定義按照 Workfront 團隊設定；
* 而完成日期為本週某個時間的（此規則使用預先建立的日期篩選器來定義「本週」）。

![影像顯示使用基於使用者的萬用字元建立任務篩選器的畫面](assets/user-wildcard-exercise-answer.png)

如果您想要對清單設定更多限制，您可能要新增其他篩選器。例如，您可能想要新增篩選規則去搜尋您的團隊負責的特定方案或專案組合。
