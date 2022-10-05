---
title: 配置全局預設問題首選項
description: 了解如何為轉換的問題、實際日期和問題存取設定問題偏好設定。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
kt: 10018
exl-id: 9924e479-c300-47b4-8e40-241ebb2435cf
source-git-commit: 3ded3fe9d8b97b1c11cb382f8088930842399c98
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 0%

---

# 配置全局預設問題首選項

若干系統範圍的設定會針對下列情形中的問題行為建立預設值： [!DNL Workfront].

最佳做法是保留全局預設值，並允許項目經理在項目級別或項目模板中進行所需的調整。

您可以調整全域問題偏好設定，但建議您和您的 [!DNL Workfront] 顧問討論貴組織的工作流程、流程和報表需求所需的設定。 您的顧問也可協助您了解，如果某些設定變更，將會發生什麼情況。

問題首選項允許系統管理員控制將問題轉換為任務或項目時的選項、如何計算實際日期，以及在分配問題時由誰獲得項目訪問權限。 讓我們查看這些設定在何處 [!DNL Workfront].

## 轉換的問題首選項

這些設定可控制問題轉換為 [!DNL Workfront].

![[!UICONTROL 工作與問題] 首選項窗口 [!UICONTROL 問題] 突出顯示的部分](assets/admin-fund-issue-prefs-converting.png)

1. 按一下 **[!UICONTROL 設定]** 在 **[!UICONTROL 主菜單]**.
1. 展開 **[!UICONTROL 專案偏好設定]** 區段。
1. 選擇 **[!UICONTROL 工作與問題]**.
1. 捲動至 **[!UICONTROL 問題]** 區段。
1. 按一下所需的選項。
1. 等你完成了再保存。

讓我們查看本節中的選項，以便您為組織選擇適當的選項。

* **[!UICONTROL 當解決對象的狀態更改時，自動更新可解決的問題狀態]**

   此設定可讓您將原始問題的解決與新對象（任務或項目）的解決建立關聯。

   啟用此設定（已勾選）後，您可以建立與任務或專案狀態具有相同狀態索引鍵的自訂問題狀態。 當任務或項目（可解析的對象）設定為自定義狀態時，更改也會顯示在問題狀態上。

   禁用後，解析對象狀態將自動設定為預設狀態，而不是自定義狀態。

   為了讓此設定有任何效果，請使用[!UICONTROL 保留原始問題，並將其解決方案與任務掛鈎]」選項。

* **[!UICONTROL 保留原始問題，並將與任務/項目聯繫起來]**

   轉換問題時，會告訴 [!DNL Workfront] 以保留原始問題。 問題的狀態會隨著任務或項目的狀態更改而更改。 一旦將任務或項目標籤為完成，問題就會標籤為已解決。

   如果未核取此選項，則會刪除原始問題，並僅保留已轉換的任務或項目。

   此設定會影響報告專案上原始記錄或 [!DNL Workfront] 請求佇列。

* **[!UICONTROL 允許主要聯繫人訪問任務/項目]**

   這可讓建立原始問題的人員存取轉換期間建立的任務或專案。 他們可以審查工作、更新工作，並隨時了解工作進展。

* **[!UICONTROL 允許在轉換過程中變更這些設定]**

   選取時，此選項表示「」的預設設定[!UICONTROL 保留原始問題]&quot;和&quot;[!UICONTROL 允許主聯繫人]「 」可由轉換問題的使用者變更。 如果希望預設值保持不變，請取消選擇此選項。

<!---
learn more URLs
Configure system-wide task and issue preferences
Issue statuses
Create and customize system-wide statuses
--->

## 實際日期偏好設定

使用的日期類型有多種 [!DNL Workfront]. 實際日期是「時間戳記」， [!DNL Workfront] 會在特定狀態變更時產生。

此 [!UICONTROL 實際開始日期] 時間戳記會在問題狀態從「新」變更為其他狀態時建立。 此 [!UICONTROL 實際完成日期] timestamp是問題狀態變更為指示已關閉的狀態時。

請務必注意，此偏好設定會控制任務和問題的實際日期設定。

![[!UICONTROL 工作與問題] 首選項窗口 [!UICONTROL 實際日期] 突出顯示的部分](assets/admin-fund-issue-prefs-actual-dates.png)

1. 按一下 **[!UICONTROL 設定]** 在 **[!UICONTROL 主菜單]**.
1. 展開 **[!UICONTROL 專案偏好設定]** 區段。
1. 選擇 **[!UICONTROL 工作與問題]**.
1. 捲動至 **[!UICONTROL 實際日期]** 區段。
1. 選取 **[!UICONTROL 實際開始日期]** — [!UICONTROL 現在] （目前日期和時間）或 [!UICONTROL 計劃開始日期] ( [!UICONTROL 實際開始日期] 符合問題詳細資料中設定的開始日期)。
1. 現在，選取 **[!UICONTROL 實際完成日期]** — [!UICONTROL 現在] （目前日期和時間）或 [!UICONTROL 計畫完成日期] ( [!UICONTROL 實際開始日期] 符合問題詳細資料中設定的日期)。
1. 等你完成了再保存。


<!---
learn more URLs
Definitions for the project, task, and issue dates within Workfront
Configure system-wide task and issue preferences
--->

## 問題存取

此 [!UICONTROL 存取] 問題的設定會控制在Workfront中為使用者指派問題時，授與的存取權。 這些設定除了可存取與問題相關聯的專案外，還可控制問題本身的存取權。

在變更這些設定之前，請先與您的 [!DNL Workfront] 顧問和您的內部治理團隊。

![[!UICONTROL 工作與問題] 首選項窗口 [!UICONTROL 將某人指派給ISSUE時] 突出顯示的部分](assets/admin-fund-issue-prefs-access-1.png)

1. 按一下 **[!UICONTROL 設定]** 在 **[!UICONTROL 主菜單]**.
1. 展開 **[!UICONTROL 專案偏好設定]** 區段。
1. 選擇 **[!UICONTROL 工作與問題]**.
1. 捲動至 **[!UICONTROL 存取]** 區段，並尋找「[!UICONTROL 將某人指派給ISSUE時]」。
1. 設定問題本身的共用存取權 —  [!UICONTROL 檢視], [!UICONTROL Contribute]，或 [!UICONTROL 管理]. [!DNL Workfront] 建議保留進階選項原樣。
1. 如果問題受託人也應該擁有項目訪問權限，請選中此框
1. 然後，選擇項目的共用訪問權 —  [!UICONTROL 檢視], [!UICONTROL Contribute]，或 [!UICONTROL 管理]. 當您設定 [!UICONTROL 進階選項]，請記得貴組織的工作流程和存取需求。
1. 等你完成了再保存。

![[!UICONTROL 存取] 視窗顯示 [!UICONTROL Contribute] 選項](assets/admin-fund-issue-prefs-access-2.png)

<!---
learn more URLs
Configure system-wide task and issue preferences
Grant access to issues
--->
