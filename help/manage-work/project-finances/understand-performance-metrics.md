---
title: 瞭解績效量度
description: 瞭解如何使用績效量度 —  [!UICONTROL 績效指數方法] ([!UICONTROL PIM])和 [!UICONTROL 預估完成成本] ([!UICONTROL EAC])。
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
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# 瞭解績效量度

專案經理使用的兩個績效指標包括 [!UICONTROL 績效指數方法] ([!UICONTROL PIM])和 [!UICONTROL 預估完成成本] ([!UICONTROL EAC])。 系統範圍預設值可設定於 [!DNL Workfront] 並套用至新建立的專案。 [!UICONTROL PIM] 然後可以在個別專案上修改。

**[!UICONTROL 績效指數方法]**

的設定 [!UICONTROL PIM] 控制方式 [!DNL Workfront] 會計算其他專案績效量度，例如 [!UICONTROL 成本績效指數] ([!UICONTROL CPI])， [!UICONTROL 成本排程績效指數] ([!UICONTROL CSI])， [!UICONTROL 排程績效指數] ([!UICONTROL SPI])，以及 [!UICONTROL 預估完成成本] ([!UICONTROL EAC])。

的選項 [!UICONTROL PIM] 是以小時和成本為基礎。

* **基於小時** — Workfront在計算專案的CPI和EAC時使用計畫時數。 專案的EAC顯示為數字，以小時為單位。
* **基於成本** — Workfront使用計畫勞力成本來計算專案的CPI和EAC。 EAC會顯示為貨幣值。 使用此選項時，請確定任務受指派人（使用者和/或職務角色）與成本費率相關聯。

**[!UICONTROL EAC]**

[!UICONTROL EAC] 代表任務或專案完成時的預估總成本。 選項會在專案層級計算，並從任務/子任務累計。

* **在專案層級計算** — [!UICONTROL EAC] 上階作業與專案的實際時數/實際勞力成本決定於 [!UICONTROL EAC] 公式。 計算包括直接新增至父級任務或專案的實際時數/成本和費用。
* R **從任務/子任務向上滾動** — [!UICONTROL EAC] 上層任務和專案的，其決定方式為加上 [!UICONTROL EAC] 用於每個子任務。 此計算不包括直接新增到父級任務或專案的實際時數/成本。

此 [!UICONTROL EAC] 計算列於 [計算完工估算(EAC)](https://experienceleague.adobe.com/docs/workfront/using/manage-work/projects/project-finances/calculate-eac.html?lang=en).

**效能測量結果：設定**

要設定 [!UICONTROL PIM] 和 [!UICONTROL EAC] 系統預設值：

1. 選取 **[!UICONTROL 設定]** 從主功能表。
1. 按一下 **[!UICONTROL 專案偏好設定]** 在左側面板選單中，然後按一下 **[!UICONTROL 專案]**
1. 在 [!UICONTROL 專案狀態] 區段，尋找 [!UICONTROL 績效指數方法]. 選取以時數或成本為基準。
1. 對象 [!UICONTROL 預估完成成本]，選取「在專案層級計算」或「從任務/子任務累計」。
1. 按一下 **[!UICONTROL 儲存]** 在視窗底部。

![的影像 [!UICONTROL 專案偏好設定] 畫面](assets/setting-up-finances-1.png)

**設定 [!UICONTROL PIM] 在個別專案上**

1. 前往專案的登陸頁面。
1. 按一下 **[!UICONTROL 專案詳細資訊]** 從左側面板。
1. 開啟 **[!UICONTROL 財務]** 區段。
1. 連按兩下下文字 **[!UICONTROL 績效指數方法]** 以編輯它。
1. 選取以時數或成本為基準。
1. 按一下 **[!UICONTROL 儲存]** 變更完成。

![的影像 [!UICONTROL 專案詳細資訊] 畫面](assets/setting-up-finances-2.png)

[!UICONTROL PIM] 可以在以下位置對專案範本設定： [!UICONTROL 財務] 範本詳細資訊的部分。
