---
title: 瞭解績效量度
description: 瞭解如何使用績效量度，包括[!UICONTROL 績效指數方法] ([!UICONTROL PIM]) 以及[!UICONTROL 預估完工成本] ([!UICONTROL EAC])。
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-performance-metrics.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10065
exl-id: 190c66f5-b412-48bd-8695-3bd7da088ccb
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '433'
ht-degree: 100%

---

# 瞭解績效量度

專案經理人使用的兩種績效量度包括[!UICONTROL 績效指數方法] ([!UICONTROL PIM]) 和[!UICONTROL 預估完工成本] ([!UICONTROL EAC])。在 [!DNL Workfront] 中可以設定全系統適用的預設值，並套用到新建立的專案。然後個別專案可以修改其 [!UICONTROL PIM]。

**[!UICONTROL PIM]**

[!UICONTROL PIM] 設定會控制 [!DNL Workfront] 計算其他專案效能量度的方式，例如[!UICONTROL 成本績效指數] ([!UICONTROL CPI])、[!UICONTROL 成本排程績效指數] ([!UICONTROL CSI])、[!UICONTROL 進度績效指數] ([!UICONTROL SPI]) 以及[!UICONTROL 預估完工成本] ([!UICONTROL EAC)]。

[!UICONTROL PIM] 的選項包含依小時計算和依成本計算。

* **依小時計算** — Workfront 使用規劃時數來計算專案的 CPI 和 EAC。專案的 EAC 以小時數為單位顯示一個數字。
* **依成本計算** — Workfront 使用規劃勞力成本來計算專案的 CPI 和 EAC。EAC 以貨幣價值的形式顯示。使用此選項時，請確保任務受指派者 (使用者和/或職務角色) 與成本費率相關聯。

**[!UICONTROL EAC]**

[!UICONTROL EAC] 代表您的任務或專案完成時的預計總成本。選項包括在專案層級計算以及將任務/子任務的資料匯總。

* **在專案層級計算** — 父系任務和專案的 [!UICONTROL EAC] 是使用 [!UICONTROL EAC] 公式中的實際時數/實際勞力成本計算出來。計算項目包含實際時數/成本以及直接新增到父系任務或專案的費用。
* **將任務/子任務的資料匯總**  — 父系任務和專案的 [!UICONTROL EAC] 是把每個子系任務的 [!UICONTROL EAC] 加總起來。此計算不包含直接新增到父系任務或專案的實際時數/成本。

[!UICONTROL EAC] 計算方式請參閱「[計算預估完工成本 EAC)](https://experienceleague.adobe.com/docs/workfront/using/manage-work/projects/project-finances/calculate-eac.html?lang=zh-Hant)」。

**績效量度：設定**

若要設定 [!UICONTROL PIM] 和 [!UICONTROL EAC] 的系統預設值：

1. 在主選單中選取「**[!UICONTROL 設定]**」。
1. 在左側面板選單中按一下「**[!UICONTROL 專案偏好設定]**」，再按一下「**[!UICONTROL 專案]**」
1. 在「[!UICONTROL 專案狀態]」區段，尋找「[!UICONTROL 績效指數方法]」。選取「依小時計算」或「依成本計算」。
1. 對於「[!UICONTROL 預估完工成本]」，請選取「在專案層級計算」或「將任務/子任務的資料匯總」。
1. 在視窗底部按一下「**[!UICONTROL 儲存]**」。

![影像顯示「[!UICONTROL 專案偏好設定]」畫面](assets/setting-up-finances-1.png)

**設定個別專案的 [!UICONTROL PIM]**

1. 前往專案的登錄頁面。
1. 按一下左側面板的「**[!UICONTROL 專案詳細資料]**」。
1. 開啟「**[!UICONTROL 財務]**」區段。
1. 按兩下「**[!UICONTROL 績效指數方法]**」下方的文字來進行編輯。
1. 選取「依小時計算」或「依成本計算」。
1. 按一下「**[!UICONTROL 儲存]**&#x200B;變更」來完成操作。

![影像顯示「[!UICONTROL 專案詳細資料]」畫面](assets/setting-up-finances-2.png)

您可以在專案範本上，在範本詳細資料的「[!UICONTROL 財務]」區段設定 [!UICONTROL PIM]。
