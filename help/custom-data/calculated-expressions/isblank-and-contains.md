---
title: 使用ISBLANK和CONTAINS運算式
description: 瞭解如何在Adobe的計算欄位中使用和建立ISBLANK和CONTAINS運算式 [!DNL Workfront].
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: isblank-contains.png
exl-id: 819ffec8-e7e6-4a3c-a589-1348aa09e27d
source-git-commit: 409147f9a62302d28e14b834981992a0421d4e4b
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# 使用ISBLANK和CONTAINS運算式

CONTAINS和ISBLANK運算式都用來提供簡單的true或false值。 差別在於ISBLANK運算式會檢查欄位是否保留值，而CONTAINS文字運算式會尋找欄位中的特定字串。

例如，若要檢視專案是否有說明，請使用ISBLANK運算式。 如果說明欄位為空白，運算式會傳回true值。 如果說明欄位非空白，則會傳回false值。

![具有使用率報告的工作負載平衡器](assets/isblank01.png)

若要在說明中尋找特定值（例如「慈善活動」），請使用CONTAINS文字運算式。 如果在說明中找到「慈善活動」，則計算欄位會顯示「true」。 如果找不到「慈善活動」，則會顯示「false」。

![具有使用率報告的工作負載平衡器](assets/isblank02.png)

## ISBLANK

ISBLANK文字運算式包含運算式名稱和一個資料點。

**ISBLANK({data point})**

![具有使用率報告的工作負載平衡器](assets/isblank03.png)

在上述範例中（您想要知道專案是否有說明），運算式會是：

ISBLANK({description})

## 包含

CONTAINS文字運算式包含運算式名稱、您要尋找的字詞或片語，以及要尋找的欄位。

**CONTAINS(「片語」，{fields})**

請務必在尋找的字詞或片語兩側加上引號，否則運算式將無效。

在上述範例中（在專案說明中尋找「慈善事件」），運算式會是：

**CONTAINS(&quot;charity event&quot;，{description})**

![具有使用率報告的工作負載平衡器](assets/isblank04.png)

**注意**： CONTAINS運算式區分大小寫。 例如，如果「慈善事件」在說明欄位中大寫，請在運算式中大寫該片語。

**CONTAINS(「慈善活動」，{description})**

如果您想要檢視值是否存在，最好同時使用ISBLANK和CONTAINS運算式。 不過，知道該值是什麼、實際檢視它或擁有某種描述項以提供更好的深入分析可能更有用。

例如，您不想只知道專案已從請求轉換，而是想知道原始請求的名稱。

在這種情況下，請搭配使用CONTAINS運算式和IF運算式。

ISBLANK和CONTAINS文字運算式經常搭配IF文字運算式使用。
