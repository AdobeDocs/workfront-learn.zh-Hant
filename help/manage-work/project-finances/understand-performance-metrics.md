---
title: 了解效能量度
description: 效能量度為 [!UICONTROL 效能索引方法] ([!UICONTROL PIM])和 [!UICONTROL 完成時的估計] ([!UICONTROL EAC])。
feature: Work Management
thumbnail: understand-performance-metrics.png
type: Tutorial
role: User
level: Intermediate
kt: 10065
exl-id: 190c66f5-b412-48bd-8695-3bd7da088ccb
source-git-commit: d0c842ad8bf6f52161f003a62237fbcd35d23176
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# 了解效能量度

項目經理使用的兩個效能指標包括 [!UICONTROL 效能索引方法] ([!UICONTROL PIM])和 [!UICONTROL 完成時的估計] ([!UICONTROL EAC])。 系統範圍的預設值可在 [!DNL Workfront] 並套用至新建立的專案。 [!UICONTROL PIM] 然後可在個別專案上修改。

**[!UICONTROL 績效指數方法]**

的設定 [!UICONTROL PIM] 控制方式 [!DNL Workfront] 計算其他項目效能度量，如 [!UICONTROL 成本效能指數] ([!UICONTROL CPI]), [!UICONTROL 成本計畫效能索引] ([!UICONTROL CSI]), [!UICONTROL 計畫效能索引] ([!UICONTROL SPI])和 [!UICONTROL 完成時的估計] ([!UICONTROL EAC])。

選項 [!UICONTROL PIM] 以小時為基礎，以成本為基礎。

* **小時型** —Workfront在計算項目的CPI和EAC時使用計畫時數。 專案的EAC會以小時為單位顯示為數字。
* **成本型** —Workfront在計算項目的CPI和EAC時使用計畫的人工成本。 EAC顯示為貨幣值。 使用此選項時，確保任務分配者（用戶和/或任務角色）與成本費率相關聯。

**[!UICONTROL EAC]**

[!UICONTROL EAC] 表示任務或項目完成時的預計總成本。 選項在專案層級計算，並從任務/子任務匯總。

* **在專案層級計算** — [!UICONTROL EAC] 對於父任務和項目，使用 [!UICONTROL EAC] 公式。 計算包括直接添加到父任務或項目的實際小時數/成本和費用。
* R **從任務/子任務中調出** — [!UICONTROL EAC] 對於父任務和項目，將 [!UICONTROL EAC] 每個子任務。 此計算不包括直接添加到父任務或項目的實際小時數/成本。

此 [!UICONTROL EAC] 計算列在「完成時計算估計(EAC)」中 <!-- link to article -->文章 [!UICONTROL [!DNL Workfront] 一].

**效能量度：設定**

若要設定 [!UICONTROL PIM] 和 [!UICONTROL EAC] 系統預設值：

1. 選擇 **[!UICONTROL 設定]** 的上界。
1. 按一下 **[!UICONTROL 專案偏好設定]** 在左側面板功能表中，按一下 **[!UICONTROL 專案]**
1. 在 [!UICONTROL 專案狀態] 區段，尋找 [!UICONTROL 效能索引方法]. 選擇基於小時或基於成本。
1. 針對 [!UICONTROL 完成時的估計]，選取「在專案層級計算」或「從任務/子任務匯總」。
1. 按一下 **[!UICONTROL 儲存]** 在窗底。

![的影像 [!UICONTROL 專案偏好設定] 螢幕](assets/setting-up-finances-1.png)

**設定 [!UICONTROL PIM] 關於個別專案**

1. 前往專案的登陸頁面。
1. 按一下 **[!UICONTROL 專案詳細資料]** 從左側面板。
1. 開啟 **[!UICONTROL 金融]** 區段。
1. 按兩下下方的文字 **[!UICONTROL 效能索引方法]** 來編輯。
1. 選擇基於小時或基於成本。
1. 按一下 **[!UICONTROL 儲存]** 完成變更。

![的影像 [!UICONTROL 專案詳細資料] 螢幕](assets/setting-up-finances-2.png)

[!UICONTROL PIM] 可在專案範本上設定，位於 [!UICONTROL 金融] 一節。
