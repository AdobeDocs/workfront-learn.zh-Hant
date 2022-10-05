---
title: 如何追蹤校樣進度
description: 了解如何使用 [!UICONTROL SOCD] 指標、證明進度和報告，以追蹤證明的進度 [!DNL  Workfront].
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: track-proof-progress.png
kt: 10111
exl-id: 343483fe-487a-4a23-914d-2807a00630f9
source-git-commit: 1f7a4da813805691fc0e52d3ad1ea708f9e07a9a
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 1%

---

# 追蹤校樣進度

身為專案經理、證明經理或審核與核准程式中的其他利害關係人，您會想要追蹤證明的進度。 您可以透過 [!DNL Workfront’s] 內建 **證明進度指標** 在 [!UICONTROL 檔案] 頁面或撰寫自訂報表。

要查看校樣進度，請在 [!DNL Workfront]，您必須擁有「計畫」、「工作」或「審核」許可證，並且是校對用戶。 如果你不確定 [!DNL Workfront] 配置檔案符合這些要求，請與貴組織的校對系統管理員聯繫。

## 使用追蹤校樣進度 [!UICONTROL SOCD] 指標和證明狀態

從高層了解通過審核和批准流程(使用 [!UICONTROL SOCD] 表徵圖 [!UICONTROL 檔案] 清單。 這些圖示表示對校樣採取的特定動作。

![的影像 [!UICONTROL 檔案] 清單 [!DNL  Workfront] 專案 [!UICONTROL SOCD] 表徵圖。](assets/manage-proofs-socd.png)

這些圖示會指出從您將校樣傳送給收件者，到他們決定校樣時，校樣所完成的工作。

* **S —** 校樣已傳送給收件者。
* **O —** 校樣已經開啟。
* **C —** 已對證據發表評論。
* **D —** 已對校樣（核准、拒絕等）做出決定。

顏色會指出動作是否完成。

* **懷特 —** 步驟還沒發生。
* **綠色 —** 步驟已完成。
* **橙色 —** 證明截止時間在24小時內，且步驟尚未發生。
* **紅色 —** 校樣截止日期已過，而步驟尚未發生。

此 [!UICONTROL SOCD] 在 [!UICONTROL 檔案] 清單、摘要面板或 [!UICONTROL 文檔詳細資訊]，是證明進度的高階摘要。 [!DNL Workfront] 根據校對程式中「最落後」的收件者來設定。

例如，如果有三個審核者/批准者，其中只有兩個審核者查看了校樣並發表了評論，則 [!UICONTROL SOCD] 圖示會顯示已傳送校樣([!UICONTROL S])和開啟([!UICONTROL O])，但並未提供評論([!UICONTROL C])。

如果您想要了解每個校樣收件者的運作方式，請開啟校樣工作流程。 整體校樣進度位於視窗頂端。 每個階段在灰條中都有其自己的進度指標。  每個使用者旁邊就是個人的進度。

![的影像 [!UICONTROL 校對工作流程] 的子句。](assets/manage-proofs-socd-in-proofing-workflow-window.png)

## 校樣狀態

校樣狀態是根據階段校樣收件者的狀態。 整體校樣狀態會顯示在 [!UICONTROL 檔案] 頁面，位於 [!UICONTROL SOCD] 指標，因此您可以輕鬆判斷是否對證明有決定。

![的影像 [!UICONTROL 檔案] 清單 [!DNL  Workfront] 會強調顯示整體校樣狀態的專案。](assets/manage-proofs-overall-status.png)

此校樣狀態表示校樣的整體狀態。 例如，如果兩個收件者核准了校樣，其個別狀態會顯示 [!UICONTROL 已核准]. 不過，第三個收件者尚未作出決定，因此該人的狀態為 [!UICONTROL 待定]. 因此，整體狀態顯示為 [!UICONTROL 待定].

如果您的組織已設定自訂狀態，系統將會使用這些狀態。 否則，您會看到下列標準狀態選項：

* [!UICONTROL 未決]
* [!UICONTROL 已核准]
* [!UICONTROL 變更已核准]
* [!UICONTROL 所需變更]
* [!UICONTROL 不相關]

開啟校對工作流程視窗，查看指派給的收件者的校樣狀態 [!UICONTROL 審核者與核准者] 或 [!UICONTROL 核准者 ]校樣角色。

## 報表於 [!DNL Workfront]

您也可以運用 [!DNL Workfront’s] 報告功能，可在校樣在審核和核准程式中移動時追蹤校樣。

校樣核准報表可協助您追蹤未完成的核准，以確保符合期限。

![校樣核准報表的影像，位於 [!DNL  Workfront].](assets/proof-approval-report.png)

文檔版本報告允許您管理和跟蹤校樣版本。

![檔案版本報表的影像，位於 [!DNL  Workfront].](assets/document-version-report.png)

建議您使用 [!DNL Workfront] 顧問，以建立符合貴組織需求的報表。 有些報表需要熟悉 [!DNL Workfront’s] 文本模式報告。

## 該你了

請洽詢您的團隊或校對系統管理員，了解您將在Workfront中使用哪種報表，以確保校樣工作流程順利執行。

<!--
### Learn more
* Learn to create reports in [!DNL Workfront] with the Basic Report Creation course.
* View progress and status of a proof
* View activity on a proof within [!DNL Workfront]
-->
