---
title: 設定全域預設問題偏好設定
description: 瞭解如何設定轉換的問題、實際日期和問題存取權的問題偏好設定。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10018
exl-id: 9924e479-c300-47b4-8e40-241ebb2435cf
source-git-commit: 4568e4e47b719e2dee35357d42674613112a9c43
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 75%

---

# 設定全域預設問題偏好設定

數個全系統適用的設定已針對 [!DNL Workfront] 中問題在特定情況下之行為方式建立預設值。

最佳實務是保留原本的全域預設值，並允許專案經理人在專案層級或在專案範本中進行所需的調整。

您可以調整全域問題偏好設定，但建議您與您的[!DNL Workfront]顧問討論組織的工作流程、流程和報告需求所需設定。 您的顧問也可以協助您瞭解若是變更某些設定會發生什麼事。

系統管理員可以利用問題偏好設定來控制將問題轉換為任務或專案時的選項、實際日期的計算方式，以及指派問題時誰會獲得專案存取權。讓我們看看這些設定在[!DNL Workfront]中的位置。

## 轉換的問題偏好設定

這些設定可控制問題在[!DNL Workfront]中轉換為任務或專案時發生的情況。

![[!UICONTROL 任務與問題]偏好設定視窗，其[!UICONTROL 問題]區段突顯標示](assets/admin-fund-issue-prefs-converting.png)

1. 在&#x200B;**[!UICONTROL 主選單]**&#x200B;中按一下「**[!UICONTROL 設定]**」。
1. 展開左側選單面板中的「**[!UICONTROL 專案偏好設定]**」區段。
1. 選取「**[!UICONTROL 任務與問題]**」。
1. 捲動到「**[!UICONTROL 問題]**」區段。
1. 按一下所需的選項.
1. 完成時儲存。

讓我們看看本節中的選項，讓您可以為您的組織選擇適當的選項。

* **[!UICONTROL 當解決物件的狀態變更時，自動更新可解決問題狀態]**

  透過這項設定，您可以把初始問題的解決方案與新物件 (任務或專案) 的解決方案相互關聯。

  啟用這項設定 (勾選) 的情況下，您可以建立與任務或專案狀態擁有相同狀態索引鍵的自訂問題狀態。當任務或專案 (可解決物件) 設定為自訂狀態時，問題狀態上也會顯示變更。

  若停用，解決物件狀態會自動設為預設狀態而不是自訂狀態。

  為了讓此設定生效，必須選取&quot;[!UICONTROL 保留原始問題並將其解決方案連結至任務]&quot;選項。

* **[!UICONTROL 保留初始問題並將其解決方案連結至任務/專案]**

  當問題被轉換時，這個選項會讓 [!DNL Workfront] 保留初始問題。當任務或專案的狀態變更時，問題的狀態也會變更。任務或專案一旦標記為已完成，問題便會標記為已解決。

  如果未勾選這個選項，則初始問題會被刪除，僅保留轉換後的任務或專案。

  這項設定會影響我們針對原本記錄在專案上或是從 [!DNL Workfront] 請求佇列而來的問題之報告。

* **[!UICONTROL 允許主要聯絡人存取任務/專案]**

  建立初始問題的人員因此擁有在轉換時建立的任務或專案的存取權。他們可以檢閱工作、進行更新並隨時瞭解其進展。

* **[!UICONTROL 允許在轉換過程中變更這些設定]**

  選取此選項時，表示轉換問題的使用者可以變更「[!UICONTROL 保留原始問題]」和「[!UICONTROL 允許主要連絡人]」的預設設定。 如果您希望預設值維持不變，請取消選取這個選項。

<!--
learn more URLs
Configure system-wide task and issue preferences
Issue statuses
Create and customize system-wide statuses
-->

## 實際日期偏好設定

整個 [!DNL Workfront] 中使用多種類型的日期。實際日期是[!DNL Workfront]在某些狀態變更時產生的「時間戳記」。

當問題狀態從「新」變更為另一種狀態時，便會建立「[!UICONTROL 實際開始日期]」時間戳記。問題狀態變更為表示已結案的狀態時，便會產生「[!UICONTROL 實際完成日期]」時間戳記。

請務必注意，此偏好設定會控制任務和問題的實際日期設定。

![[!UICONTROL 任務與問題]偏好設定視窗，其[!UICONTROL 實際日期]區段突顯標示](assets/admin-fund-issue-prefs-actual-dates.png)

1. 在&#x200B;**[!UICONTROL 主選單]**&#x200B;中按一下「**[!UICONTROL 設定]**」。
1. 展開左側選單面板中的「**[!UICONTROL 專案偏好設定]**」區段。
1. 選取「**[!UICONTROL 任務與問題]**」。
1. 捲動到「**[!UICONTROL 實際日期]**」區段。
1. 選取所需的「**[!UICONTROL 實際開始日期]**」選項 —「[!UICONTROL 現在]」(目前日期和時間) 或「[!UICONTROL 規劃開始日期]」(「[!UICONTROL 實際開始日期]」與問題詳細資料中設定的開始日期相符)。
1. 現在選取「**[!UICONTROL 實際完成日期]**」的選項 —「[!UICONTROL 現在]」(目前日期和時間) 或「[!UICONTROL 規劃完成日期]」(「[!UICONTROL 實際開始日期]」與問題詳細資料中設定的開始日期相符)。
1. 完成時儲存。


<!--
learn more URLs
Definitions for the project, task, and issue dates within Workfront
Configure system-wide task and issue preferences
-->

## 問題存取權

問題的[!UICONTROL 存取權]設定可控制當使用者在Workfront中被指派問題時，他們被授予哪些存取權。 這些設定控制其對問題本身的存取權，以及與問題相關聯的專案之存取權。

在變更這些設定之前，請與您的 [!DNL Workfront] 顧問以及內部治理團隊討論任何工作流程或程序需求。

![[!UICONTROL 任務與問題]偏好設定視窗，其中突顯標示[!UICONTROL 有人被指派負責一個問題時]區段](assets/admin-fund-issue-prefs-access-1.png)

1. 在&#x200B;**[!UICONTROL 主選單]**&#x200B;中按一下「**[!UICONTROL 設定]**」。
1. 展開左側選單面板中的「**[!UICONTROL 專案偏好設定]**」區段。
1. 選取「**[!UICONTROL 任務與問題]**」。
1. 捲動至&#x200B;**[!UICONTROL 存取]**&#x200B;區段，並尋找&quot;[!UICONTROL 將某人指派給問題]&quot;選項。
1. 設定問題本身的共用存取權 —「[!UICONTROL 檢視]」、「[!UICONTROL 貢獻]」或「[!UICONTROL 管理]」。[!DNL Workfront] 建議維持原本的進階選項。
1. 如果問題受指派者也應該具有專案的存取權，請勾選方塊
1. 接著選取專案的共用存取權 —「[!UICONTROL 檢視]」、「[!UICONTROL 貢獻]」或「[!UICONTROL 管理]」。設定[!UICONTROL 進階選項]時，請牢記組織的工作流程與存取需求。
1. 完成時儲存。

![[!UICONTROL 存取]視窗顯示[!UICONTROL 貢獻]選項](assets/admin-fund-issue-prefs-access-2.png)

<!--
learn more URLs
Configure system-wide task and issue preferences
Grant access to issues
-->
