---
title: 超越基本對應
description: 了解如何使用對應面板公式來操控或轉換傳送至模組的欄位。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: 11039
thumbnail: KT11039.png
exl-id: 979d794d-b936-402e-b07c-71e999f40780
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---

# 超越基本對應

了解如何使用對應面板公式來操控或轉換傳送至模組的欄位。

## 練習概觀

使用「對應」面板公式，從「基本對應以外」逐步練習中變更專案名稱、計劃開始日期和優先順序。

![超出基本映射映像1](../12-exercises/assets/beyond-basic-mapping-walkthrough-1.png)

## 遵循步驟

**複製初始藍本設計案例。**

1. 在方案部分中，選擇初始方案設計右側的克隆選項，如下所示。 將其命名為「超出基本對應」。

   ![超出基本映射映像2](../12-exercises/assets/beyond-basic-mapping-walkthrough-2.png)

   **現在，我們將使用建立Workfront專案模組中的對應面板，設定專案名稱、計劃開始日期和優先順序欄位。**

1. 按一下「建立Workfront專案」模組以編輯設定。 使用映射面板，將「名稱」欄位更改為「[我的專案名稱] by [贊助商].&quot;

   + 此 [我的專案名稱] 是剖析CSV模組的第1欄，而 [贊助商] 是欄6。 「by」這個詞只是在兩者之間輸入。

1. 接著前往「計劃開始日期」，使用addDays公式將15天新增至欄位，如「超出基本對應」逐步影片所述。
1. 找到「優先順序」欄位，並切換欄位右上角的「對應」按鈕。 選擇清單菜單更改為數字。 如果CSV檔案信賴等級小於100，則建立if陳述式，將專案標示為高(4)優先順序，否則可設為一般(2)。

   + 信賴等級在第4欄。

   **此時，您的對應面板應如下所示：**

   ![超出基本映射影像3](../12-exercises/assets/beyond-basic-mapping-walkthrough-3.png)

1. 按一下「確定」，然後按一下「運行一次」。
1. 在您的Workfront例項中尋找專案，以確定所有項目皆已正確對應。
1. 儲存您的藍本。
