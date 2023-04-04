---
title: 建立ADDDAYS、ADDWEEKDAY、ADDMONTHS、ADDYEARS運算式
description: 了解如何在Adobe的計算欄位中使用和建立ADD運算式 [!DNL Workfront].
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Experienced
activity: use
team: Technical Marketing
thumbnail: 335175.png
kt: 8912
exl-id: f194fbc8-99b3-4fed-9fc5-a2f5fa4593d2
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# 建立ADDDAYS、ADDWEEKDAY、ADDMONTHS、ADDYEARS運算式

在此影片中，您將學習：

* ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR運算式的計算方式
* 如何在計算欄位中建立ADDWEEKDAYS資料運算式

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12&learn=on)

## 其他範例

以下是Adobe Workfront客戶已建立的一些額外ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR運算式。

**本該由**

客戶想要根據實際起始日期和計畫持續時間了解任務何時應完成。 在此情況下，預計完成日期將不起作用，因為如果任務延遲，則它可以移動；如果先前任務延遲，計畫完成日期將不起作用。

建立的表達式為ADDDAYS({actualStartDate},{durationMinutes}/480)

持續時間欄位中的時間以分鐘為單位儲存。 因此，在此運算式中，如果時間要反映在天中，「持續時間」欄位不能獨立。 若要執行此動作，「持續時間」必須除以480分鐘（480分鐘= 8小時= 1天）

這就是為什麼第二個值槽包含(Duration/480)。


**發票完成日期**

此範例不僅包含使用ADDAYS運算式，也包含預先建立並儲存在自訂表單中的自訂欄位。

客戶正在通過名為「發票提交日期」的自定義日期欄位獲取發票提交日期。

發票提交後，必須在30天內完成並歸檔。 要自動生成完成和歸檔日期，將使用ADDDAYS計算欄位和「發票提交日期」自定義欄位。 運算式如下所示：

ADDDAYS（{DE：發票提交日期},30）
