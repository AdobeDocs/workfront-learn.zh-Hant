---
title: 超出基本對應
description: 瞭解如何使用對應面板公式來操作或轉換傳送至模組的欄位。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11039
thumbnail: KT11039.png
exl-id: 979d794d-b936-402e-b07c-71e999f40780
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# 超出基本對應

瞭解如何使用對應面板公式來操作或轉換傳送至模組的欄位。

## 練習概述

使用對應面板公式，從「超出基本對應」逐步解說練習中變更專案名稱、規劃開始日期和優先順序。

![超出基本對應影像1](../12-exercises/assets/beyond-basic-mapping-walkthrough-1.png)

## 要遵循的步驟

**仿製您的初始案例設計案例。**

1. 在情境區段中，選取初始情境設計右側的「原地複製」選項，如下所示。 將其命名為「Beyond basic mapping」。

   ![超出基本對應影像2](../12-exercises/assets/beyond-basic-mapping-walkthrough-2.png)

   **現在，我們將使用「建立Workfront專案」模組中的對應面板，來設定專案名稱、規劃開始日期和優先順序欄位。**

1. 按一下「建立Workfront專案」模組以編輯設定。 使用對應面板，將名稱欄位變更為&quot;[我的專案名稱] 作者： [贊助者].」

   + 此 [我的專案名稱] 是「剖析CSV」模組中的欄1，且 [贊助者] 為欄6。 輸入字詞「by」時，只會在兩者之間輸入。

1. 接著，前往計劃開始日期，並使用addDays公式將15天新增至欄位，如超出基本對應逐步解說影片中所述。
1. 找到「優先順序」欄位，並切換欄位右上角的「對應」按鈕。 挑選清單功能表會變更為數字。 如果CSV檔案信賴評等低於100，請建立if陳述式以將專案標示為高(4)優先順序，否則可為正常(2)。

   + 信賴評等位於欄4中。

   **此時，您的對應面板應如下所示：**

   ![超出基本對應影像3](../12-exercises/assets/beyond-basic-mapping-walkthrough-3.png)

1. 按一下「確定」，然後按一下「執行一次」。
1. 在您的Workfront例項中尋找專案，確認所有專案皆正確對應。
1. 儲存您的案例。
