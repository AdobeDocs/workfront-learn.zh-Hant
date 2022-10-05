---
title: 使用ISBLANK和CONTAINS運算式
description: 了解如何在Adobe的計算欄位中使用和建立ISBLANK和CONTAINS運算式 [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: isblank-contains.png
exl-id: 819ffec8-e7e6-4a3c-a589-1348aa09e27d
source-git-commit: 2b9a31b45ff94222a77c05292ee5b9d8229f5f0b
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# 使用ISBLANK和CONTAINS運算式

CONTAINS和ISBLANK運算式都用來提供簡單的true或false值。 區別在於，當CONTAINS文本表達式在欄位內查找特定字串時，ISBLANK表達式會檢查欄位是否完全保留值。

例如，要查看項目是否有說明，請使用ISBLANK表達式。 如果說明欄位空白，運算式會傳回true值。 如果說明欄位不空白，則會傳回false值。

![具有利用率報告的工作負載平衡器](assets/isblank01.png)

若要在說明中尋找特定值（例如「慈善活動」），請使用CONTAINS文字運算式。 如果在說明中找到「慈善活動」，則計算欄位會顯示「true」。 如果找不到「慈善活動」，則會顯示「false」。

![具有利用率報告的工作負載平衡器](assets/isblank02.png)

## ISBLANK

ISBLANK文本表達式包含表達式的名稱和一個資料點。

**ISBLANK（資料點）**

![具有利用率報告的工作負載平衡器](assets/isblank03.png)

在上述範例中（您想知道專案是否有說明的位置），運算式會是：

ISBLANK（說明）

## 包含

CONTAINS文本表達式包括表達式的名稱、要查找的單詞或短語以及要查找的欄位。

**CONTAINS(&quot;phrase&quot;,field)**

請務必在您要尋找的字詞或片語周圍加上引號，否則運算式將無效。

在上述範例中（在專案說明中尋找「慈善活動」），運算式會是：

**CONTAINS(&quot;charity event&quot;,Description)**

![具有利用率報告的工作負載平衡器](assets/isblank04.png)

**附註**:CONTAINS運算式區分大小寫。 例如，如果「慈善活動」在說明欄位中大寫，請在運算式中大寫該片語。

**CONTAINS(&quot;Charity Event&quot;,Description)**

如果您想查看是否有值，則ISBLANK和CONTAINS運算式都適合使用。 但是，知道值是什麼、實際看到它或者有某種描述詞來提供更好的洞察力，可能會更有用。

例如，您並不想只知道專案已從請求中轉換，而想知道原始請求的名稱。

在這種情況下，請使用CONTAINS表達式和IF表達式。

ISBLANK和CONTAINS文本表達式通常與IF文本表達式一起使用。
