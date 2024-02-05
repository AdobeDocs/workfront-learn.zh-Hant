---
title: 設定事件通知
description: 瞭解如何透過管理事件通知來控制使用者接收的電子郵件和應用程式內通知。
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
workflow-type: ht
source-wordcount: '621'
ht-degree: 100%

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
>因為採取分階段推行的方式，有些 [!DNL Workfront] 使用者暫時無法使用允許系統和群組管理員管理事件通知的功能。關於功能發佈的最新消息，請關注本文章：開放使用群組事件通知設定

系統管理員會決定使用者應該收到 [!DNL Workfront] 的哪些通知。

![[!UICONTROL 電子郵件通知]視窗，位於[!UICONTROL 設定]區域](assets/admin-fund-notifications-1.png)

「[!UICONTROL 事件通知]」清單依類型分組。所列出的每一個事件通知均有五項資訊：

* **[!UICONTROL 進行中] —**&#x200B;您可以利用「[!UICONTROL 進行中]」欄來關閉或開啟適用於全系統的通知。
* **[!UICONTROL 名稱] —**&#x200B;這是 [!DNL Workfront] 內通知的名稱。
* **[!UICONTROL 描述] —**&#x200B;該描述簡要說明發生哪些動作而觸發了通知，或是收到通知後要採取哪些動作來回應。
* **[!UICONTROL 電子郵件主旨] —**&#x200B;傳送電子郵件給使用者時，在主旨行顯示的內容。
* **[!UICONTROL 群組存取] —**&#x200B;開放通知的存取權，讓群組管理員可以管理通知。

## 開啟通知

若要管理全域系統層級的通知，請確認搜尋列顯示「[!UICONTROL 系統事件通知]」。

按一下切換按鈕使其顯示藍色，即可開啟特定通知，讓所有使用者均會收到通知。若未顯示藍色，則通知是關閉狀態。

![[!UICONTROL 進行中]欄，位於[!UICONTROL 電子郵件通知]頁面](assets/admin-fund-notifications-2.png)

開啟事件通知後，事件發生時會立即傳送訊息。

## 允許群組管理員控制

系統管理員可以把權限授予群組管理員，讓後者根據其群組和子群組的功能以及本身的工作流程自訂通知清單。

![[!UICONTROL 群組存取]欄，位於[!UICONTROL 電子郵件通知]頁面](assets/ganotifications_01.png)

要讓群組管理員擁有管理群組和子群組通知的能力，便必須開放傳送系統層級的通知。

* 導覽到「電子郵件通知」頁面的「事件通知」標籤。

* 請確認搜尋列顯示「系統事件通知」。

* 按一下「群組存取」欄的切換按鈕使其顯示藍色，對所有群組管理員開放傳送單一通知。

* 勾選每個通知左邊的方塊，並按一下清單上方工具列的解鎖圖示，一次性開放傳送多個通知。

![[!UICONTROL 群組存取]欄，位於[!UICONTROL 電子郵件通知]頁面](assets/ganotifications_02.png)

按一下切換按鈕使其顯示灰色，把開放傳送的通知鎖定。選取多個核取方塊並按一下工具列的解鎖圖示，同時鎖定多個通知。

![[!UICONTROL 群組存取]欄，位於[!UICONTROL 電子郵件通知]頁面](assets/ganotifications_03.png)

最高層級的群組管理員會看到開放傳送的通知，並決定其群組和子群組是否也需要收到該通知。子群組繼承最上層父系群組的通知設定。﻿


## 管理群組通知

系統管理員開放通知選項之後，群組管理員便可以在個人的「群組」頁面上按一下左側面板選單的「事件通知」，管理群組的各項通知。接著您可以啟用或停用通知選項。

![[!UICONTROL 群組存取]欄，位於[!UICONTROL 電子郵件通知]頁面](assets/managegroupnotifications_01.png)

如有需要，系統管理員可以利用「通知」頁面並在視窗上方的搜尋列輸入群組名稱，即可管理群組的通知。

![[!UICONTROL 群組存取]欄，位於[!UICONTROL 電子郵件通知]頁面](assets/managegroupnotifications_02.png)

## 專業技巧

根據 [!DNL Workfront] 的建議，您應該讓使用者接收某些通知。

對於大多數使用者：

* [!UICONTROL 我的其中一項任務的前置任務已完成]
* [!UICONTROL 有人將我加入定向更新]
* [!UICONTROL 有人在我的工作項目留下註解]
* [!UICONTROL 指派給我的一項任務的到期日發生變更]


專案經理人專用：

* [!UICONTROL 我參與的專案變為使用中]
* [!UICONTROL 我擁有的一項專案進度落後]
* [!UICONTROL 我擁有的專案中新增了一個問題]
* [!UICONTROL 我擁有的專案完成了里程碑任務]

<!---
learn more URLs
--->
