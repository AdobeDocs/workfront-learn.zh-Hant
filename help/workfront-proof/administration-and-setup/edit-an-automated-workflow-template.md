---
title: 編輯自動化工作流程範本
description: 瞭解在  [!DNL  Workfront] 中如何在現有的自動化校訂工作流程範本中進行變更。
activity: use
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
team: Technical Marketing
thumbnail: 335131.png
jira: KT-8831
exl-id: 03841b1f-741d-4427-ae84-ddb9f890fc95
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 100%

---

# 編輯自動化工作流程範本

隨著校訂檢閱與核准流程有所改進或發生組織變更，自動化工作流程範本應更新並反映使用 Workfront 之團隊目前的運作。

保持範本最新狀態可確保檢閱與核准流程的一致性，也能節省上傳校訂的時間，因為不需要持續調整工作流程。

1. 從 [!DNL Workfront] 的&#x200B;**[!UICONTROL 主選單]**&#x200B;選取「**[!UICONTROL 校訂]**」。
1. 在那裡的左側面板選單中選取「**[!UICONTROL 工作流程]**」。
1. 按一下範本名稱最右邊的三圓點選單，並選取「**[!UICONTROL 檢視範本詳細資料]**」。

共用、複製和刪除範本的選項位在每個範本的範本詳細資料視窗的頂端。刪除範本不會影響已套用該範本的進行中校訂，但是該範本將無法再使用。

![範本詳細資料視窗](assets/proof-system-setup-edit-templates-details-area.png)

<!--
Lean More URLs
-->

按一下箭頭展開「[!UICONTROL 詳細資料]」區段，以便變更範本名稱或範本時區一類設定。

## 變更階段和收件者

當因為流程簡化使得截止期限提早，或是有人參與團隊並將檢閱校訂時，「[!UICONTROL 工作流程]」區域可能需要變更。

自動化工作流程的每個階段均有專屬區段，可以獨立修改截止期限、隱私權、校訂收件者和其他資訊。

這段影片簡單示範您在「[!UICONTROL 工作流程]」區域可做的一些變更。參閱本影片下方的項目符號清單來檢視這些設定。這段影片沒有音訊。

>[!VIDEO](https://video.tv.adobe.com/v/335131/?quality=12&learn=on)

回顧以下這些在「[!UICONTROL 工作流程]」區段可以進行的校訂範本變更：

* 按一下進入「[!UICONTROL 階段名稱]」欄位或「[!UICONTROL 截止期限]」欄位來更新該資訊。
* 選取「[!UICONTROL 截止期限]」旁邊的箭頭來鎖定階段、決定要啟動哪個階段，或是只需要一個決定。
* 在收件者清單中，按一下進入「[!UICONTROL 角色]」或者「[!UICONTROL 電子郵件提示]」欄位來選擇另一個選項。
* 使用收件者名稱最右邊的三圓點選單，可刪除清單中的收件者、讓他們成為該工作流程階段的主要決策者，或是編輯校訂角色和電子郵件警報資訊。
* 您有兩個選項可以把收件者新增到清單中。您開啟「[!UICONTROL 新增人員至階段]」視窗後，按一下想要新增人員的階段。接著在收件者清單中輸入他們的名稱或電子郵件地址，並指派校訂角色和電子郵件警報。執行完成時按一下「[!UICONTROL 新增人員]」按鈕。
   1. 在每個階段區段的右上角，前往「[!UICONTROL 更多]」選單並選取「[!UICONTROL 新增人員至階段]」。
   1. 在「[!UICONTROL 工作流程]」區域的頂端，選取「[!UICONTROL 新增人員至階段]」。

## 範本共用

「[!UICONTROL 共用對象]」區域顯示可使用範本的校訂使用者。按一下人員名稱最右邊的三圓點選單並選取「[!UICONTROL 移除]」，將不再需要使用範本的人員移除。

![[!UICONTROL 共用對象]清單](assets/proof-system-setups-edit-template-shared-with.png)

但是，您在這個區段無法將人員新增到共用清單。若要新增，請返回範本詳細資料視窗的頂端並按一下「[!UICONTROL 共用範本]」按鈕。

## 活動區段

[!DNL Workfront] 保留範本所做變更的稽核歷史記錄。您可以查看日期、進行變更者以及關於所做變更的簡短資訊。

本區段不記錄校訂何時使用範本的相關資訊。

![校訂活動清單](assets/proof-system-setups-edit-template-activity.png)
