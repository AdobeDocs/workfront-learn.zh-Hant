---
title: 使用使用者型萬用字元建立篩選器
description: 了解如何使用使用者型萬用字元，以及如何根據登入的使用者建立篩選器。
activity: use
feature: Reports and Dashboards
thumbnail: 336810.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9081
exl-id: 46c83acd-6e43-42aa-875f-ae24b09a7fee
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---

# 使用使用者型萬用字元建立篩選器

在此影片中，您將學習如何：

* 了解為何使用萬用字元
* 使用使用者型萬用字元建立篩選器

>[!VIDEO](https://video.tv.adobe.com/v/336810/?quality=12)

>[!TIP]
>
>建立查看任務或發放分配資訊的篩選器時，請使用「分配用戶>> ID」欄位源和名稱。  此選項會查看指派給該任務或問題的所有用戶，而不只是「所有者」或主要受託人。

>[!TIP]
>
>即使您自己建立篩選器，也可以使用$$USER.ID（而非您的名稱）。 如此一來，如果有人看到您執行的篩選器並說「與我共用該篩選器」，篩選器就會設定完畢，讓使用篩選器的每個人都能看見自己的資訊。

>[!TIP]
>
>使用基於用戶的通配符時，始終必須使用等於篩選限定符。

## 活動

你這週有點多餘的時間，所以你想看看你的團隊中是否有人可以在他們的任務上得到一些幫助。 建立任務篩選器以查找本週到期但尚未完成的任務。

## 回答

你幫你的隊友真是太棒了！ 將篩選器設定如下圖所示，您便會找到工作：

* 尚未完成(表示沒有 [!UICONTROL 完成] 相當於的狀態或狀態 [!UICONTROL 完成]);
* 在專案中 [!UICONTROL 目前] 狀態（畢竟，您不想為尚未啟動的專案尋找工作）;
* 會依Workfront團隊設定的定義，指派給您主團隊中的某個人；
* 而且完成日期為本週某時（此規則使用預先建立的日期篩選器來定義「本週」）。

![使用基於用戶的通配符建立任務篩選器的螢幕影像](assets/user-wildcard-exercise-answer.png)

如果您需要進一步限制清單，則可能需要新增一些其他篩選器。 例如，您可能想要新增篩選規則，以查看您的團隊使用的特定方案或產品組合。
