---
title: 建立ADDDAYS、ADDWEEKDAY、ADDMONTHS、ADDYEARS運算式
description: 瞭解如何在Adobe的計算欄位中使用和建立ADD運算式 [!DNL Workfront].
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335175.png
jira: KT-8912
exl-id: f194fbc8-99b3-4fed-9fc5-a2f5fa4593d2
doc-type: video
source-git-commit: 409147f9a62302d28e14b834981992a0421d4e4b
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# 建立ADDDAYS、ADDWEEKDAY、ADDMONTHS、ADDYEARS運算式

在本影片中，您將瞭解：

* ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR運算式計算的內容
* 如何在計算欄位中建立ADDWEEKDAYS資料運算式

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12&learn=on)

## 其他範例

以下是Adobe Workfront客戶建立的額外ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR運算式。

**應該完成日期**

客戶想要根據實際開始日期和計畫期間知道任務何時應該完成。 在此情況下，「預計完成日期」無法運作，因為如果任務延遲，它就會移動，而如果先前任務有延遲，「計畫完成日期」則無濟於事。

建立的運算式為ADDDAYS({actualStartDate}，{durationMinutes}/480)

「持續時間」欄位中的時間會以分鐘為單位儲存。 因此，在此運算式中，如果時間要反映為天，則Duration欄位不能獨立。 為此，持續時間必須除以480分鐘（480分鐘= 8小時= 1天）

這就是第二個值位置包含(Duration/480)的原因。


**商業發票完成日期**

此範例不僅包含使用ADDDAYS運算式，還包含先前以自訂表單建立和儲存的自訂欄位。

客戶透過名為「商業發票提交日期」的自訂日期欄位，擷取提交商業發票的日期。

提交後，必須在30天內完成並存檔商業發票。 若要自動產生完成和歸檔日期，會使用ADDDAYS計算欄位與「發票提交日期」自訂欄位。 運算式看起來像這樣：

ADDDAYS（{DE：發票提交日期}，30）
