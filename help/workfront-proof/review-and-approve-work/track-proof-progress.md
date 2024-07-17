---
title: 追蹤校訂進度
description: 瞭解如何使用 [!UICONTROL SOCD] 指標、校訂進度和報告來追蹤  [!DNL  Workfront] 中的校訂進度。
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
source-wordcount: '675'
ht-degree: 100%

---

# 追蹤校訂進度

作為專案經理人、校訂管理員或檢閱與核准流程中的其他利害關係人，您想要追蹤校訂的進度。您可以在「[!UICONTROL 文件]」頁面使用 [!DNL Workfront’s] 內建的&#x200B;**校訂進度指標**，或是撰寫自訂報告來追蹤進度。

若要在 [!DNL Workfront] 檢視校訂進度，您必須具有「計劃」、「工作」或「檢閱」授權，而且是一位校訂使用者。若您不確定自己的 [!DNL Workfront] 設定檔是否符合這些需求，請諮詢貴組織的校訂系統管理員。

## 利用 [!UICONTROL SOCD] 指標和校訂狀態來追蹤校訂進度

使用「[!UICONTROL 文件]」清單中的 [!UICONTROL SOCD] 圖示，從高層次角度檢視校訂工作在檢閱與核准流程中的進度。這些圖示表示對校訂採取的特定動作。

![影像顯示 [!DNL  Workfront] 專案中「[!UICONTROL 文件]」清單，並且突顯標示 [!UICONTROL SOCD] 圖示。](assets/manage-proofs-socd.png)

這些圖示表示從您傳送校訂給收件者直到他們對校訂做出決定為止，在校訂上已完成的工作。

* **S —** 校訂已經傳送給收件者。
* **O —** 校訂已經開啟。
* **C —** 已在校訂上留下註解。
* **D —** 已針對校訂做出決定 (核准、拒絕等)。

顏色表示動作是否已經完成。

* **白色 —** 該步驟尚未執行。
* **綠色 —** 該步驟已經完成。
* **橘色 —** 校訂期限僅剩下 24 小時，而且該步驟並未執行。
* **紅色 —** 校訂期限已過，而且該步驟並未執行。

位在摘要面板的[!UICONTROL 文件]清單中，或是位在[!UICONTROL 文件詳細資料]中的 [!UICONTROL SOCD]，是校訂進度的高層次摘要。[!DNL Workfront] 根據校訂流程中「進度最慢」的收件者進行這項設定。

比如，若有三位檢閱者/核准者，而其中只有兩位看過校訂內容並留下註解，則 [!UICONTROL SOCD] 圖示會顯示校訂已傳送 ([!UICONTROL S]) 和已開啟 ([!UICONTROL O])，但是並未留下註解 ([!UICONTROL C])。

若您想要知道每位校訂收件者目前的進度，請開啟校訂工作流程。整體校訂進度顯示在視窗最上方。在灰色橫條可看見每個階段本身的進度指標。而每個使用者旁邊則顯示其個人進度。

![影像顯示文件的「[!UICONTROL 校訂工作流程]」區段。](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## 校訂狀態

校訂狀態是以該階段的校訂收件者之狀態為準。您可以在「[!UICONTROL 文件]」頁面，在 [!UICONTROL SOCD] 指標的右側看到整體校訂狀態，所以您可以輕鬆判斷校訂是否已有決定。

![影像顯示 [!DNL  Workfront] 專案的「[!UICONTROL 文件]」清單並突顯標示整體校訂狀態。](assets/manage-proofs-overall-status.png)

這個校訂狀態表示校訂的整體狀態。比如，有兩位收件者核准校訂，其個別狀態會顯示「[!UICONTROL 已核准]」但是，第三位收件者尚未做出決定，所以該名人員的狀態是「[!UICONTROL 待處理]」。因此整體狀態顯示為「[!UICONTROL 待處理]」。

若是您的組織已設定自訂狀態，則會顯示那些狀態。否則，您將會看到以下標準狀態選項：

* [!UICONTROL 待處理]
* [!UICONTROL 已核准]
* [!UICONTROL 已核准 (附帶變更)]
* [!UICONTROL 所需變更]
* [!UICONTROL 不相關]

開啟校訂工作流程視窗，查看被指派為「[!UICONTROL 檢閱者與核准者]」或「[!UICONTROL 核准者]」校訂角色的收件者之校訂狀態。

## [!DNL Workfront] 的報告

您還可以利用 [!DNL Workfront’s] 報告功能，追蹤校訂在檢閱與核准流程中的進度。

校訂核准報告協助您追蹤待完成的核准，以確保在截止期限前完成。

![影像顯示 [!DNL  Workfront] 中的校訂核准報告。](assets/proof-approval-report.png)

您可以利用文件版本報告來管理和追蹤校訂版本。

![影像顯示 [!DNL  Workfront] 中的文件版本。](assets/document-version-report.png)

我們建議與您的 [!DNL Workfront] 顧問一起合作，建立符合組織需求的報告。有些報告必須熟悉 [!DNL Workfront’s] 文字模式報告功能方能使用。

## 換您來操作

與您的團隊或校訂系統管理員討論，找出要在 Workfront 中使用哪一種報告以利維持校訂工作流程能順利進行。

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->
