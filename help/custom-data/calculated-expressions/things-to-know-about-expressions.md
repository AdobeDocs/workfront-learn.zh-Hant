---
title: 關於計算欄位運算式的應知事項
description: 快速瀏覽有助於在  [!DNL Workfront] 中使用自訂計算欄位的一系列概念。
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: to-know-expressions.png
exl-id: 512a3071-f47f-4fd4-bf5f-9b18bef8ba59
source-git-commit: 409147f9a62302d28e14b834981992a0421d4e4b
workflow-type: ht
source-wordcount: '959'
ht-degree: 100%

---

# 關於計算欄位運算式的應知事項

瞭解以下這些概念，對於您在 Workfront 中使用自訂計算欄位會有幫助。

## 運算式名稱的大小寫非常重要

若是運算式的名稱，則大小寫很重要。在一開始寫出運算式名稱時，您可以使用大寫、小寫或是兩者混合。

![運算式名稱沒有區分大小寫的錯誤訊息](assets/T2K01.png)

但是，運算式必須全部使用大寫字母，系統才能辨識該運算式並儲存該欄位。



## 時數以分鐘為儲存單位

Workfront 資料庫中的時數以分鐘為儲存單位。如果您參照「規劃時數」或「實際時數」等欄位，數字請除以 60，用小時而非分鐘來顯示時間。

## 空格不影響運算式

編寫運算式的建議方法是各運算式之間極少使用或完全不使用空格。

* IF(ISBLANK({description}),&quot;No Description&quot;,&quot;Has Description&quot;)

![欄位之間沒有空格的運算式](assets/T2K02.png)

但是，如果空格可以幫助您理解運算式，您可以在運算式中加入一些空格。額外的空格不應妨礙運算式收集或計算 [!DNL Workfront] 中的值。

* IF (ISBLANK ({description}), &quot;No Description&quot; , &quot;Has Description&quot; )

![運算式的欄位之間有空格](assets/T2K03.png)

欄位和捲曲引號之間不可以有空格。否則，您會收到錯誤消息，並且無法儲存欄位或自訂表單。

![欄位名稱與捲曲引號之間有空格的錯誤](assets/T2K04.png)

## 必須使用直式引號

在運算式中使用引號時，請務必使用直式引號 (&quot;)。若是使用捲曲引號 (&quot;)，[!DNL Workfront] 系統會繼續顯示「自訂運算式無效」的訊息。

![弧型引號錯誤](assets/T2K05.png)

## 儲存表單和編輯物件時更新計算

這是我們應該瞭解的關於計算欄位的重要層面。

顯示在計算欄位的資訊將會維持不變並變成過時，除非重新計算自訂表單。

使用物件上「更多」選單的「重新計算運算式」選項便可以重新整理運算式。

您想要查看一個問題開啟的天數。使用運算式 DATEDIFF 建立一個稱為「Days Open」的計算欄位。

* Field Name = Days Open
* Expression = DATEDIFF({entryDate},$$TODAY)

儲存後，問題首次建立或輸入到 Workfront 的時間到今天日期之間的天數，可以顯示在物件的詳細資料頁面或是報告視圖中。

在隔天檢視相同的詳細資料頁面或報告視圖時，您預計該數字會遞增一個單位。如果今天的數字是 5，則明天應該是 6。第二天應該是 7，接著是 8 等。

然後該欄位將每天繼續顯示為 5。該欄位必須「重新執行」或重新計算以便重新整理資訊。

要使用「重新計算運算式」選項來更新欄位：

* 按一下物件的名稱來開啟。
* 按一下「更多」選單。
* 從清單中選取「重新計算運算式」。

![在物件中的「重新計算運算式」選項](assets/T2K06.png)

您也可以使用清單或報告中的「大量編輯」功能，同時重新計算多個運算式。假設您建立了一份報告，顯示一份問題清單，其中一欄顯示「Days Open」的計算。若要馬上重新計算全部問題：

* 選取報告中所有問題。
* 選取編輯選項，對所選問題進行大量編輯。
* 按一下左邊的「自訂表單」標籤，向下捲動至自訂表單區段。
* 勾選「自訂表單」區段底部的「重新計算自訂運算式」方塊。
* 按一下「儲存變更」。

![多個物件的重新計算運算式選項](assets/T2K07.png)

螢幕重新整理以便顯示計算欄位的更新資訊。

**備註**：雖然尚有其他方法可以更新或重新計算計算欄位的運算式，這是最快且最簡單的方法。

## 每個表單中相同欄位的計算可能不相同

計算欄位儲存到自訂表單，而且自訂表單亦已儲存之後，計算欄位會新增到「欄位資料庫」，以供其他表單使用。

但是，如果表單 A 上有一個計算欄位，而且表單 B 上有相同的計算欄位，則一開始的想法是計算會完全相同。情況並非總是如此。表單 A 上計算欄位的計算方式可能與表單 B 截然不同。

從欄位資料庫選取計算自訂欄位並新增到自訂表單時，新增了該欄位但計算卻是空白。這個情況的其中一個原因，是計算可能參考另一個物件類型中不存在的欄位。

例如，您建立一個計算欄位「Days to Complete」，以判斷專案中完成一項任務需要多少時間。

* WEEKDAYDIFF({actualStartDate},{actualCompletionDate})

您想要在一個疊代中執行完全相同的計算。您可以使用相同的運算式；但是任務物件的可用欄位並不一定永遠可供疊代物件使用。所以 [!DNL Workfront] 讓您有機會使用正確的物件欄位來建立計算。

**專家提示**：建立自訂欄位時，把「計算」方塊中的計算運算式複製到「指示」欄位。把一個計算自訂欄位新增到欄位資料庫的自訂表單時，這個欄位不會被刪除。

根據需求，自訂表單的計算欄位可能很簡單或是非常複雜。運算式可以內嵌或套疊其他運算式和值，以便提供更多的詳細資料，讓您更加瞭解貴組織所執行工作的現況。

<!--Depending on the need, calculated fields in custom forms can be quite simple or very complex. Expressions can embed, or nest, other expressions and values to provide the level of detail needed to get a better picture of what is going on with the work being done at your organization. 

Most of the examples and exercises in this course have been relatively simple to provide a base understanding of the expressions most commonly used and how to build those expressions in a custom calculated field. 

Now you're ready to start building your own calculated custom fields.-->
