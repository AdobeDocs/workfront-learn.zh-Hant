---
title: 設定全域預設專案設定
description: 瞭解如何變更自訂狀態、設定全域專案偏好設定以及建立作為全域預設設定的排程。
feature: System Setup and Administration
role: Admin
level: Intermediate
activity: deploy
type: Tutorial
team: Technical Marketing
thumbnail: 335065.png
jira: KT-8753
exl-id: b961ba8c-9597-4ed4-a6d7-79689c8e290d
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 100%

---

# 設定全域預設專案設定

<!--
21.4 updates have been made
-->

觀看這段影片，您將瞭解如何：

* 變更自訂狀態
* 設定全域專案偏好設定
* 建立和使用排程

>[!VIDEO](https://video.tv.adobe.com/v/335065/?quality=12&learn=on&enablevpops=1)

## 全域和群組專案、任務和問題設定

當您開啟 [!DNL Workfront] 中的「[!UICONTROL 專案]」設定時，您會注意到視窗頂端的搜尋列顯示「[!UICONTROL 系統專案偏好設定]」。您可以藉此知道這些設定對 [!DNL Workfront] 系統中每個人均有影響，因為這是全域設定。

![[!UICONTROL 專案偏好設定]頁面，位於[!UICONTROL 設定]](assets/admin-fund-system-project-preferences-1.png)

在您開啟「[!UICONTROL 任務和問題]」設定時，將會看到類似的內容。

![[!UICONTROL 任務和問題偏好設定]，位於[!UICONTROL 設定]](assets/admin-fund-task-issue-preferences-2.png)

然而，有可能 [!DNL Workfront] 中並不是每個群組都需要相同的專案、任務和問題偏好設定。例如，行銷群組想把新專案的狀態設為「規劃」，而專案經理人群組想設為「請求」狀態。

[!DNL Workfront] 允許群組管理員為其群組調整某些專案、任務和問題偏好設定。[!DNL Workfront] 系統管理員會使用鎖定/解鎖切換按鈕來決定可以調整哪些偏好設定。

首先導覽到「[!UICONTROL 設定]」區域：

1. 在&#x200B;**[!UICONTROL 主選單]**&#x200B;中選取「**[!UICONTROL 設定]**」。
1. 展開左側選單的「**[!UICONTROL 專案偏好設定]**」。
1. 根據您要修改的設定，選取「**[!UICONTROL 專案]**」或「**[!UICONTROL 任務和問題]**」。

鎖定一個偏好設定，防止群組管理員為其群組調整該設定。

![偏好設定已鎖定的訊息](assets/admin-fund-preferences-locked-3.png)

將偏好設定解鎖，讓群組管理員可以自訂。

![偏好設定已解鎖的訊息](assets/admin-fund-preferences-unlocked-4.png)

有些設定無法解鎖，所以會保留全域系統設定。

![偏好設定已鎖定的訊息](assets/admin-fund-preferences-always-locked-5.png)

### 設定群組和子群組偏好設定

對於系統管理員解鎖的任何設定，群組管理員可為所管理的群組以及群組之下的任何巢狀子群組進行調整。此外，群組管理員可以控制其子群組管理員可以修改哪些設定。

1. 在&#x200B;**[!UICONTROL 主選單]**&#x200B;中選取「**[!UICONTROL 設定]**」。
1. 按一下左側選單中的「**[!DNL Groups]**」。
1. 按一下群組或子群組名稱來開啟。
1. 在左側選單中選取「**[!UICONTROL 專案偏好設定]**」或「**[!UICONTROL 任務和問題偏好設定]**」。
1. 針對已解鎖的每項偏好設定進行所需變更。
1. 選取&#x200B;**[!UICONTROL 「儲存」]**。

![[!UICONTROL 專案狀態]區段，位於[!UICONTROL 群組]頁面](assets/admin-fund-group-preferences.png)

如果您的組織沒有使用群組管理員，則系統管理員可以管理不同群組的偏好設定。

<!--
learn more URLs and guides
Create or edit a group status 
Group administrators 
Configure system-wide project preferences 
Configure project preferences for a group 
Configure task and issue preferences for a group 
Create and modify a group’s schedule 
-->
