---
title: 了解多種計費率
description: 在Workfront中，專案經理可以覆寫特定專案中的系統計費率。
feature: Work Management
thumbnail: understand-multiple-billing-rates.png
type: Tutorial
role: User
level: Intermediate
kt: 10048
exl-id: bda562b9-f8da-49c9-bea7-0440fdc4c24c
source-git-commit: d0c842ad8bf6f52161f003a62237fbcd35d23176
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# 了解多種計費率

內 [!DNL Workfront]，專案經理便能覆寫特定專案內的系統計費率。 以前，將新的計費率套用至專案時，不僅會影響未來小時數，也會影響已登入專案的小時數。

使用 [!DNL Workfront]項目經理的新多計費費率功能，能夠決定應應用計費費率的時間段。 這樣，如果某個費率已經協商或更改，項目經理就可以確定該費率何時生效。

## 更改開單率

1. 前往專案的登陸頁面。 選擇 **[!UICONTROL 計費率]** 從左側面板。

   ![選擇的影像 [!UICONTROL 計費率] in [!DNL Workfront]](assets/project-finances-1.png)

1. 從 **[!UICONTROL 計費率]** ，按一下 **[!UICONTROL 添加計費率]** 按鈕。 選擇 **[!UICONTROL 新計費率]** 中。

   ![選擇的影像 [!UICONTROL 新計費率] in [!DNL Workfront]](assets/project-finances-2.png)

1. 此 [!UICONTROL 新計費率] 對話框。 從 **[!UICONTROL 工作角色]** 下拉式清單，選擇將應用新計費率的作業角色。

   ![在 [!DNL Workfront]](assets/project-finances-3.png)

1. 一旦選取工作角色， [!UICONTROL 預設開單率] 和 [!UICONTROL 計費率1] 欄位。 在 [!UICONTROL 計費率1] 欄位。 如果此計費率適用於整個專案（過去、現在和未來記錄的小時數），請按一下 **[!UICONTROL 儲存]** 按鈕。

   ![儲存適用於以下項目的新計費率的影像： [!DNL Workfront]](assets/project-finances-5.png)

1. 如果新計費率僅適用於特定時段，請按一下 **[!UICONTROL 新增率]** 按鈕。 此 [!UICONTROL 開單費率1結束日期] 和 [!UICONTROL 計費率2] 欄位。 輸入的結束日期 [!UICONTROL 計費率1]. 您不能為 [!UICONTROL 計費率1] 因為系統假定它在項目開始時啟動。

   ![一種影像，可建立適用於特定時段的新計費率，從中的專案開始開始開始。 [!DNL Workfront]](assets/project-finances-6.png)

1. 如果情況並非如此：

   * 輸入的預設開單費率 [!UICONTROL 計費率1].
   * 選擇結束日期 [!UICONTROL 計費率1] ([!UICONTROL 預設開單率])。
   * 開始日期 [!UICONTROL 計費率2] 會自動設為 [!UICONTROL 計費率1] 結束。
   * 在 [!UICONTROL 計費率2] 區段。
   * 視需要繼續新增計費率，方法是按一下 **[!UICONTROL 新增率]** 按鈕。
   * 完成後，按一下 **[!UICONTROL 儲存]**.
   * 所有計費率將顯示在 [!UICONTROL 計費率] 頁簽。
   ![一種影像，用於建立適用於 [!DNL Workfront]](assets/project-finances-7.png)
