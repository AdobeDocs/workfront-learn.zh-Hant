---
title: 設定事件通知
description: 瞭解如何透過管理事件通知來控制使用者會收到哪些電子郵件和應用程式內通知。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate
thumbnail: 10093.jpeg
jira: KT-10093
exl-id: 6bd3a777-0ed8-4383-ad8e-f1238e334e78
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
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
>由於分階段推出，允許系統和群組管理員管理事件通知的功能暫時不適用於部分使用者 [!DNL Workfront] 客戶。 請詳閱本文，瞭解版本相關更新：解鎖群組事件通知的設定。

系統管理員會決定使用者應透過哪些通知接收 [!DNL Workfront].

![[!UICONTROL 電子郵件通知] 中的視窗 [!UICONTROL 設定] 區域](assets/admin-fund-notifications-1.png)

此 [!UICONTROL 事件通知] 清單會依型別分組。 對於列出的每個事件通知，您將會看到五則資訊：

* **[!UICONTROL 作用中] —** 此 [!UICONTROL 作用中] 欄可讓您在整個系統層級開啟或關閉通知。
* **[!UICONTROL 名稱] —** 這是中的通知名稱 [!DNL Workfront].
* **[!UICONTROL 說明] —** 說明會提供觸發通知所發生的動作或接收通知時所需採取的動作的簡短說明。
* **[!UICONTROL 電子郵件主旨] —** 將電子郵件傳送給使用者時，在主旨行中向使用者顯示的內容。
* **[!UICONTROL 群組存取] —** 解鎖通知，以便群組管理員能夠管理這些通知。

## 開啟通知

若要在全球系統層級管理通知，請確定搜尋列顯示 [!UICONTROL 系統事件通知].

按一下切換按鈕，即可開啟特定通知，讓所有使用者都能使用，以顯示藍色。 如果藍色為隱藏，則通知為關閉。

![[!UICONTROL 作用中] 欄於 [!UICONTROL 電子郵件通知] 頁面](assets/admin-fund-notifications-2.png)

開啟事件通知後，訊息會在事件發生時立即傳送。

## 允許群組管理員控制

系統管理員可授予群組管理員許可權，讓他們進一步根據群組和子群組的運作方式及其工作流程來自訂通知清單。

![[!UICONTROL 群組存取] 欄於 [!UICONTROL 電子郵件通知] 頁面](assets/ganotifications_01.png)

若要讓群組管理員能夠管理其群組和子群組的通知，則需要解除鎖定系統層級通知。

* 切換作業選項至「電子郵件通知」頁面的「事件通知」標籤。

* 請確定搜尋列顯示為「系統事件通知」。

* 按一下「群組存取」欄中的切換按鈕，讓藍色顯示，以解除鎖定所有群組管理員的單一通知。

* 勾選每個通知左側的方塊，然後按一下清單上方工具列中的解鎖圖示，即可一次解鎖多個通知。

![[!UICONTROL 群組存取] 欄於 [!UICONTROL 電子郵件通知] 頁面](assets/ganotifications_02.png)

按一下切換即可鎖定解除鎖定的通知，使灰色顯示。 選取核取方塊並按一下工具列中的解鎖圖示，同時鎖定多個通知。

![[!UICONTROL 群組存取] 欄於 [!UICONTROL 電子郵件通知] 頁面](assets/ganotifications_03.png)

頂層群組管理員會顯示解除鎖定的通知，以判斷其群組和子群組是否需要該通知。 子群組會繼承其上層父群組的通知設定。 ﻿


## 管理群組通知

系統管理員解鎖通知選項後，群組管理員可以按一下左側面板選單中的「事件通知」，從個別群組頁面管理群組的通知。 然後，您就可以啟用或停用通知選項。

![[!UICONTROL 群組存取] 欄於 [!UICONTROL 電子郵件通知] 頁面](assets/managegroupnotifications_01.png)

如有需要，系統管理員可以透過視窗頂端的搜尋列輸入群組名稱，從「通知」頁面管理群組通知。

![[!UICONTROL 群組存取] 欄於 [!UICONTROL 電子郵件通知] 頁面](assets/managegroupnotifications_02.png)

## Pro提示

有一些通知 [!DNL Workfront] 建議讓您的使用者可以使用。

對於大多數使用者：

* [!UICONTROL 我的其中一項任務的前置任務已完成]
* [!UICONTROL 有人將我加入定向更新]
* [!UICONTROL 有人對我工作專案發表評論]
* [!UICONTROL 在指派給我的任務上變更了到期日期]


專案經理專屬：

* [!UICONTROL 我所在的專案變為使用中]
* [!UICONTROL 我持有的專案落後]
* [!UICONTROL 向我持有的專案新增了一個問題]
* [!UICONTROL 在我持有的專案上完成了里程碑任務]

<!---
learn more URLs
--->
