---
title: 顯示休假會影響專案時間表
description: 檢視當休假設定開啟和關閉時專案時間表的情況。
feature: Resource Management
type: Tutorial
role: Leader, User
level: Intermediate, Experienced
activity: use
team: Technical Marketing
jira: KT-10180
exl-id: 0f79dd8d-b7ce-4ee9-b211-23c8ed5d497c
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 4%

---

# 休假如何影響專案時間表

指派使用者的休假是否會計入專案時間表，取決於名為的專案設定 [!UICONTROL 使用者休假]. 此設定決定任務的主要受指派人的休假是否調整專案上該任務的計畫日期。

讓我們看看選取每個設定時，專案時間表會發生什麼情況 — C[!UICONTROL 考量使用者在任務持續期間的休假] 或 [!UICONTROL 忽略使用者在任務持續期間的休假].

![使用者休假設定](assets/toapt_01.png)

## 考量使用者在任務持續期間的休假

此選項是Workfront的預設設定。

在此範例中，任務的主要受指派人在他們的個人行事曆上有標示的休假。

![個人行事曆](assets/toapt_02.png)

專案經理想要將此人指派給計畫日期與使用者的休假重疊的任務。

![具有日期的專案任務](assets/toapt_03.png)

當此使用者指派到任務時，計畫日期會自動調整。 現在，任務的計畫完成日期已延長數天，以適應使用者的休假。 請務必注意，此變更可能會影響專案中其他任務的計畫日期，並可能影響專案的計畫完成日期。

![具有到期日的專案任務](assets/toapt_04.png)

## [!UICONTROL 忽略使用者在任務持續期間的休假]

透過此選項，任務的計畫日期保持與原始計畫相同，即使主要受指派人在任務持續期間具有休假。

團隊成員在其行事曆上標示了休假。

![具有已標籤關閉日期的pto行事曆](assets/toapt_05.png)

專案經理會指派與休假重疊的任務。 指派使用者後，任務計畫日期將維持原計畫。

![調整專案任務日期](assets/toapt_06.png)

為確保工作按時完成，當原始受指派人不在辦公室時，指派另一位可處理此任務的人可能會有所幫助。

## 調整專案層級的設定

若要變更專案的「使用者休假」設定：

* 在Workfront中按一下專案名稱以開啟專案。

* 選取 [!UICONTROL 編輯] 從頁首的3點選單，到專案名稱的右側。

* 捲動至 [!UICONTROL 專案設定] 區段並尋找 [!UICONTROL 使用者休假] 欄位。

* 選取您要套用至此專案的選項 —  [!UICONTROL 考量使用者在任務持續期間的休假] 或I[!UICONTROL 遺漏使用者在任務持續期間的休假].

* 按一下 [!UICONTROL 儲存] 按鈕。

![考量使用者在任務持續期間的休假](assets/toapt_07.png)


**注意**：此設定在選取時無法使用 [!UICONTROL 專案詳細資訊] 從專案頁面的左側面板選單。

全域設定存在於的專案偏好設定中 [!UICONTROL 設定] 功能表。 此設定由您的系統管理員管理。 群組管理員或許可以針對他們管理的群組調整此設定。

Workfront建議將此設定設為您希望組織內大部分專案處理休假的方式。

您也可以透過範本詳細資訊，將此設定內建到專案範本中。
