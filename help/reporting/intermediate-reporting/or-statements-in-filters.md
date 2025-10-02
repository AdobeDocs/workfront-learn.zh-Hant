---
title: 在篩選器中建立 OR 陳述式
description: Workfront彈性的篩選邏輯可讓使用者使用預設的「AND」規則、選用的「OR」條件，以及針對複雜條件整理的篩選群組，來調整報表檢視。
activity: use
team: Technical Marketing
feature: Reports and Dashboards
thumbnail: create-or-statements-in-filters.png
type: Tutorial
role: User
level: Intermediate
jira: KT-9987
exl-id: 1a56f2f6-12df-43a5-943c-986a85661efa
last-substantial-update: 2025-08-11T00:00:00Z
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 31%

---

# 在篩選器中建立 OR 陳述式

影片說明如何在Workfront中建立和使用具備多個規則的篩選器。&#x200B;URL 依預設，Workfront在篩選規則之間使用「AND」，這表示所有條件都必須為True，專案才會出現在清單中。
或者，您也可以將篩選邏輯變更為「OR」，以顯示符合任何條件的專案。
此影片也會示範如何使用篩選器群組來建立任務的篩選器。&#x200B;URL 例如，您可以建立兩個群組：一個用於指派給延遲創意團隊的未完成任務，另一個用於指派給未指派創意團隊的未完成任務。&#x200B;URL 在每個群組中，「AND」邏輯適用，這表示必須符合群組中的所有條件。&#x200B;URL 群組之間的「OR」邏輯可確保顯示符合任一群組條件的任務。

>[!VIDEO] (https://video.tv.adobe.com/v/3470692/?quality=12&learn=on&enablevpops=0

## OR 篩選活動

您想要尋找指派給您的或是未指派給任何人的未完成任務。您設定一個類似以下內容的篩選器。這個篩選器會產生您想要的結果嗎？為什麼會或不會？

![影像顯示未正確建立的 OR 陳述式，位於 [!DNL Workfront]](assets/or-statement-your-turn-1.png)

### 解答

否，此篩選不會提供您想要的結果（未完成的任務，已指派給您或未指派給任何人），因為任務完整的篩選規則僅在OR的一側。

相反的，這個篩選器會產生清單如下：

* 指派給您的未完成任務。
* **PLUS (OR)**
* 所有未指派的任務，無論狀態如何。

篩選器應如下所示。請注意，此篩選器在OR兩側都有任務完整度的篩選規則。

![影像顯示正確建立的 OR 陳述式，位於 [!DNL Workfront]](assets/or-statement-your-turn-2.png)
