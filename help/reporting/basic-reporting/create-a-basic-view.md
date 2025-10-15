---
title: 建立基本視圖
description: 了解在 Workfront 中什麼是視圖、如何建立視圖，以及如何與其他使用者共用視圖。
activity: use
feature: Reports and Dashboards
thumbnail: 335148.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
last-substantial-update: 2025-06-06T00:00:00Z
jira: KT-8854
exl-id: ba3c0e10-dcf1-4a7b-bf11-ccfed9040e6d
doc-type: video
source-git-commit: cc423944628d01e16d390842ecb25696505f923c
workflow-type: tm+mt
source-wordcount: '976'
ht-degree: 75%

---

# 建立基本視圖

影片說明如何在Workfront中建立和自訂檢視，以顯示清單中專案的特定資訊，例如專案、任務、問題和檔案。&#x200B;URL 檢視可讓使用者檢視詳細資訊，例如名稱、說明、狀態，以及與專案相關的其他欄位。&#x200B;URL

影片強調Workfront檢視的彈性，並提供建立、自訂及管理檢視的逐步指示。

>[!VIDEO](https://video.tv.adobe.com/v/3450249/?captions=chi_hant&quality=12&learn=on&enablevpops=0)

## 關鍵重點

* **自訂檢視**：使用者可以新增、移除或重新排列欄以顯示特定資訊，例如專案狀態或預算，以編輯現有檢視或建立新檢視。
* **內嵌編輯**：清單檢視中的某些欄位可以直接更新，而不需要開啟個別專案，因此變更的速度更快。&#x200B;URL
* **從頭開始建立檢視**：使用者可以透過新增預算、實際成本和進度狀態等相關欄，來設計檢視以滿足特定需求，例如追蹤專案狀況。&#x200B;URL
* **共用及管理檢視**：自訂檢視可與團隊成員共用，以進行共同作業，或在不再需要自訂檢視時移除。

## 「建立基本視圖」活動


### 活動 1：建立任務狀態視圖

作為專案經理人、團隊領導者或資源管理員，您想要追蹤任務工作的進展。透過這個視圖，您可以看到任務的數個狀態指標以清單或報告的形式全部排列顯示。

建立名為「任務狀態視圖」的任務視圖且包含下列欄：

* [!UICONTROL 任務名稱]
* [!UICONTROL 指派]
* [!UICONTROL 期間]
* [!UICONTROL 完成百分比]
* [!UICONTROL 狀態]
* [!UICONTROL 進度狀態]
* [!UICONTROL 狀態圖示]

### 解答 1

![影像顯示建立任務狀態視圖的畫面](assets/view-exercise.png)

1. 在任務清單報告中，前往「**[!UICONTROL 視圖]**」下拉式選單並選取「**[!UICONTROL 新增視圖]**」。
1. 將您的視圖命名為「任務狀態視圖」。
1. 移除這些欄：「[!UICONTROL 規劃時數]」、「[!UICONTROL 前置任務]」、「[!UICONTROL 開始日期]」和「[!UICONTROL 到期日]」。
1. 按一下「**[!UICONTROL 新增欄]**」。
1. 在「[!UICONTROL 在此欄中顯示]」欄位中，輸入「[!UICONTROL 狀態]」，然後在「任務」欄位來源之下選取「狀態」。
1. 再按一下「**[!UICONTROL 新增欄]**」。
1. 在「[!UICONTROL 在此欄中顯示]」欄位中，輸入「狀態」，然後在「[!UICONTROL 任務]」欄位來源之下選取「進度狀態」。
1. 再按一下「**[!UICONTROL 新增欄]**」。
1. 在「[!UICONTROL 在此欄中顯示]」欄位中，輸入「狀態」，然後在「任務」欄位來源之下選取「狀態圖示」。
1. 按一下「**[!UICONTROL 儲存]**」。

將游標懸停在「[!UICONTROL 狀態圖示]」欄的每個圖示上來看看他們代表的狀態。如果圖示呈現灰色，則表示該任務沒有備註、文件、核准流程等。如果圖示顯示顏色，則至少有一個項目與該任務關聯。您可以按一下備註或文件圖示前往該項目。

### 活動 2：建立里程碑視圖

如果您使用里程碑，此檢視是在工作清單中依名稱檢視里程碑，並使用內嵌編輯在工作中新增或移除里程碑的最簡單方式。

建立一個名為「里程碑視圖」的任務視圖且包含下列欄：

* [!UICONTROL 任務名稱]
* [!UICONTROL 指派]
* [!UICONTROL 期間]
* [!UICONTROL 計畫小時]
* [!UICONTROL 里程碑：名稱]
* [!UICONTROL 開始日期]
* [!UICONTROL 到期日]
* [!UICONTROL 完成百分比]


### 解答 2

![影像顯示建立里程碑視圖的畫面](assets/view-milestone-exercise-1.png)

1. 在專案任務清單中，前往「**[!UICONTROL 視圖]**」下拉式選單並選取「**[!UICONTROL 新增視圖]**」。
1. 將您的視圖命名為「里程碑視圖」。
1. 按一下「[!UICONTROL 前置任務]」欄來選取前置任務。
1. 在「[!UICONTROL 在此欄顯示]」欄位中，按一下「[!UICONTROL 任務>>前置任務]」欄位中的「減號」圖示，然後輸入「[!UICONTROL 里程碑名稱]」並按一下清單中的「[!UICONTROL 名稱]」。
1. 按一下「**[!UICONTROL 儲存]**」。

![影像顯示使用里程碑視圖的任務清單](assets/view-milestone-exercise-2.png)

### 活動 3：建立期間類型和任務限制視圖

您可以利用此視圖檢查和編輯專案中所有期間類型和任務限制。

建立名為「期間類型和任務限制視圖」的任務視圖並包含下列欄：

* [!UICONTROL 任務名稱]
* [!UICONTROL 指派]
* [!UICONTROL 期間]
* [!UICONTROL 規劃期間]
* [!UICONTROL 計畫小時]
* [!UICONTROL 前置任務]
* [!UICONTROL 開始日期]
* [!UICONTROL 到期日]
* [!UICONTROL 期間類型]
* [!UICONTROL 任務限制]
* [!UICONTROL 限制日期]

變更「[!UICONTROL 開始日期]」和「[!UICONTROL 到期日]」欄的「[!UICONTROL 欄位格式]」以便同時顯示日期和時間。

### 解答 3

![影像顯示畫面中顯示時間類型和任務限制視圖](assets/view-activity-3.png)

1. 在專案任務清單中，前往「**[!UICONTROL 視圖]**」下拉式選單並選取「**[!UICONTROL 新增視圖]**」。
1. 將您的視圖命名為「期間類型與任務限制視圖」。
1. 移除「[!UICONTROL 完成百分比]」欄。
1. 按一下「**[!UICONTROL 新增欄]**」。
1. 在「[!UICONTROL 在此欄中顯示]」欄位，輸入「[!UICONTROL 期間]」然後在「[!UICONTROL 任務]」欄位來源之下選取「[!UICONTROL 規劃期間]」。
1. 將這一欄移動到「[!UICONTROL 期間]」和「[!UICONTROL 規劃時數]」欄之間。
1. 再按一下「**[!UICONTROL 新增欄]**」。
1. 在「[!UICONTROL 在此欄中顯示]」欄位，輸入「[!UICONTROL 期間類型]」然後在「[!UICONTROL 任務]」欄位來源之下選取「[!UICONTROL 期間類型]」。
1. 再按一下「**[!UICONTROL 新增欄]**」。
1. 在「[!UICONTROL 在此欄中顯示]」欄位中，輸入「[!UICONTROL 限制]」然後在「任務」欄位來源之下選取「[!UICONTROL 任務限制]」。
1. 再按一下「**[!UICONTROL 新增欄]**」。
1. 在「[!UICONTROL 在此欄中顯示]」欄位中，輸入「[!UICONTROL 限制]」然後在「任務」欄位來源之下選取「[!UICONTROL 限制日期]」。
1. 選取「[!UICONTROL 開始日期]」欄，然後按一下「[!UICONTROL 進階選項]」。
1. 在[!UICONTROL 欄位格式]下拉式清單中，選取[!UICONTROL &quot;10/17/60 3:00 AM&quot;]。
1. 選取「[!UICONTROL 到期日]」欄，然後按一下「[!UICONTROL 進階選項]」。
1. 在[!UICONTROL 欄位格式]下拉式清單中，選取[!UICONTROL &quot;10/17/60 3:00 AM&quot;]。
1. 按一下「**[!UICONTROL 儲存]**」。

### 活動 4：建立專案範本使用中狀態視圖

任何管理專案範本的人都會喜歡看到清單中每個範本使用中狀態 (True 或 False)。更好的是 - 該欄位是行間可編輯欄位！

建立一個名為「標準+使用中狀態」的專案範本視圖，且包含以下欄：

* [!UICONTROL 名稱]
* [!UICONTROL 所有者]
* [!UICONTROL 期間]
* [!UICONTROL 規劃時數]
* [!UICONTROL 規劃成本]
* [!UICONTROL 標幟]
* [!UICONTROL 群組名稱]
* [!UICONTROL 使用中]


### 解答 4

![顯示專案範本使用中狀態視圖的螢幕影像](assets/view-activity-4.png)

1. 在專案範本清單中，前往「**[!UICONTROL 視圖]**」下拉式選單並選取「**[!UICONTROL 新增視圖]**」。
1. 將您的視圖命名為「標準+使用中狀態」。
1. 按一下「**[!UICONTROL 新增欄]**」。
1. 在「[!UICONTROL 在此欄中顯示]」欄位中，輸入「使用」後選取「使用中」 (在「[!UICONTROL 範本]」欄位來源中)。
1. 按一下「**[!UICONTROL 儲存視圖]**」。
