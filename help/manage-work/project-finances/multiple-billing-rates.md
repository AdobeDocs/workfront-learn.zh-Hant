---
title: 瞭解多種收費率
description: 瞭解如何在專案中覆寫系統計費率。
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-multiple-billing-rates.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10048
exl-id: bda562b9-f8da-49c9-bea7-0440fdc4c24c
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# 瞭解多種收費率

範圍 [!DNL Workfront]，專案經理可以覆寫特定專案中的系統計費率。 先前，當新計費率套用至專案時，它不僅會影響未來時數，還會影響已記錄至專案的時數。

替換為 [!DNL Workfront]專案經理的全新多計費率功能可決定應套用計費率的時段。 如此一來，如果費率已經議定或變更，專案經理可以決定該費率何時生效。

## 變更收費率

1. 前往專案的登陸頁面。 選取 **[!UICONTROL 收費率]** 從左側面板。

   ![選取的影像 [!UICONTROL 收費率] 在 [!DNL Workfront]](assets/project-finances-1.png)

1. 從 **[!UICONTROL 收費率]** 索引標籤，按一下 **[!UICONTROL 新增收費率]** 按鈕。 選取 **[!UICONTROL 新收費率]** 下拉式清單中的。

   ![選取的影像 [!UICONTROL 新收費率] 在 [!DNL Workfront]](assets/project-finances-2.png)

1. 此 [!UICONTROL 新收費率] 對話方塊隨即顯示。 從 **[!UICONTROL 工作角色]** 在下拉式清單中，選取將套用新收費率的工作角色。

   ![在中選取新計費費率中工作角色的影像 [!DNL Workfront]](assets/project-finances-3.png)

1. 選取工作角色後， [!UICONTROL 預設收費率] 和 [!UICONTROL 收費率1] 欄位隨即顯示。 在「 」中輸入新的計費率 [!UICONTROL 收費率1] 欄位。 如果該收費率適用於整個專案（過去、目前和未來記錄的時數），請按一下 **[!UICONTROL 儲存]** 按鈕。

   ![儲存適用於整個專案的新計費率的影像 [!DNL Workfront]](assets/project-finances-5.png)

1. 如果新的收費率僅適用於特定時段，請按一下 **[!UICONTROL 新增費率]** 按鈕。 此 [!UICONTROL 記帳費率1結束日期] 和 [!UICONTROL 收費率2] 欄位隨即顯示。 輸入結束日期 [!UICONTROL 收費率1]. 您不能輸入開始日期 [!UICONTROL 收費率1] 因為系統假設它是在專案開始時啟動。

   ![建立適用於特定時段的新收費率的影像，從專案開始時開始，位置在 [!DNL Workfront]](assets/project-finances-6.png)

1. 如果不是這種情況：

   * 輸入下列專案的預設收費率 [!UICONTROL 收費率1].
   * 選取結束日期 [!UICONTROL 收費率1] ([!UICONTROL 預設收費率])。
   * 的開始日期 [!UICONTROL 收費率2] 將自動設定為之後的第二天 [!UICONTROL 收費率1] 結束。
   * 在「 」中輸入所需的收費率 [!UICONTROL 收費率2] 區段。
   * 視需要按一下「 」，繼續新增收費率 **[!UICONTROL 新增費率]** 按鈕。
   * 完成後，按一下 **[!UICONTROL 儲存]**.
   * 所有收費率將顯示在 [!UICONTROL 收費率] 索引標籤中。

   ![建立適用於中不同時段的新收費率的影像 [!DNL Workfront]](assets/project-finances-7.png)
