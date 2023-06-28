---
title: 建立SUB、SUM、DIV或PROD資料運算式
description: 瞭解如何在Adobe的計算欄位中使用和建立基本的數學運算式 [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335177.png
jira: KT-8914
exl-id: e767b73b-1591-4d96-bb59-2f2521e3efa3
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 0%

---

# 建立SUB、SUM、DIV或PROD資料運算式

在本影片中，您將瞭解：

* SUB、SUM、DIV和PROD運算式的功能
* 如何在計算欄位中建立SUB資料運算式

>[!VIDEO](https://video.tv.adobe.com/v/335177/?quality=12&learn=on)

## 其他資訊： ROUND運算式

### 建立ROUND運算式

ROUND運算式會取用任何數字，並將其四捨五入為特定數量的小數位數。

大多數情況下，ROUND資料運算式會與其他資料運算式搭配使用，且格式欄位會保留為「文字」或「數字」。

讓我們建立一個計算欄位，以決定計畫與實際登入任務的時數之間的差異，這需要使用SUB運算式，看起來像這樣：

**SUB({workRequired}，{actualWorkRequired})**

由於時間是以分鐘追蹤，且偏好格式是以小時顯示資訊，因此運算式也需要除以60，如下所示：

**DIV(SUB({workRequired}，{actualWorkRequired})，60)**

如果在自訂表單中建立計算欄位時格式變更為數字，則可以在檢視中新增欄位時變更數字格式。

![具有使用率報告的工作負載平衡器](assets/round01.png)

但是，如果在建立自訂欄位時欄位格式保留為文字，則無法輕鬆地在檢視內變更格式。 ROUND運算式必須用來避免在您的專案中看到類似這樣的數字：

![具有使用率報告的工作負載平衡器](assets/round02.png)

<b>在計算欄位中使用ROUND資料運算式</b>

ROUND運算式包含運算式名稱(ROUND)，通常包含兩個資料點。 這些資料點可以是Workfront中的運算式或欄位，後面接著數字表示您要前往的小數位數。

運算式的結構如下： ROUND(data point， #)

在計算計畫和實際時數之間差異的運算式中，使用此運算式 — DIV(SUB({workRequired}，{actualWorkRequired})，60) — 作為第一個資料點。 然後請確定該運算式所得的數字不會在小數右邊超過2位。

![具有使用率報告的工作負載平衡器](assets/round03.png)

運算式可以寫成如下形式： ROUND(DIV(SUB({workRequired}，{actualWorkRequired})、60)、2)。
