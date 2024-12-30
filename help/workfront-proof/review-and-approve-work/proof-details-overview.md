---
title: 瞭解校訂詳細資料
description: 在  [!DNL  Workfront]  中透過摘要面板和「[!UICONTROL 資料詳細資料]」頁面，深入瞭解校訂的相關細節。
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: understand-proof-details.png
jira: KT-10110
exl-id: 196f9318-eced-4825-b0fd-8592b6cb3403
source-git-commit: cb72c429f0ef4cd9945282876aa49189dab1bd96
workflow-type: ht
source-wordcount: '1038'
ht-degree: 100%

---

# 瞭解校訂詳細資料

## 檢視校訂詳細資料

作為校訂管理員或所有者，您可以透過摘要面板以及「[!UICONTROL 文件詳細資料]」頁面瞭解校訂的相關細節。首先在專案、任務或問題的「[!UICONTROL 文件]」區段找到您的校訂。

### 摘要面板

從文件清單中選取一個校訂，然後按一下畫面右上角的「摘要」圖示。

![影像顯示專案的「[!UICONTROL 文件]」區段，其中已選取一個校訂。](assets/document-summary-1.png)

下一步按一下「概觀」，展開概觀區段。

![影像顯示專案的「[!UICONTROL 文件]」區段，其中已選取校訂而且摘要面板已展開。摘要面板圖示和摘要面板均突顯標示。](assets/document-summary-2.png)

然後向下捲動到「校訂」區段。您可以在這裡看到校訂所有者、進度、註解數量、狀態和截止日期。

![影像顯示專案的「[!UICONTROL 文件]」區段，其中已選取校訂而且摘要面板已展開。摘要面板圖示和摘要面板均突顯標示。](assets/document-summary-3.png)

備註：摘要面板的「[!UICONTROL 核准]」區段是用於&#x200B;**文件**&#x200B;核准，與校訂檢閱及核准流程&#x200B;**沒有**&#x200B;關聯。在 [!DNL Workfront] 中此兩者是分開的流程。

### [!UICONTROL 文件詳細資訊]

如需關於校訂的更多資訊，請按一下「[!UICONTROL 文件詳細資訊]」。

![影像顯示專案的「[!UICONTROL 文件]」區段，其中已選取一個校訂，且標示出「[!UICONTROL 文件詳細資訊]」。](assets/document-summary-4.png)

此動作會將您帶往「[!UICONTROL 文件詳細資訊]」頁面，並在左側面板顯示其他各種選項。

![影像顯示 [!DNL  Workfront] 中的校訂頁面。](assets/document-details.png)

需要注意的是，檢視校訂流程相關資訊的能力，取決於您在 [!DNL Workfront] 中的校訂權限。

在校訂頁面中，您可以利用左側面板選單存取這些區段：

* **更新** — 於校訂檢視器中留下的註解會顯示在這裡，附有「校訂註解」標記。您也可以在檔案上留下註解，如同您在任務或專案上留下註解 (這些註解不會出現在校訂檢視器)。
* **批准** — 此區段用於文件核准而非校訂核准。兩種核准在 [!DNL Workfront] 中是獨立的流程，並未有任何連結。如果您使用校訂工作流程進行檢閱和核准，您不會用到這個區段。
* **所有版本** — 追蹤和管理校訂的版本歷史記錄。使用「[!UICONTROL 文件]」清單中的摘要面板來存取這項資訊，是比較簡單的方法。
* **自訂表單** — 校訂使用自訂表單來擷取特定組織的資訊。這些資料可以與檔案一起傳送到整合式文件儲存系統，例如 [!DNL Workfront] DAM 或 Adobe Experience Manager。自訂表單由您的 [!DNL Workfront] 系統管理員或群組管理員進行設定。與您的團隊或管理員討論，瞭解您是否會在校訂上使用自訂表單。
* **校訂工作流程** — 管理或修改指派給校訂的工作流程。您也可以使用「[!UICONTROL 文件]」清單內校訂上的「[!UICONTROL 校訂工作流程]」連結來開啟這個視窗。

我們來詳細了解其中兩個區段：[!UICONTROL 校訂檢視器設定]與[!UICONTROL 校訂活動]。

### [!UICONTROL 校訂檢視器設定]

這些設定可協助您控制校訂本身的存取權。

![影像顯示校訂頁面的「[!UICONTROL 校訂檢視器設定]」，並突顯標示左側面板選單中的「[!UICONTROL 校訂檢視器設定]」選項](assets/proofing-settings-on-details-page.png)

* **[!UICONTROL 需要登入。此校訂無法與訪客使用者共用 ]—** 校訂僅可與擁有 [!DNL Workfront] 校訂授權的人員共用。
* **[!UICONTROL 要求以電子形式簽署決策] —**&#x200B;共用校訂時，此選項要求收件者需擁有 [!DNL Workfront] 的校訂權限，並應於做出校訂決策時輸入校訂密碼，以「電子形式簽署」校訂。(備註：校訂密碼與您的 [!DNL Workfront] 密碼不同。校訂密碼無法輕易存取，因此大多數收件人不會知道此密碼。) Adobe 建議您在使用此功能前先與 [!DNL Workfront] 顧問討論。
* **[!UICONTROL 做出所有必要的決定後鎖定校訂] —** 在完成校訂的每一項決定之後，此選項會鎖定校訂，避免再做任何註解、回覆、決定等。這樣會鎖定整個校訂版本，而不僅是校訂工作流程的特定階段。
* **[!UICONTROL 允許下載原始檔案] —** 校訂收件者可以從校訂檢視器下載校訂的原始來源檔案。
* **[!UICONTROL 允許透過公共 URL 或內嵌程式碼共用校訂] —** 校訂收件者可以與任何人共用可供公眾存取的校訂連結。
* **[!UICONTROL 允許透過公開 URL 或內嵌程式碼訂閱校訂] —** 收到公開 URL 的任何人可以使用其電子郵件地址和名稱 (若不是校訂使用者) 或是其電子郵件地址和校訂密碼 (若是校訂使用者)，把自己新增到校訂中。(備註：校訂密碼與 [!DNL Workfront] 密碼不相同。)


### [!UICONTROL 校訂活動]

此頁面會追蹤校訂上發生的所有活動，以及所傳送之關於此校訂的電子郵件訊息。

![影像顯示校訂頁面的「[!UICONTROL 校訂活動]」區段，其中左側面板選單突顯標示「[!UICONTROL 校訂活動]」選項。](assets/proofing-activity-in-details.png)

「**[!UICONTROL 活動]**」區段會記錄各個註解與決定的時間戳記以及執行這些動作的使用者。此外，亦追蹤校訂工作流程階段的開始時間、收件者第一次開啟校訂的時間，以及其他校訂管理員或所有者想要知道的資訊。當您試圖了解某些問題，例如為什麼校訂工作流程階段並未啟動時，這些詳細資訊可能會有所幫助。

「**[!UICONTROL 訊息]**」區段記錄電子郵件警報和訊息傳送給收件者的時間戳記、寄件者及訊息內容。如果有人表示他們未收到校訂相關的電子郵件，而您要針對此事進行疑難排解時，這些資訊可能會有所幫助。您可以確認電子郵件是否發送以及於何時發送。

Adobe 建議校訂管理員和校訂所有者應熟悉這兩個區段內的資訊。當您擁有這些資訊且知道如何閱讀 [!UICONTROL SOCD] 進度列時，便能真正了解及管理您的校訂，無論處於校訂工作流程的哪個階段。

在您完成「[!UICONTROL 文件詳細資料]」區段的操作之後，請使用階層連結路徑返回校訂所在之專案、任務或問題的「[!UICONTROL 文件]」區段。

![影像顯示標頭內有階層連結路徑。](assets/proof-breadcrumb.png)

<!--
#### Learn more
* [!UICONTROL Document details] overview
* Add a custom form to a document
* Request document approvals
* Summary for documents overview
* View activity on a proof within [!DNL Workfront]
-->
