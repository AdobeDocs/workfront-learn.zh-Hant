---
title: 瞭解多種計費費率
description: 瞭解如何覆寫專案內的系統計費費率。
activity: use
team: Technical Marketing
feature: Work Management
thumbnail: understand-multiple-billing-rates.png
type: Tutorial
role: User
level: Intermediate
jira: KT-10048
hide: true
exl-id: 5b1ae2c4-43bd-4382-900f-078ef84408a5
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
autotag-review: '2026-05-05T19:00:23.025Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 438
ht-degree: 93%

---

# 瞭解多種計費費率

在 [!DNL Workfront] 中，專案經理人可以覆寫特定專案內的系統計費費率。 之前把新的計費費率套用到專案時，不但是未來的時數，連專案中已經記錄的時數也會受到影響。

透過[!DNL Workfront]的新多重收費率功能，專案經理能夠決定應套用收費率的時間段。 這樣一來，若費率經過議定或有所變更，專案經理人可以決定該費率何時生效。

## 更改計費費率

1. 前往專案的登陸頁面。 從左側面板選取「**[!UICONTROL 計費費率]**」。

   ![影像顯示選取[!UICONTROL 計費費率]，位於 [!DNL Workfront]](assets/project-finances-1.png)

1. 在「**[!UICONTROL 計費費率]**」標籤中，按一下「**[!UICONTROL 新增計費費率]**」按鈕。 從下拉式選單選取「**[!UICONTROL 新增計費費率]**」。

   ![影像顯示選取[!UICONTROL 新增計費費率]，位於 [!DNL Workfront]](assets/project-finances-2.png)

1. 接著顯示「[!UICONTROL 新增計費費率]」對話方塊。 在「**[!UICONTROL 職務角色]**」下拉式選單中，選取將套用新計費費率的職務角色。

   ![影像顯示在新計費費率中選取職務角色，位於 [!DNL Workfront]](assets/project-finances-3.png)

1. 選取職務角色之後，便會顯示「[!UICONTROL 預設計費費率]」和「[!UICONTROL 計費費率 1]」欄位。 在「[!UICONTROL 計費費率 1]」欄位中輸入新的計費費率。 如果該計費費率適用於整個專案 (過去、現在和未來所記錄的時數)，請按一下「**[!UICONTROL 儲存]**」按鈕。

   ![影像顯示儲存套用至整個專案的新計費費率，位於 [!DNL Workfront]](assets/project-finances-5.png)

1. 如果新的計費費率僅適用於特定時段，請按一下「**[!UICONTROL 新增費率]**」按鈕。 [!UICONTROL 「計費費率 1」的「結束日期」]和「[!UICONTROL 計費費率 2]」欄位出現。 輸入「[!UICONTROL 計費費率 1]」的「結束日期」。 您不能輸入「[!UICONTROL 計費費率 1]」的「開始日期」，因為系統假設它從專案開始時起算。

   ![影像顯示建立套用於特定時段的新計費費率，從專案開始時起算，位於[!DNL Workfront]](assets/project-finances-6.png)

1. 若不是上述情況：

   * 輸入「[!UICONTROL 計費費率 1]」的預設計費費率。
   * 選取「[!UICONTROL 計費費率 1]」([!UICONTROL 預設計費費率]) 的「結束日期」。
   * 「[!UICONTROL 計費費率 2]」的「開始日期」會自動設定為「[!UICONTROL 計費費率 1]」結束的隔天。
   * 在「[!UICONTROL 計費費率 2]」區段輸入所需的計費費率。
   * 如有需要，按一下「**[!UICONTROL 新增費率]**」按鈕繼續新增計費費率。
   * 完成時，按一下「**[!UICONTROL 儲存]**」。
   * 所有計費費率將會顯示在專案的「[!UICONTROL 計費費率]」標籤。

   ![影像顯示建立套用至不同時段的新計費費率，位於 [!DNL Workfront]](assets/project-finances-7.png)
