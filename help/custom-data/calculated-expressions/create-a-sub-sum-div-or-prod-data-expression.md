---
title: 建立SUB、SUM、DIV或PROD資料表達式
description: 了解如何在Adobe的計算欄位中使用和建立基本數學運算式 [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335177.png
kt: 8914
exl-id: e767b73b-1591-4d96-bb59-2f2521e3efa3
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 0%

---

# 建立SUB、SUM、DIV或PROD資料表達式

在此影片中，您將學習：

* SUB、SUM、DIV和PROD表達式的作用
* 如何在計算欄位中建立SUB資料運算式

>[!VIDEO](https://video.tv.adobe.com/v/335177/?quality=12)

## 其他資訊：ROUND運算式

### 建立ROUND表達式

ROUND表達式採用任何數字，並將其四捨五入到特定數量的小數位數。

大多數情況下，ROUND資料表達式與其他資料表達式一起使用，並且格式欄位保留為「文本」或「數字」。

讓我們建立一個計算欄位，以確定計畫小時數和實際登入任務的小時數之間的差異，這需要SUB運算式，如下所示：

**SUB({workRequired},{actualWorkRequired})**

由於時間是以分鐘為單位來追蹤，且偏好的格式是以小時為單位來顯示資訊，因此運算式也需要除以60，如下所示：

**DIV(SUB({workRequired},{actualWorkRequired}),60)**

如果在自訂表單中建置計算欄位時，格式變更為「數字」，則在檢視中新增欄位時，您可以變更數字格式。

![具有利用率報告的工作負載平衡器](assets/round01.png)

不過，如果建立自訂欄位時的欄位格式保留為「文字」，則無法在檢視中輕鬆變更格式。 必須使用ROUND運算式，才能避免在專案中看到類似以下的數字：

![具有利用率報告的工作負載平衡器](assets/round02.png)

<b>在計算欄位中使用ROUND資料表達式</b>

ROUND表達式包括表達式的名稱(ROUND)，通常包括兩個資料點。 這些資料點可以是Workfront中的運算式或欄位，後面接著數字，指出您要前往多少個小數位數。

運算式的結構如下：ROUND（資料點， #）

在計算計畫小時數與實際小時數之差的表達式中，將此表達式 — DIV(SUB({workRequired},{actualWorkRequired}),60) — 用作第一個資料點。 然後，確定該運算式產生的數字在小數點右側不超過2位。

![具有利用率報告的工作負載平衡器](assets/round03.png)

表達式可以寫成如下：ROUND(DIV(SUB({workRequired},{actualWorkRequired}),60),2)。
