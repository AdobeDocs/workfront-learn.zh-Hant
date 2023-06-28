---
title: 追蹤校訂進度
description: 瞭解如何使用 [!UICONTROL SOCD] 用於追蹤中校訂進度的指標、校訂進度和報告 [!DNL  Workfront].
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: track-proof-progress.png
jira: KT-10111
exl-id: 343483fe-487a-4a23-914d-2807a00630f9
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 1%

---

# 追蹤校訂進度

身為專案經理、校樣經理或稽核及核准流程中的其他利害關係人，您將想要追蹤校樣進度。 您可以透過以下方式執行此操作： [!DNL Workfront’s] 內建 **校訂進度指示器** 於 [!UICONTROL 檔案] 頁面或撰寫自訂報表。

若要檢視中校訂進度 [!DNL Workfront]，您必須擁有計畫、工作或檢閱授權且為校訂使用者。 如果您不確定 [!DNL Workfront] 設定檔符合這些要求，請洽詢您組織的校訂系統管理員。

## 透過以下專案追蹤校訂進度 [!UICONTROL SOCD] 指標和校訂狀態

透過，以高階方式瞭解校訂如何通過檢閱和核准流程 [!UICONTROL SOCD] 圖示於 [!UICONTROL 檔案] 清單。 這些圖示會指出對校樣執行的特定動作。

![的影像 [!UICONTROL 檔案] 清單于 [!DNL  Workfront] 專案與 [!UICONTROL SOCD] 圖示會反白顯示。](assets/manage-proofs-socd.png)

圖示會指出對校訂完成的工作，從您將校訂傳送給收件者到他們對校訂做出決定為止。

* **S —** 校樣已傳送給收件者。
* **O —** 校訂已開啟。
* **C —** 已對此校訂進行評論。
* **D —** 證明已做出決定（已核准、已拒絕等）。

這些顏色表示動作是否完成。

* **白色 —** 步驟尚未發生。
* **綠色 —** 步驟已完成。
* **橙色 —** 校訂截止日期在24小時內，並且步驟尚未發生。
* **紅色 —** 校訂截止日期已過，該步驟尚未發生。

此 [!UICONTROL SOCD] 於 [!UICONTROL 檔案] 清單、摘要面板或 [!UICONTROL 檔案詳細資訊]是校訂進度的高階摘要。 [!DNL Workfront] 根據在校樣程式中「最落後」的收件者來設定此設定。

例如，如果有三名稽核者/核准者，且只有兩名稽核者/核准者檢視過校樣並發表了評論，則 [!UICONTROL SOCD] 圖示會顯示校樣已傳送([!UICONTROL S])和已開啟([!UICONTROL O])，但並未進行評論([!UICONTROL C])。

如果您想知道每個個別校樣收件者的表現，請開啟校樣工作流程。 整體校訂進度位於視窗頂端。 灰色列中的每個階段都有自己的進度指示器。  而在每個使用者旁邊，是該個人的進度。

![的影像 [!UICONTROL 校訂工作流程] 檔案的區段。](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## 校訂狀態

校訂狀態以階段校訂收件者的狀態為基礎。 整體校訂狀態可見於 [!UICONTROL 檔案] 頁面，右側 [!UICONTROL SOCD] 指標，以便您輕鬆判斷您是否對校訂有決策。

![的影像 [!UICONTROL 檔案] 清單于 [!DNL  Workfront] 突出顯示整體校訂狀態的專案。](assets/manage-proofs-overall-status.png)

此校訂狀態代表校訂的整體狀態。 例如，如果兩個收件者核准證明，則其個別狀態會顯示 [!UICONTROL 已核准]. 但是，第三個收件者尚未做出決定，因此該人員的狀態為 [!UICONTROL 擱置中]. 因此，整體狀態會顯示為 [!UICONTROL 擱置中].

如果貴組織配置了自訂狀態，則會使用這些狀態。 否則，您將會看到下列的標準狀態選項：

* [!UICONTROL 未決]
* [!UICONTROL 已核准]
* [!UICONTROL 變更已核准]
* [!UICONTROL 所需變更]
* [!UICONTROL 不相關]

開啟校訂工作流程視窗以檢視指派的收件者的校訂狀態 [!UICONTROL 檢閱者和核准者] 或 [!UICONTROL 核准者]校訂角色。

## 中的報表 [!DNL Workfront]

您也可以善用 [!DNL Workfront’s] 報告功能，可在校樣通過稽核和核准程式時進行追蹤。

校訂核准報告可幫助您追蹤未完成的核准，以確保遵守截止日期。

![中的校訂核准報告影像 [!DNL  Workfront].](assets/proof-approval-report.png)

檔案版本報告可讓您管理和追蹤校訂版本。

![中的檔案版本報表影像 [!DNL  Workfront].](assets/document-version-report.png)

我們建議您與您的 [!DNL Workfront] 顧問，建立符合您組織需求的報告。 部分報表需先熟悉 [!DNL Workfront’s] 文字模式報告。

## 輪到你了

請洽詢您的團隊或校訂系統管理員，以瞭解您將在Workfront中使用何種報告，讓校訂工作流程順暢運作。

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->
