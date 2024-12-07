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
workflow-type: tm+mt
source-wordcount: '1038'
ht-degree: 57%

---

# 瞭解校訂詳細資料

## 檢視校訂詳細資料

作為校訂管理員或所有者，您可以透過摘要面板以及「[!UICONTROL 文件詳細資料]」頁面瞭解校訂的相關細節。首先在專案、任務或問題的「[!UICONTROL 文件]」區段找到您的校訂。

### 摘要面板

從檔案清單中選取校訂，然後按一下畫面右上角的「摘要」圖示。

![已選取校訂之專案的[!UICONTROL 檔案]區段的影像。](assets/document-summary-1.png)

接下來，按一下「概觀」以展開「概觀」區段。

![影像顯示專案的「[!UICONTROL 文件]」區段，其中已選取校訂而且摘要面板已展開。摘要面板圖示和摘要面板均突顯標示。](assets/document-summary-2.png)

然後向下捲動至「校樣」區段。 您可以在此處檢視校訂所有者、進度、評論數量、狀態和到期日。

![影像顯示專案的「[!UICONTROL 文件]」區段，其中已選取校訂而且摘要面板已展開。摘要面板圖示和摘要面板均突顯標示。](assets/document-summary-3.png)

備註：摘要面板中的[!UICONTROL 核准]區段是用於&#x200B;**檔案**&#x200B;核准，而&#x200B;**不是**&#x200B;繫結至校訂檢閱和核准程式。 在 [!DNL Workfront] 中此兩者是分開的流程。

### [!UICONTROL 文件詳細資訊]

若要取得校訂的詳細資訊，請按一下[!UICONTROL 檔案詳細資料]。

![已選取校訂且強調顯示[!UICONTROL 檔案詳細資訊]之專案的[!UICONTROL 檔案]區段的影像。](assets/document-summary-4.png)

這會帶您進入[!UICONTROL 檔案詳細資料]頁面，以及左側面板中的各種其他選項。

![影像顯示 [!DNL  Workfront] 中的校訂頁面。](assets/document-details.png)

請務必注意，檢視校訂程式相關資訊的能力取決於您在[!DNL Workfront]中的校訂許可權。

從校訂的頁面，您可以從左側面板選單存取這些區段：

* **更新 —**&#x200B;在校訂檢視器中所做的評論會顯示在此處，並帶有「校訂評論」標籤。 您也可以在檔案上留下註解，如同您在任務或專案上留下註解 (這些註解不會出現在校訂檢視器)。
* **批准** — 此區段用於文件核准而非校訂核准。兩種核准在 [!DNL Workfront] 中是獨立的流程，並未有任何連結。如果您針對檢閱和核准使用校訂工作流程，則不會使用此區段。
* **所有版本** — 追蹤和管理校訂的版本歷史記錄。使用「[!UICONTROL 文件]」清單中的摘要面板來存取這項資訊，是比較簡單的方法。
* **自訂表單** — 校訂使用自訂表單來擷取特定組織的資訊。此資訊可與檔案一起傳遞至整合式檔案儲存系統，例如[!DNL Workfront] DAM或Adobe Experience Manager。 自訂表單由您的 [!DNL Workfront] 系統管理員或群組管理員進行設定。與您的團隊或管理員討論，瞭解您是否會在校訂上使用自訂表單。
* **校訂工作流程** — 管理或修改指派給校訂的工作流程。您也可以使用[!UICONTROL 檔案]清單中校訂上的[!UICONTROL 校訂工作流程]連結來開啟此視窗。

讓我們更仔細地瞭解下列兩個區段：[!UICONTROL 校訂檢視器設定]和[!UICONTROL 校訂活動]。

### [!UICONTROL 校訂檢視器設定]

這些設定可協助您控制校訂本身的存取權。

![影像顯示校訂頁面的「[!UICONTROL 校訂檢視器設定]」，並突顯標示左側面板選單中的「[!UICONTROL 校訂檢視器設定]」選項](assets/proofing-settings-on-details-page.png)

* **[!UICONTROL 需要登入。此校訂無法與訪客使用者共用 ]—** 校訂僅可與擁有 [!DNL Workfront] 校訂授權的人員共用。
* **[!UICONTROL 需要以電子方式簽署決定] —**&#x200B;共用校訂時，這需要收件者在[!DNL Workfront]中擁有校訂許可權，並在他們做出校訂決定時輸入校訂密碼，讓他們以電子方式簽署校訂。 (備註：校訂密碼與您的 [!DNL Workfront] 密碼不同。驗證密碼不容易存取，因此大多數收件者不會知道此密碼。) Adobe建議在使用此功能之前先與您的[!DNL Workfront]顧問交談。
* **[!UICONTROL 做出所有必要的決定後鎖定校訂] —** 在完成校訂的每一項決定之後，此選項會鎖定校訂，避免再做任何註解、回覆、決定等。這樣會鎖定整個校訂版本，而不僅是校訂工作流程的特定階段。
* **[!UICONTROL 允許下載原始檔案] —**&#x200B;校訂收件者可以從校訂檢視器下載校訂的原始來源檔案。
* **[!UICONTROL 允許透過公共 URL 或內嵌程式碼共用校訂] —** 校訂收件者可以與任何人共用可供公眾存取的校訂連結。
* **[!UICONTROL 允許透過公開 URL 或內嵌程式碼訂閱校訂] —** 收到公開 URL 的任何人可以使用其電子郵件地址和名稱 (若不是校訂使用者) 或是其電子郵件地址和校訂密碼 (若是校訂使用者)，把自己新增到校訂中。(備註：校訂密碼與 [!DNL Workfront] 密碼不相同。)


### [!UICONTROL 校訂活動]

此頁面會追蹤校訂上發生的所有活動，以及就此校訂傳送的電子郵件訊息。

![影像顯示校訂頁面的「[!UICONTROL 校訂活動]」區段，其中左側面板選單突顯標示「[!UICONTROL 校訂活動]」選項。](assets/proofing-activity-in-details.png)

「**[!UICONTROL 活動]**」區段會記錄各個註解與決定的時間戳記以及執行這些動作的使用者。此外，亦追蹤校訂工作流程階段的開始時間、收件者第一次開啟校訂的時間，以及其他校訂管理員或所有者想要知道的資訊。舉例來說，當您嘗試瞭解為何校訂工作流程階段從未啟動時，這些詳細資料會很有幫助。

「**[!UICONTROL 訊息]**」區段記錄電子郵件警報和訊息傳送給收件者的時間戳記、寄件者及訊息內容。在疑難排解中如果有人說他們沒有收到有關校訂的電子郵件時，這會很有用。 您可以檢查電子郵件是否以及何時發送。

Adobe建議校訂管理員和校訂所有者熟悉這兩個部分中的資訊。 當您擁有這些資訊而且知道如何閱讀 [!UICONTROL SOCD] 進度列時，便能真正瞭解及管理您的校訂，無論在校訂工作流程的哪個階段。

當您完成[!UICONTROL 檔案詳細資料]區段中的工作後，請使用階層連結追蹤回到附有校訂的專案、任務或問題的[!UICONTROL 檔案]區段。

![影像顯示標題有階層連結路徑。](assets/proof-breadcrumb.png)

<!--
#### Learn more
* [!UICONTROL Document details] overview
* Add a custom form to a document
* Request document approvals
* Summary for documents overview
* View activity on a proof within [!DNL Workfront]
-->
