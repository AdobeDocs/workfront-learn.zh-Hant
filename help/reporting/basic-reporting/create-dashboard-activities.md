---
title: 建立儀表板活動
description: 透過逐步指示，練習建立控制面板。
activity: use
feature: Reports and Dashboards
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335157.png
jira: KT-8862
hidefromtoc: true
source-git-commit: 915b28bbbf138fa84dce6d1915387fbe22c63362
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 49%

---

# 建立儀表板活動

透過逐步指示，練習建立控制面板。

## 活動1：建立控制面板

建立[!UICONTROL 儀表板]，其中只有一個報告 — 「搜尋此專案的附註」。 這樣可以快速找到專案上的任何更新，即使要搜尋的更新多達數千。它會搜尋更新資料串，以利快速擷取符合您在提示中指定之條件的任何更新。

複製您在「建立備註報告」活動中建立的「搜尋備註報告」，以建立此報告（或者如果您未執行該活動，則使用其他報告）。

* 從複製中移除「專案名稱」提示，並將報告重新命名為「搜尋此專案的附註」。
* 將[!UICONTROL 儀表板]命名為「搜尋附註」。
* 前往任何專案登陸頁面並建立[!UICONTROL 儀表板]的自訂區段。
* 請注意，當您在自訂區段中搜尋附註時，它只會顯示您目前所在專案中所包含的附註。

## 答案1

1. 執行您在「建立備註報表」活動中建立的報表。
1. 按一下「**[!UICONTROL 報告動作]**」並選取「**[!UICONTROL 複製]**」。[!DNL Workfront]會建立名為「附註搜尋（複製）」的新報告。
1. 前往「**[!UICONTROL 報告動作]**」並選取「**[!UICONTROL 編輯]**」。按一下&#x200B;**[!UICONTROL 報表設定]**&#x200B;並將名稱變更為「搜尋此專案的附註」。
1. 按一下「[!UICONTROL 報告提示]」並刪除清單中的「[!UICONTROL 專案]」>「[!UICONTROL 名稱]」提示。

   ![影像顯示建立新儀表板的畫面](assets/edit-report-prompts.png)

1. 勾選「**[!UICONTROL 在儀表板中顯示提示]**」方塊。
1. 按一下「**[!UICONTROL 完成]**」，然後「**[!UICONTROL 儲存並關閉]**」。您現在看到的是報告的「[!UICONTROL 提示]」畫面。

   接下來，您將使用捷徑來建立新控制面板並新增此報表。

1. 按一下「**[!UICONTROL 報告動作]**」並選取「**[!UICONTROL 新增到儀表板]**」>「**[!UICONTROL 新增儀表板]**」。
1. 將報告「搜尋此專案的筆記」拖曳至&#x200B;**[!UICONTROL 配置]**&#x200B;面板。
1. 請注意，報告的名稱將成為儀表板的名稱。將名稱編輯為「搜尋附註」。

   ![影像顯示建立新儀表板的畫面](assets/create-dashboard.png)

1. 按一下「**[!UICONTROL 儲存並關閉]**」。

   現在把儀表板新增到專案頁面。

   ![影像顯示建立新儀表板的畫面](assets/add-custom-section.png)

1. 前往任何專案。從左側面板選單，按一下「**[!UICONTROL 新增自訂區段]**」圖示。
1. 在「**[!UICONTROL 新增儀表板]**」欄位中，輸入「搜尋附註」並從清單中選取[!UICONTROL 儀表板]。
1. 在&#x200B;**[!UICONTROL 自訂區段標題]**&#x200B;欄位中，輸入「搜尋備註」。
1. 按一下「**[!UICONTROL 新增新區段]**」。
1. 從左側面板選單中，找到「搜尋備註」。按一下區段名稱左邊的圓點，並把它拖曳到「更新」下方。
