---
title: 建立基本篩選活動
description: 在此活動中，您將建立一個名為「我擁有的專案本月關閉」的專案篩選器。
activity: use
feature: Reports and Dashboards
thumbnail: 336807.jpeg
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8856
exl-id: fc29b4ce-2937-478e-abd5-0b559657ead0
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# 建立基本篩選活動

在本影片中，您將建立一個名為「本月結束的我擁有的專案」專案篩選器。 如果您正在密切關注許多專案，此篩選器可以幫助您放大即將關閉的專案。

以下包含逐步指示。

>[!VIDEO](https://video.tv.adobe.com/v/336807/?quality=12&learn=on)

## 答案

![建立新篩選器的畫面影像](assets/basic-filter-activity-updated-6-15-21.png)

1. 導覽至 [!UICONTROL 專案] 區域來自 [!UICONTROL 主要功能表]. 這會向您顯示專案清單。
1. 按一下 **[!UICONTROL 篩選]** 功能表並選取 **[!UICONTROL 新增篩選器]**.
1. 將您的篩選器命名為「本月關閉的我所擁有的專案」。
1. 按一下 **[!UICONTROL 新增篩選規則]**.
1. 在 [!UICONTROL 開始輸入欄位名稱] 欄位，輸入「owner」。 然後選取 [!UICONTROL 擁有者ID] 在 [!UICONTROL 專案] 欄位來源。
1. 離開 [!UICONTROL 等於] 運運算元。
1. 在開始輸入名稱欄位中輸入「$$」。
1. 選取 [!UICONTROL $$USER.ID]. 這是登入使用者的萬用字元。
1. 按一下 [!UICONTROL 新增篩選規則] 再來一次。
1. 在 [!UICONTROL 開始輸入欄位名稱] 欄位，開始輸入「完成」。 然後選取 [!UICONTROL 完成] 在「專案」欄位來源底下。
1. 離開 [!UICONTROL 等於] 運運算元。
1. 選取「假」。
1. 按一下 [!UICONTROL 新增篩選規則] 再來一次。
1. 在 [!UICONTROL 開始輸入欄位名稱] 欄位型別「計畫」，然後選取 [!UICONTROL 計畫完成日期] 在 [!UICONTROL 專案] 欄位來源。
1. 變更 [!UICONTROL 等於] 運運算元至 [!UICONTROL 本月].
1. 按一下 **[!UICONTROL 儲存篩選器]**
