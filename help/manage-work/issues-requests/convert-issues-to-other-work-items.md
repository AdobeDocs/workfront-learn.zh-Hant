---
title: 將問題轉換為其他工作專案
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
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1098'
ht-degree: 0%

---

# 將問題轉換為其他工作專案

## 將問題轉換為任務

一個問題可能非常重大，需要將其解決的時間和精力計入專案時間表，並分配適當的資源。 在此情況下，問題可轉換為任務。

![的影像 [!UICONTROL 轉換為任務] 中的問題選項 [!UICONTROL Workfront].](assets/15-convert-issue-to-task-menu-option.png)

1. 導覽至 [!UICONTROL 問題] 問題已登入之專案或任務的區段。 或在您有權存取的報告中尋找問題。
1. 按一下問題名稱以開啟。
1. 從問題名稱右側的3點選單中，選擇 **[!UICONTROL 轉換為任務]**.
1. 填寫 [!UICONTROL 轉換為任務] 表單。 首先，為新任務指定名稱和說明。
1. 如果新任務應是不同專案的一部分，請輸入專案名稱。
1. 在 [!UICONTROL 選項] 區段，核取方塊以保留原始問題、允許存取新任務並保持完成日期。 進行這些選擇時，請遵循您組織的工作流程。 如果要將自訂表單資料從問題傳輸到任務，請附加自訂表單。 （問題表單和任務表單中存在的所有欄位將自動轉移到任務表單。）
1. 填寫自訂表格（若已附加）。
1. 按一下 **[!UICONTROL 轉換為任務]** 完成。

![的影像 [!UICONTROL 轉換為任務] 中的問題形式 [!UICONTROL Workfront].](assets/16-convert-to-task-options.png)

視您組織的 [!DNL Workfront] 系統設定時，您可能無法變更轉換任務時選項區段中的設定。 這些選項會同時影響原始問題和新任務。

* **「保留原始問題，並將其解決方案與此任務繫結」** 保留原始問題和相關資訊（小時、檔案等）。 選取此選項後，任務完成後，問題將標籤為已解決。 如果未選取此選項，則會在任務完成時刪除原始問題。 這可能會影響貴組織追蹤和報告問題的方式。
* 此 **「允許（使用者名稱）存取此任務」** 選項將允許建立問題的人員存取此新任務。
* 此 **「保持問題的計畫完成日期」** 選項可讓您保留已在問題上設定的計畫完成日期。 這會將任務限制設定為 [!UICONTROL 完成時間不晚於]. 如果取消核取此方塊，則會設定任務的日期，就像在專案中建立新任務一樣。

新任務會放置在專案上任務清單的底部。 將任務移至所需位置、將使用者或團隊指派至工作、新增計畫時數和持續時間等。

>[!NOTE]
>
>您無法將問題新增至專案時間表，因為它們代表「未計畫工作」。 專案時間表是用於「計畫工作」，即任務。

## 將問題轉換為專案

有時候，解決問題本身或將其轉換為任務無法解決問題，因為解決問題的過程需要更複雜的協調。 在此情況下，您可以將問題轉換為專案。

1. 導覽至問題已登入之專案或任務的問題區段。 或在您有權存取的報告中尋找問題。
1. 按一下問題名稱以開啟。
1. 按一下問題名稱右側的3點選單，以顯示「更多」選單。
1. 然後選取是否要建立完全空白的新專案，或使用專案範本，以預先填入任務和時間表資訊。
1. 在轉換至專案視窗中填寫資訊，從專案名稱開始。
1. 根據您的團隊或組織的要求，填寫其他專案詳細資訊。
1. 在選項區段中，核取方塊以保留原始問題並允許存取新專案。 進行這些選擇時，請遵循您組織的工作流程。
1. 填寫自訂表格（若已附加）。 如果要將自訂表單資料從問題傳輸到專案，請附加自訂表單。 （問題表單和專案表單中存在的所有欄位都將自動轉移到專案表單。）
1. 按一下 **轉換為專案** 完成。

「轉換為專案」視窗中顯示的專案詳細資訊欄位取決於您用來建立專案的方法。 如果您使用「從範本轉換為專案」選項，您將在左側選單中看到更多資訊。

>[!NOTE]
>
>視您組織的Workfront系統設定而定，某些區段（例如選項區段）雖然可見，但可能無法存取。

![顯示轉換選項的專案畫面影像](assets/conversion-options.png)

* 按一下「**保留原始問題並將其解決方案連結至此專案**」選項。 此選項會保留原始問題和相關資訊（小時、檔案等）。 新專案完成時，問題會標籤為已解決。 如果未選取此選項，原始問題將在專案完成時刪除。 這可能會影響貴組織追蹤和報告問題的方式。
* 「**允許（使用者名稱）存取此專案**「選項可讓建立問題的人員存取正在建立的專案。

## 在轉換過程中維護資訊

<!-- Need link to wf one doc article below 

To learn about what information transfers when you convert an issue to a task or project, we recommend you read through the conversion considerations in the article, Convert issues. This lists what information is kept when converting issues and what isn’t. Workfront recommends you become familiar with these considerations so you don’t lose important information when converting issues to tasks or projects.

-->

傳輸自訂表單資料需要：

* 同一自訂表單的多個副本 — 一個用於問題，另一個用於任務或專案。 這些自訂表單上的欄位應該完全相符，因此資訊可以從一個自訂表單傳輸到另一個自訂表單。

* 或是選取問題、任務和/或專案物件的單一自訂表單。 使用此方法時，您只需在單一自訂表單中建立和維護自訂欄位即可。 這是近期的增強功能，比起擁有相同表單的多個復本要容易得多，但兩種方法都可以運作。



<!-- Need link to wf one doc article below

Learn more in the article, Transfer custom form data to a larger work item.

-->

<!-- Pro tips graphic -->

如果您在專案範本中加入自訂表單，則在轉換程式中選取範本時，將會自動指派該表單。

<!-- Learn more graphic and documentation article links 

* Convert issues
* Transfer custom form data to a larger work item
* Overview of resolving and resolvable objects
* Understanding resolving and resolvable objects
* Unlink issues from their resolvable objects

-->

## 從任何問題清單將問題轉換為任務或專案

為了提高您的工作效率，並讓在快節奏的環境中轉換問題更容易，您能夠從專案、報告或儀表板中的任何問題清單將問題轉換為任務或專案。 只要選取問題，然後按一下出現的3點選單。

![顯示問題轉換選項的專案畫面影像](assets/convert-from-a-list.png)

