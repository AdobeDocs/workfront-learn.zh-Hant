---
title: 探索Workfront中的專案時間表
description: 了解如何指派任務、使用甘特圖和關鍵路徑功能、透過視圖監控專案、有效安排任務排程以及套用限制，以實現最佳專案規劃。
activity: use
feature: Work Management
thumbnail: 335213.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
last-substantial-update: '2024-11-01T00:00:00.000Z'
recommendations: noDisplay,catalog
jira: KT-8953
exl-id: ba993197-9f84-4fc0-86cc-cf849c889f56
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T14:48:54.364Z'
source-git-commit: df1a568be7d42893910e1c0afde8bbba213a7803
workflow-type: tm+mt
source-wordcount: 700
ht-degree: 74%

---

# 探索Workfront中的專案時間表

學習內容：

* 概略了解使用 Workfront 進行專案規劃及管理的情形。 了解父系任務如何將數個子任務組成群組，而這些子任務會指派給各個工作角色，再指派給具備所需技能的使用者。 前置任務表示任務之間的順序關係，而沒有前置任務的任務則可以同時進行。 甘特圖提供視覺化時間軸，而關鍵路徑功能則會醒目標示出一旦有所延誤，將會影響專案進度的任務。
* Workfront 中的不同視圖，例如用於規劃的標準視圖以及用於監控進度的狀態視圖，其中包括進度、評論、文件、問題、核准、關鍵路徑以及里程碑的標幟。 可以追蹤最近的活動以查看更新和備註。
* 可以使用開始日期或完成日期來設定排程，Workfront 會根據任務持續時間及前置任務，自動計算相對應的日期。 影片建議從開始日期設定關鍵完成日期，以便預留一些寬限時間。 也會探討各種任務限制，例如「盡快」和「越晚越好」，說明這些限制如何影響任務排程。 可以建立自訂視圖來顯示任務限制。

>[!VIDEO](https://video.tv.adobe.com/v/3435846/?captions=chi_hant&quality=12&learn=on&enablevpops=1)

>[!IMPORTANT]
>
>有關期間類型和任務限制的完整說明，請參閱「[了解和管理期間類型和任務限制](/help/manage-work/intermediate-projects/understand-and-manage-duration-types-and-task-constraints.md)」。

## 關鍵重點

* **任務管理與指派：**&#x200B;父系任務會將數個子任務分組，這些子任務會指派給工作角色，並稍後再指派給具有必要技能的使用者。 前置任務&#x200B;表示循序關係，而沒有前置任務的工作可以並行完成。 
* **甘特圖與關鍵路徑：**&#x200B;甘特圖提供專案的視覺時間表，而關鍵路徑功能會醒目顯示可能延遲專案的工作（如果發生滑動）。 &#x200B;
* **視圖和監控：** Workfront 中的不同視圖，例如用於規劃的標準視圖以及用於監控進度的狀態視圖，其中包括進度、評論、文件、問題、核准、關鍵路徑和里程碑的標幟。 也可以追蹤最近的活動。 
* **排程選項：**&#x200B;專案可從開始日期或完成日期排程，Workfront會根據任務持續期間和前置任務計算對應的日期。 建議從開始日期開始排&#x200B;程重要完成日期，以允許一些寬限。 
* **任務限制：**&#x200B;如「儘快」和「儘可能遲」等任務限制會影響任務排程。 在專&#x200B;案建立後變更排程模式可能會影響任務限制和計畫日期。 可以建立&#x200B;自訂檢視來顯示任務限制。 


## 是否要更改專案時間軸上的日期…

| PROS (變更日期) | CONS (變更日期) | PROS (不變更日期) | CONS (不變更日期) |
|---------------------------|---------------------------|---------------------------|---------------------------|
| <ul><li>為使用者減輕壓力並提供最新的預期資訊：「_創作者無法掌握真實狀況_」</li><li>準確的資源分配，特別是在工作負載平衡器中的分配狀況</li><li>使用日誌項目報告 (或專案期間) 調出日期變更</li><li>使用條件顯示專案是否超出範圍</li><li>可以新增自訂表單 (或使用問題) 來追蹤變更——為什麼延遲、因誰而延遲、延遲多久</li></ul> | <ul></li><li>若將誤導性資料彙整成報告，就無法反映真實狀態</li><li>對進度的錯誤認知，會產生一切都按計劃進行的錯覺</li><li>形成一種總是延遲時間軸，而不是解決根本原因的文化</li><li>利害關係人失去信心/團隊自覺無法準時完成任務 </li></ul> | <ul></li><li>精確展現專案時間軸：資料可用於分析，並清楚描述發生的事情</li><li>可選擇更改期間，或新增延遲至前置任務</li><li>輕鬆找出未來專案規劃和風險管理流程的改進空間。</li><li>選擇善用基準線來取得原始專案計劃，並將其作為比較依據</li><li>若沒有充足的人力或資源，請不要啟動任務。</li></ul> | <ul></li><li>使用者感到困惑和/或沮喪，因為才剛收到任務通知，就看到大量的「延遲」任務</li><li>資源已依照原始計劃進行有效分派，但現在卻因延遲的任務增加了額外的負荷</li><li>專案時間軸無法用以向利害關係人清楚傳達最新資訊</li></ul> |


## 有關此主題的推薦教學課程

* [使用完成百分比和進度狀態追蹤進度](/help/manage-work/project-timelines/track-work-progress-from-the-project-timeline.md)
* [瞭解日期類型和進度狀態](/help/manage-work/project-timelines/understand-task-dates-and-progress-status.md)
* [主要期間型別和任務限制](/help/manage-work/intermediate-projects/understand-and-manage-duration-types-and-task-constraints.md)


