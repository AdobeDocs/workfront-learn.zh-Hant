---
title: 說明休假如何影響專案時間表
description: 瞭解休假設定開啟或關閉對專案時間表的影響。
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
ht-degree: 100%

---

# 休假如何影響專案時間表

受指派的使用者的休假是否影響專案時間表，取決於稱為「[!UICONTROL 使用者休假]」的專案設定。這項設定決定是否根據任務主要受指派人的休假來調整該專案任務的規劃日期。

來瞭解選取以下各項設定時專案時間表會有什麼變動 -「[!UICONTROL 考量使用者在任務期間的休假]」或是「[!UICONTROL 忽略使用者在任務期間的休假]」。

![使用者休假設定](assets/toapt_01.png)

## 考量使用者在任務期間的休假

此選項是 Workfront 的預設設定。

在此範例中，任務的主要受指派人在其個人行事曆上標記了休假時間。

![個人行事曆](assets/toapt_02.png)

專案經理人想要對這名人員指派任務，但任務的規劃日期與使用者的休假時間重疊。

![附帶日期的專案任務](assets/toapt_03.png)

當這位使用者被指派任務時，規劃日期會自動調整。現在，任務的規劃完成日期為了配合使用者的休假已延長幾天。請務必注意，這項變更可能會影響專案中其他任務的規劃日期，並可能影響專案的規劃完成日期。

![附有截止日期的專案任務](assets/toapt_04.png)

## [!UICONTROL 忽略使用者在任務期間的休假]

使用此選項，任務的規劃日期將保持不變，即使主要受指派人在該任務期間有休假也是如此。

團隊成員在其行事曆上標記休假時間。

![附有標記日期的 PTO 行事曆](assets/toapt_05.png)

專案經理人指派給他們的任務與休假時間重疊。在指派使用者之後，任務的規劃日期維持原始設定。

![調整專案任務日期](assets/toapt_06.png)

為確保準時完成工作，在原始受指派人休假期間指派可以執行任務的另一名人員會有所幫助。

## 調整專案層級的設定

若要變更專案的「使用者休假」設定：

* 在 Workfront 中按一下專案名稱來開啟專案。

* 在專案名稱右側的頁面標題三圓點選單中選取「[!UICONTROL 編輯]」。

* 捲動到「[!UICONTROL 專案設定]」區段並尋找「[!UICONTROL 使用者休假]」欄位。

* 選取您要套用到此專案的選項 —「[!UICONTROL 考量使用者在任務期間的休假]」或「[!UICONTROL 忽略使用者在任務期間的休假]」

* 按一下視窗右上角的「[!UICONTROL 儲存]」按鈕。

![考量使用者在任務期間的休假](assets/toapt_07.png)


**備註**：當您在專案頁面的左側面板選單中選取「[!UICONTROL 專案詳細資料]」時，無法使用這個設定。

您可以透過「[!UICONTROL 設定]」選單的專案偏好設定，用全域設定的形式完成這項設定。這項設定由您的系統管理員管理。群組管理員可以為所管理的群組調整此設定。

Workfront 建議按照您希望組織中大多數專案處理休假的方式來進行設定。

相關設定也可以透過範本詳細資料內建到專案範本中。
