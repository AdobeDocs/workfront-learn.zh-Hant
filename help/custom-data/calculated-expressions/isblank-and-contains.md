---
title: 使用 ISBLANK 和 CONTAINS 運算式
description: 瞭解如何在Adobe [!DNL Workfront]的計算欄位中使用和建立ISBLANK和CONTAINS運算式。
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: isblank-contains.png
exl-id: 819ffec8-e7e6-4a3c-a589-1348aa09e27d
TQID: 'https://experienceleague.adobe.com/q25cuV-wKAkoEJTzDIho1Ab-XTexGhEZCHReoE0TFxg'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
    internal-label: Leader
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
source-git-commit: 54883ad8c8df3aaee06ba8f8dca64227594c1c77
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 93%
---
# 使用 ISBLANK 和 CONTAINS 運算式

CONTAINS 和 ISBLANK 運算式都用於提供簡單的 true 或 false 值。 兩者的區別在於 ISBLANK 運算式檢查欄位是否含有任何值，而 CONTAINS 文字運算式則是在欄位中搜尋特定字串。

例如，要查看專案是否有說明，請使用 ISBLANK 運算式。 如果說明欄位是空白，則運算式會傳回 true 值。 如果說明欄位不是空白，則會傳回 false 值。

![附帶使用情況報告的工作負載平衡器](assets/isblank01.png)

要在說明中搜尋特定值，例如「charity event」，請使用 CONTAINS 文字運算式。 若是在說明中找到「charity event」，則計算欄位表示「true」。 若是沒有找到「charity event」，則顯示「false」。

![附帶使用情況報告的工作負載平衡器](assets/isblank02.png)

## ISBLANK

ISBLANK 文字運算式包括運算式的名稱及一個資料點。

**ISBLANK({data point})**

![附帶使用情況報告的工作負載平衡器](assets/isblank03.png)

在上述範例中，您想要知道專案是否有說明，則運算式如下：

ISBLANK({description})

## CONTAINS

CONTAINS 文字運算式包含運算式的名稱、您要搜尋的字詞或短句，以及要搜尋的欄位。

**CONTAINS(&quot;phrase&quot;，{fields})**

在要搜尋的字詞或短句前後必須加上引號，否則便不是有效的運算式。

在上述範例 (在專案說明中搜尋「charity event」) 中，運算式如下：

**CONTAINS(&quot;charity event&quot;，{description})**

![附帶使用情況報告的工作負載平衡器](assets/isblank04.png)

**備註**：CONTAINS 運算式區分大小寫。 例如，如果「Charity Event」在說明欄位中有大寫字母，在運算式中的短句也要使用大寫。

**CONTAINS(&quot;Charity Event&quot;，{description})**

若您想要搜尋是否存在某個值，則 ISBLANK 和 CONTAINS 運算式皆適用。 但是，知道該值是什麼意思、看到實際的值或是擁有某些描述項來提供更深入的洞察，可能更有用處。

例如，您不只是想要知道專案是從請求轉換而來，而是想要知道原始請求的名稱。

在這種情況下，請使用 CONTAINS 運算式結合 IF 運算式。

ISBLANK 和 CONTAINS 文字運算式經常與 IF 文字運算式一起使用。
