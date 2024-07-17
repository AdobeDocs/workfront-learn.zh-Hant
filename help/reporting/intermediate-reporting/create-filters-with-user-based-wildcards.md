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
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 100%

---

# 使用基於使用者的萬用字元建立篩選器

觀看這段影片，您將瞭解如何：

* 瞭解為何要使用萬用字元
* 使用基於使用者的萬用字元建立篩選器

>[!VIDEO](https://video.tv.adobe.com/v/336810/?quality=12&learn=on)

>[!TIP]
>
>建立搜尋任務或問題指派資料的篩選器時，請使用「指派使用者>>ID」欄位來源和名稱。這個選項會搜尋指派至任務或問題的所有使用者，而不只是「所有者」或主要受指派人。

>[!TIP]
>
>即使是建立自己使用的篩選器，亦請使用 $$USER.ID (而不是您的名稱)。這樣一來，若有人看到您所執行的篩選器並要求共用時，該篩選器的原本設定便能讓每個人看到自己的資訊。

>[!TIP]
>
>使用基於使用者的萬用字元時，您一定要使用「等於」篩選限定詞。

## 活動

您這一週多了一些閒空時間，所以想要看看團隊中是否有人需要協助處理他們的指派工作。建立任務篩選器來尋找本週到期但尚未完成的任務。

## 解答

您對團隊同事伸出援手實在是太棒了！利用如下圖所示的篩選器設定，您能找到符合以下條件的任務：

* 尚未完成 (表示狀態不是「[!UICONTROL 完成]」也不是等同於「[!UICONTROL 完成]」)；
* 屬於狀態為「[!UICONTROL 目前]」的專案 (畢竟您不想找到尚未啟動的專案的任務)；
* 已指派給您的主團隊中某名成員，主團隊的定義按照 Workfront 團隊設定；
* 以及完成日期是本週某日 (此規則使用預先建立的日期篩選器來定義「本週」)。

![影像顯示使用基於使用者的萬用字元建立任務篩選器的畫面](assets/user-wildcard-exercise-answer.png)

如果您想要對清單設定更多限制，您可能要新增其他篩選器。例如，您可能想要新增篩選規則去搜尋您的團隊負責的特定方案或專案組合。
