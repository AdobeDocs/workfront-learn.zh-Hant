---
title: 設定事件通知
description: 了解如何透過管理事件通知來控制使用者會收到哪些電子郵件和應用程式內通知。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
thumbnail: 10093.jpeg
kt: 10093
exl-id: 6bd3a777-0ed8-4383-ad8e-f1238e334e78
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 4%

---

<!---
this has the same content as the system administrator notification setup and mangement section of the email and inapp notificiations learning path
--->

<!---
add URL link in the note at the top of the LP
--->

# 設定事件通知

>[!NOTE]
>
>由於分階段推出，部分系統和群組管理員管理事件通知的功能暫時無法使用 [!DNL Workfront] 客戶。 請依照本文章了解此版本的更新內容：解鎖組的事件通知配置。

系統管理員決定使用者應透過 [!DNL Workfront].

![[!UICONTROL 電子郵件通知] 的 [!UICONTROL 設定] 區域](assets/admin-fund-notifications-1.png)

此 [!UICONTROL 事件通知] 清單會依類型分組。 對於列出的每個事件通知，您會看到五個資訊：

* **[!UICONTROL 作用中] —** 此 [!UICONTROL 作用中] 欄可讓您在系統範圍層級開啟或關閉通知。
* **[!UICONTROL 名稱] —** 這是內通知的名稱 [!DNL Workfront].
* **[!UICONTROL 說明] —** 說明提供簡短說明，說明為觸發通知所發生或在收到通知時需要採取的動作。
* **[!UICONTROL 電子郵件主旨] —** 當傳送電子郵件給使用者時，主旨行中會向使用者顯示的內容。
* **[!UICONTROL 群組存取] —** 解除鎖定通知，以便由群組管理員管理。

## 開啟通知

若要在全域系統層級管理通知，請確定搜尋列顯示 [!UICONTROL 系統事件通知].

按一下切換按鈕，使藍色顯示，開啟特定通知，讓所有使用者都能使用。 如果藍色隱藏，則通知關閉。

![[!UICONTROL 作用中] 欄 [!UICONTROL 電子郵件通知] 頁面](assets/admin-fund-notifications-2.png)

開啟事件通知後，訊息會在事件發生時立即傳送。

## 允許組管理員控制

系統管理員可以根據群組和子群組的運作方式及其工作流程，進一步自訂通知清單，授予群組管理員權限。

![[!UICONTROL 群組存取] 欄 [!UICONTROL 電子郵件通知] 頁面](assets/ganotifications_01.png)

要使組管理員能夠管理其組和子組的通知，需要解除系統級通知的鎖定。

* 導覽至「電子郵件通知」頁面的「事件通知」標籤。

* 請確定搜尋列顯示「系統事件通知」。

* 按一下「群組存取」欄中的切換按鈕，解除鎖定所有群組管理員的單一通知，使藍色顯示。

* 勾選每個通知左側的方塊，然後按一下清單上方工具列中的解除鎖定圖示，一次解除鎖定多個通知。

![[!UICONTROL 群組存取] 欄 [!UICONTROL 電子郵件通知] 頁面](assets/ganotifications_02.png)

按一下切換按鈕以鎖定解除鎖定的通知，以顯示灰色。 選取核取方塊並按一下工具列中的解除鎖定圖示，即可同時鎖定多個通知。

![[!UICONTROL 群組存取] 欄 [!UICONTROL 電子郵件通知] 頁面](assets/ganotifications_03.png)

頂層組管理員將顯示解除鎖定的通知，以確定其組和子組是否需要該通知。 子組將繼承其上層父組的通知配置。 ﻿


## 管理群組通知

在系統管理員具有解除鎖定的通知選項後，群組管理員可以按一下左側面板功能表中的事件通知，從個別的群組頁面管理群組的通知。 然後，您就可以啟用或停用通知選項。

![[!UICONTROL 群組存取] 欄 [!UICONTROL 電子郵件通知] 頁面](assets/managegroupnotifications_01.png)

如有需要，系統管理員可以在視窗頂端的搜尋列中輸入群組名稱，從「通知」頁面管理群組的通知。

![[!UICONTROL 群組存取] 欄 [!UICONTROL 電子郵件通知] 頁面](assets/managegroupnotifications_02.png)

## 專業技巧

有些通知 [!DNL Workfront] 建議讓使用者能使用。

對於大多數用戶：

* [!UICONTROL 我的其中一項任務的前置任務已完成]
* [!UICONTROL 有人將我加入定向更新]
* [!UICONTROL 有人對我的工作項目發表評論]
* [!UICONTROL 分配給我的任務的到期日更改]


專為項目經理：

* [!UICONTROL 我正在做的一個項目]
* [!UICONTROL 我持有的專案落後]
* [!UICONTROL 向我持有的專案新增了一個問題]
* [!UICONTROL 在我擁有的項目上已完成里程碑任務]

<!---
learn more URLs
--->
