---
title: 開始使用計算欄位和運算式
description: 了解如何在計算欄位中建立運算式，以收集有關貴組織所完成工作的唯一自訂資料。
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: gs-calc-fields-expressions.png
exl-id: fbd17f01-9e97-4ead-9a56-7ce4f81255ec
source-git-commit: f81d156b4058bec70bc3256efda6f85746f0f625
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# 開始使用計算欄位和運算式

<!-- **Note**: The expression examples shown are simple and some may be mitigated by fields already supplied by  . However, the examples are used to illustrate the foundational knowledge needed in order to build expressions in Workfront.-->

Workfront提供多種在多個業務領域都很常見的欄位，並經常用於工作管理。 諸如計畫完成日期、項目預算、任務受託人名稱等欄位。

然而，每個組織都有其行業和公司的特定資料，需要收集這些資料，以了解公司目標是否實現。 例如，您的組織想要追蹤：

* 專案將貢獻哪項業務。
* 如果資金來自供應商、內部或兩者。
* 所用影像需要什麼解析度。

雖然這些欄位並非內建在 [!DNL Workfront]，您可以透過自訂表單建立自訂資料輸入欄位，以及預先填入、多選答案欄位。

此學習路徑著重於計算欄位。 您將了解計算欄位是什麼、您可以透過資料運算式提取至計算欄位的不同資訊類型，以及如何建立這些計算欄位以增強資料收集和報告功能。

![資源管理設定一個尋呼機](assets/GS01.png)

## 什麼是計算欄位？

計算欄位會儲存使用資料運算式和現有Workfront欄位建立的自訂資料。

![具有利用率報告的工作負載平衡器](assets/GS02.png)

例如，您的組織具有特定的項目編號或工作編號系統，包括：

* 在項目建立之年，
* 項目所有者的縮寫，以及
* 此 [!DNL Workfront] 項目參考編號。


在計算欄位中使用運算式，您可以擷取已儲存在 [!DNL Workfront] 並建立唯一的專案ID或工作編號，然後可以像這樣新增至報表：

![具有利用率報告的工作負載平衡器](assets/GS03.png)

根據需要的特定資料，使用一或兩個運算式或使用數個內嵌運算式時，計算欄位可能會比較簡單，或更複雜。 請記住，Workfront只能將已儲存或提取至系統中的資料用於計算欄位。

## 文字運算式

文字運算式搜尋、剖析及結合 [!DNL Workfront] 以建立更有意義的資料，或深入了解貴組織所完成的工作。

例如，文字運算式可用於：

* 在項目費用超過$5,000時顯示「超過$5,000」；在項目視圖的列中顯示費用低於$5,000時顯示「低於$5,000」。

* 為每個專案指定一個唯一編號，包含專案的建立年份、專案的  [!DNL Workfront] 參考編號、項目名稱和項目所有者的縮寫。

* 建立報告，列出未指派給產品組合及/或方案的每個專案，以便您在經理會議中使用。

文字運算式可用於自訂欄位，以在Workfront中執行這些類型的搜尋和組合。

查看可能的文字運算式時，您會找到數個選項。

![資源管理設定一個尋呼機](assets/TE01.png)

最常使用的文字運算式有6種：

* CONCAT
* 左/右
* 包含
* IF
* ISBLANK