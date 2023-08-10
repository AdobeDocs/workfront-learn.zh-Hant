---
title: 將問題/請求轉換為任務
description: 瞭解如何將問題轉換為其他工作專案。
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: convert-issues-to-other-work-items.jpeg
type: Tutorial
role: User
level: Intermediate
jira: KT-10069
exl-id: 1fd4d862-e44b-4c50-9663-70e727f6e9b7
source-git-commit: 060ceb14d274e8b2ad080c1f58290a2c5769e007
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# 將問題/請求轉換為任務

問題可能非常重大，因此解決該問題的時間和精力需要在專案時間表中予以考慮並分配適當的資源。 在此情況下，問題可轉換為任務。

![的影像 [!UICONTROL 轉換為任務] 中的問題選項 [!UICONTROL Workfront].](assets/15-convert-issue-to-task-menu-option.png)

1. 導覽至 [!UICONTROL 問題] 問題已登入之專案或任務的區段。 或在您有權存取的報告中尋找問題。
1. 按一下問題名稱以開啟。
1. 從問題名稱右側的3點選單中，選擇 **[!UICONTROL 轉換為任務]**.
1. 填寫 [!UICONTROL 轉換為任務] 表單。 首先，為新任務指定名稱和說明。
1. 如果新任務應屬於不同專案的一部分，請變更 [!UICONTROL 目標專案] 名稱。
1. 在 [!UICONTROL 選項] 部分，核取方塊以保留原始問題、允許存取新任務並保持完成日期。 進行這些選取時，請依照您組織的工作流程進行。
1. 如果要將自訂表單資料從問題傳輸到任務，請附加自訂表單。 （問題表單與任務表單中存在的所有欄位都會自動轉移到任務表單。）
1. 按一下 **[!UICONTROL 轉換為任務]** 完成。

![的影像 [!UICONTROL 轉換為任務] 中的問題形式 [!UICONTROL Workfront].](assets/16-convert-to-task-options.png)

取決於貴組織的 [!DNL Workfront] 系統設定時，您可能無法變更轉換任務時選項區段中的設定。 這些選項會影響原始問題和新任務。

* **保持初始問題並將其解決方案連結至此任務** 保留原始問題和相關資訊（小時、檔案等）。 選取此選項後，任務完成後，問題將標籤為已解決。 如果此選項為 **非** 選擇「 」，在建立任務時會刪除原始問題。 這可能會影響您的組織如何追蹤和報告問題。
* 此 **允許（使用者名稱）存取此工作** 選項將允許建立問題的人員存取此新任務。
* 此 **保持問題的計畫完成日期** 選項可讓您保留已設定在問題上的計畫完成日期。 這會將任務限制設為 [!UICONTROL 完成時間不晚於]. 如果取消核取此方塊，則會設定任務的日期，就像在專案中建立新任務一樣。

新任務會放置在專案上任務清單的底部。 將任務移至所需位置、將使用者或團隊指派至工作、新增計畫時數和持續時間等。

>[!NOTE]
>
>您無法將問題新增至專案時間表，因為它們代表「未計畫的工作」。 專案時間表是針對「計畫工作」，即任務。


