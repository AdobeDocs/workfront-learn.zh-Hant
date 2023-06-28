---
title: 瞭解校訂詳細資訊
description: 深入瞭解中校訂背後的詳細資訊 [!DNL  Workfront] 透過「摘要」面板和 [!UICONTROL 檔案詳細資訊] 頁面。
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Beginner
thumbnail: understand-proof-details.png
jira: KT-10110
exl-id: 196f9318-eced-4825-b0fd-8592b6cb3403
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1029'
ht-degree: 0%

---

# 瞭解校訂詳細資訊

## 檢視校訂詳細資訊

作為校訂管理員或所有者，您可以透過摘要面板和 [!UICONTROL 檔案詳細資訊] 頁面。 首先，請在中找到您的證明 [!UICONTROL 檔案] 專案、任務或問題的區段。

### 摘要面板

摘要面板提供校樣基本詳細資訊的高層級概觀。 需要時可使用圖示來展開面板，不需要時則摺疊面板。您甚至可以暫留在校樣縮圖上以開啟或下載它。

![的影像 [!UICONTROL 檔案] 已選取校樣並展開摘要面板的專案區段。 摘要面板圖示和摘要面板都會反白顯示。](assets/document-summary.png)

注意： [!UICONTROL 核准] 摘要面板中的區段是 **檔案** 核准和 **不是** 繫結至您在本課程中瞭解的校訂檢閱和核准流程。 這兩個程式在中是分開的 [!DNL Workfront].

### [!UICONTROL 文件詳細資訊]

如果您需要有關校訂的詳細資訊，請 [!UICONTROL 檔案詳細資訊] 連結會帶您前往中的校樣「頁面」 [!DNL Workfront].

![中校訂頁面的影像 [!DNL  Workfront].](assets/document-details.png)

請務必注意，檢視校訂程式相關資訊的能力取決於您在中的校訂許可權 [!DNL Workfront].

從校樣頁面，您可以從左側面板選單存取這些區段：

* **更新 —** 校樣檢視器中所做的評論會顯示在這裡，並帶有「校樣評論」標籤。 您也可以對檔案進行註解，就像對任務或專案進行註解一樣（這些註解不會出現在校樣檢視器中）。
* **核准 —** 此區段用於檔案核准，而不是校訂核准。 這兩種核准型別是中不同的程式 [!DNL Workfront] 並且不要連結在一起。 如果您正在將校訂工作流程用於審查和核准，則不會使用此區段。
* **所有版本 —** 追蹤及管理校訂的版本記錄。 您可能會發現在 [!UICONTROL 檔案] 清單。
* **自訂Forms —** 自訂表單用於校樣以擷取組織特定資訊。 此資訊可與檔案一起傳遞至整合式檔案儲存系統，例如 [!DNL Workfront] DAM或 [!DNL Adobe’s] AEM。 自訂表單由您的設定 [!DNL Workfront] 系統管理員或群組管理員。 請洽詢您的團隊或管理員，瞭解您是否會使用校樣上的自訂表格。
* **校訂工作流程 —** 管理或修改指派給校訂的工作流程。 您可以使用以下工具開啟此視窗： [!UICONTROL 校訂工作流程] 中校訂上的連結 [!UICONTROL 檔案] 清單。 瞭解如何使用編輯校樣工作流程影片變更工作流程。

讓我們來進一步瞭解以下兩個區段： [!UICONTROL 校訂檢視器設定] 和 [!UICONTROL 校訂活動].

### [!UICONTROL 校訂檢視器設定]

這些設定可協助您控制對校樣本身的存取。

![的影像 [!UICONTROL 校訂檢視器設定] 從校訂的頁面，使用 [!UICONTROL 校訂檢視器設定] 選項在左側面板選單中反白顯示。](assets/proofing-settings-on-details-page.png)

* **[!UICONTROL 需要登入. 此校訂無法與訪客使用者共用] —** 只有具備下列條件的人才能共用校訂： [!DNL Workfront] 校訂授權。
* **[!UICONTROL 需要以電子方式簽署決定] —** 共用校訂時，這要求收件者擁有中的校訂許可權 [!DNL Workfront] 並透過在做出校樣決定時輸入校樣密碼來讓他們「以電子方式簽署」校樣。 (注意：校訂密碼與您的密碼不同， [!DNL Workfront] 密碼。 校訂密碼不易存取，因此大多數收件者不會知道此密碼。) [!DNL Workfront] 建議與您的 [!DNL Workfront] 使用此功能之前的顧問。
* **[!UICONTROL 完成所有必要的決定時鎖定校訂]—** 一旦對校訂做出每個決定，這會將校訂鎖定到任何進一步的評論、回覆、決定等。 這會鎖定整個校訂版本，而不僅僅是校訂工作流程的特定階段。
* **[!UICONTROL 允許下載原始檔案] —** 校樣收件者可以從校樣檢視器（右側面板選單中的選項）下載校樣的原始來源檔案。
* **[!UICONTROL 允許透過公開URL或內嵌程式碼共用校訂] —** 校訂收件者可與任何人共用公開存取的校訂連結。
* **[!UICONTROL 允許透過公開URL或內嵌程式碼訂閱校訂] —** 任何人只要收到公開URL，都可以使用其電子郵件地址和名稱（如果不是校訂使用者）或電子郵件地址和校訂密碼（如果是校訂使用者）將自己新增到校訂中。 (注意：校訂密碼與 [!DNL Workfront] 密碼。)

在中上傳校樣時，可以設定這些相同的設定 [!UICONTROL 校訂設定] 區段，位於上傳視窗底部。

![的影像 [!UICONTROL 校訂設定] 區段。](assets/proof-settings-on-upload-page.png)

### [!UICONTROL 校訂活動]

此頁面追蹤校樣上發生的所有活動，以及就此校樣傳送的電子郵件訊息。

![的影像 [!UICONTROL 校訂活動] 具有的校樣頁面的區段 [!UICONTROL 校訂活動] 選項在左側面板選單中反白顯示。](assets/proofing-activity-in-details.png)

此 [!UICONTROL 活動] 區段時間戳記何時做出評論和決定，以及誰做出這些決定。 它也會追蹤校訂工作流程階段何時開始、收件者何時首次開啟校訂，以及校訂管理員或校訂所有者希望瞭解的其他資訊。 例如，當您嘗試弄清楚為什麼驗證工作流程階段從未啟動時，這些詳細資料可能會很有幫助。

此 [!UICONTROL 訊息] 區段時間戳記（電子郵件警示和訊息傳送至收件者、傳送者及訊息內容時）。 如果有人說他們沒有收到有關校訂的電子郵件，這在疑難排解時可能很有用。 您可以檢查是否及何時傳送電子郵件。

[!DNL Workfront] 建議校訂管理員和校訂所有者熟悉這兩個部分中的資訊。 當您結合此資訊並瞭解如何閱讀 [!UICONTROL SOCD] 進度列，無論校樣工作流程中的哪個位置，您都能真正瞭解和管理校樣。

一旦您完成使用 [!UICONTROL 檔案詳細資訊] 區段，使用階層連結路徑返回 [!UICONTROL 檔案] 證明附加到的專案、任務或問題的區段。

![標題中階層連結軌跡的影像。](assets/proof-breadcrumb.png)

<!--
#### Learn more
* [!UICONTROL Document details] overview
* Add a custom form to a document
* Request document approvals
* Summary for documents overview
* View activity on a proof within [!DNL Workfront]
-->
