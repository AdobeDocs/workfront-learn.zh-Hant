---
title: 設定全域預設問題偏好設定
description: 瞭解如何為轉換的問題、實際日期和問題存取權設定問題偏好設定。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10018
exl-id: 9924e479-c300-47b4-8e40-241ebb2435cf
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 0%

---

# 設定全域預設問題偏好設定

有幾個系統範圍的設定會建立問題在某些特定情況下的行為預設值，例如： [!DNL Workfront].

最佳實務是保留全域預設值，並允許專案經理在專案層級或專案範本中進行所需的調整。

您可調整全域問題偏好設定，但建議您與您的 [!DNL Workfront] 顧問會討論組織的工作流程、流程和報告需求所需設定。 您的顧問也可以協助您瞭解變更某些設定時會發生什麼情況。

問題偏好設定可讓系統管理員控制何時將問題轉換為任務或專案、如何計算實際日期以及在指派問題時誰獲得專案存取權的選項。 讓我們檢視這些設定所在的位置 [!DNL Workfront].

## 轉換的問題偏好設定

這些設定可控制當問題轉換為任務或專案時所發生的情況 [!DNL Workfront].

![[!UICONTROL 任務和問題] 偏好設定視窗具有 [!UICONTROL 問題] 區段醒目提示](assets/admin-fund-issue-prefs-converting.png)

1. 按一下 **[!UICONTROL 設定]** 在 **[!UICONTROL 主要功能表]**.
1. 展開 **[!UICONTROL 專案偏好設定]** 區段。
1. 選取 **[!UICONTROL 任務和問題]**.
1. 捲動至 **[!UICONTROL 問題]** 區段。
1. 按一下所需的選項。
1. 完成時儲存。

讓我們來看看本節中的選項，以便您為您的組織選擇適當的選項。

* **[!UICONTROL 當解析物件狀態變更時，自動更新可解析問題狀態]**

  此設定可讓您將原始問題的解決方案與新物件（任務或專案）的解決方案相關聯。

  啟用此設定後（已核取），您可以建立與任務或專案狀態具有相同狀態索引鍵的自訂問題狀態。 當任務或專案（可解析物件）設定為自訂狀態時，變更也會顯示在問題狀態上。

  停用時，解析物件狀態會自動設定為預設狀態，而不是自訂狀態。

  為了讓此設定有任何效果， &quot;[!UICONTROL 保留原始問題並將其解決方案連結至任務]必須選取「 」選項。

* **[!UICONTROL 保留原始問題並將問題與任務/專案聯絡起來]**

  當問題轉換後，這說明 [!DNL Workfront] 以保留原始問題。 問題狀態會隨著任務或專案狀態的變更而變更。 將任務或專案標籤為完成後，問題即標籤為已解決。

  如果未核取此選項，則會刪除原始問題，並且僅保留轉換的任務或專案。

  此設定會影響有關原本登入專案或來自的問題報告 [!DNL Workfront] 要求佇列。

* **[!UICONTROL 允許主要連絡人存取任務/專案]**

  這可讓建立原始問題的人員存取轉換期間建立的任務或專案。 他們可以檢閱工作、進行更新，並隨時瞭解進度。

* **[!UICONTROL 允許在轉換過程中變更這些設定]**

  選取時，此選項表示「」的預設設定[!UICONTROL 保留原始問題]「和」[!UICONTROL 允許主要連絡人]」可由轉換問題的使用者變更。 如果您希望預設值保持不變，請取消選取此選項。

<!---
learn more URLs
Configure system-wide task and issue preferences
Issue statuses
Create and customize system-wide statuses
--->

## 實際日期偏好設定

整個過程中使用了多種型別的日期 [!DNL Workfront]. 實際日期是「時間戳記」，該時間戳記會 [!DNL Workfront] 在某些狀態變更時產生。

此 [!UICONTROL 實際開始日期] 當問題狀態從新狀態變更為其他狀態時建立時間戳記。 此 [!UICONTROL 實際完成日期] timestamp是問題狀態變更為表示其關閉的狀態。

請務必注意，此偏好設定會控制任務和問題的實際日期設定。

![[!UICONTROL 任務和問題] 偏好設定視窗具有 [!UICONTROL 實際日期] 區段醒目提示](assets/admin-fund-issue-prefs-actual-dates.png)

1. 按一下 **[!UICONTROL 設定]** 在 **[!UICONTROL 主要功能表]**.
1. 展開 **[!UICONTROL 專案偏好設定]** 區段。
1. 選取 **[!UICONTROL 任務和問題]**.
1. 捲動至 **[!UICONTROL 實際日期]** 區段。
1. 選取所需的選項 **[!UICONTROL 實際開始日期]** — [!UICONTROL 現在] （目前的日期和時間）或 [!UICONTROL 計劃開始日期] (此 [!UICONTROL 實際開始日期] 符合問題詳細資料中設定的開始日期)。
1. 現在選取「 」的選項 **[!UICONTROL 實際完成日期]** — [!UICONTROL 現在] （目前的日期和時間）或 [!UICONTROL 計畫完成日期] (此 [!UICONTROL 實際開始日期] 符合問題詳細資料中設定的日期)。
1. 完成時儲存。


<!---
learn more URLs
Definitions for the project, task, and issue dates within Workfront
Configure system-wide task and issue preferences
--->

## 問題存取權

此 [!UICONTROL 存取] 問題設定可控制當使用者在Workfront中被指派問題時他們被授予的存取權。 除了存取與問題相關的專案外，這些設定還控制對問題本身的存取。

在變更這些設定之前，請與討論任何工作流程或程式需求 [!DNL Workfront] 顧問和您的內部治理團隊。

![[!UICONTROL 任務和問題] 偏好設定視窗具有 [!UICONTROL 將某人指派給問題時] 區段醒目提示](assets/admin-fund-issue-prefs-access-1.png)

1. 按一下 **[!UICONTROL 設定]** 在 **[!UICONTROL 主要功能表]**.
1. 展開 **[!UICONTROL 專案偏好設定]** 區段。
1. 選取 **[!UICONTROL 任務和問題]**.
1. 捲動至 **[!UICONTROL 存取]** 區段並找到&quot;[!UICONTROL 將某人指派給問題時]」選項。
1. 設定問題本身的共用存取權 —  [!UICONTROL 檢視]， [!UICONTROL Contribute]，或 [!UICONTROL 管理]. [!DNL Workfront] 建議將進階選項維持原狀。
1. 如果問題受指派人也應擁有專案的存取權，請核取方塊
1. 然後選取專案的共用存取權 —  [!UICONTROL 檢視]， [!UICONTROL Contribute]，或 [!UICONTROL 管理]. 當您設定 [!UICONTROL 進階選項]，請牢記您組織的工作流程與存取需求。
1. 完成時儲存。

![[!UICONTROL 存取] 視窗顯示 [!UICONTROL Contribute] 選項](assets/admin-fund-issue-prefs-access-2.png)

<!---
learn more URLs
Configure system-wide task and issue preferences
Grant access to issues
--->
