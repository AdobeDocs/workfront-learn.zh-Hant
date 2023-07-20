---
title: 開始使用計算欄位和運算式
description: 瞭解如何在計算欄位中建立運算式，以收集有關貴組織所做工作的唯一自訂資料。
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: gs-calc-fields-expressions.png
exl-id: fbd17f01-9e97-4ead-9a56-7ce4f81255ec
source-git-commit: 409147f9a62302d28e14b834981992a0421d4e4b
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# 開始使用計算欄位和運算式

<!-- **Note**: The expression examples shown are simple and some may be mitigated by fields already supplied by  . However, the examples are used to illustrate the foundational knowledge needed in order to build expressions in Workfront.-->

Workfront提供多種跨多個業務領域通用的欄位，並經常用於工作管理。 計畫完成日期、專案預算、任務受指派人名稱等欄位。

然而，每個組織都有其特定產業和公司的資料，需要收集這些資料，以瞭解是否實現了公司的目標。 例如，您的組織想要追蹤：

* 專案將貢獻的業務領域。
* 如果資金來自供應商、內部或兩者。
* 使用的影像需要何種解析度。

雖然這些欄位本身並未內建於 [!DNL Workfront]，您可以建立自訂資料輸入欄位，並透過自訂表單預先填入多選答案欄位。

此學習路徑著重於計算欄位。 您將瞭解什麼是計算欄位、您可以透過資料運算式提取到計算欄位中的不同型別的資訊，以及如何建立這些計算欄位以增強您的資料收集和報告。

![資源管理設定一頁傳呼機](assets/GS01.png)

## 什麼是計算欄位？

計算欄位會存放使用資料運算式和現有Workfront欄位建立的自訂資料。

![具有使用率報告的工作負載平衡器](assets/GS02.png)

例如，您的組織有特定的專案編號或工作編號，系統包括：

* 建立專案的年份，
* 專案所有者的縮寫，以及
* 此 [!DNL Workfront] 專案參考編號。


在計算欄位中使用運算式時，您可以取得已儲存在中的每一項資訊 [!DNL Workfront] 並建立該唯一專案ID或工作編號，然後將其新增至報表，如下所示：

![具有使用率報告的工作負載平衡器](assets/GS03.png)

視需要的特定資料而定，計算欄位可能很簡單，使用一或兩個運算式，也可能更複雜，使用數個內嵌運算式。 請記住，Workfront只能將已儲存或提取至系統中的資料用於計算欄位。

## 文字運算式

文字運算式搜尋、剖析及合併資訊於 [!DNL Workfront] 以建立更有意義的資料，或深入瞭解組織所做工作。

例如，文字運算式可用於：

* 在專案檢視的欄中，當專案費用超過$5,000時顯示「超過$5,000」，或當費用低於該費用時顯示「低於$5,000」。

* 為每個專案指定一個唯一的數字，包括專案的建立年份、專案的  [!DNL Workfront] 參考編號、專案名稱和專案所有者的首字母。

* 建立一份報告，列出未指派給投資組合和/或方案的每個專案，以便您可以在經理會議中使用此報告。

文字運算式可用於自訂欄位，以在Workfront中進行這些型別的搜尋和組合。

檢視可能的文字運算式時，您會找到數個選項。

![資源管理設定一頁傳呼機](assets/TE01.png)

有六個文字運算式最常使用：

* CONCAT
* 左/右
* 包含
* IF
* ISBLANK