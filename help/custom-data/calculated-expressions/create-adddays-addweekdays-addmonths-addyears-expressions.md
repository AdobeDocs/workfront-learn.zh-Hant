---
title: 建立 ADDDAYS、ADDWEEKDAY、ADDMONTHS、ADDYEARS 運算式
description: 瞭解如何在 Adobe  [!DNL Workfront] 的計算欄位中使用和建立 ADD 運算式。
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
source-git-commit: d17df7162ccaab6b62db34209f50131927c0a532
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 100%

---

# 建立 ADDDAYS、ADDWEEKDAY、ADDMONTHS、ADDYEARS 運算式

觀看這段影片，您將會瞭解：

* ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR 運算式計算什麼
* 如何在計算欄位中建立 ADDWEEKDAYS 資料運算式

>[!VIDEO](https://video.tv.adobe.com/v/335175/?quality=12&learn=on&enablevpops)

## 其他範例

以下是 Adobe Workfront 客戶建立的一些其他 ADDDAYS/ADDWEEKDAY/ADDMONTHS/ADDYEAR 運算式。

**應該完成的期限**

客戶想要知道，根據「實際開始日期」和「規劃期間」，任務應該何時完成。在這種情況下，「預計完成日期」並不適用，因為如果任務延遲，這個日期可能會變動，而如果之前的任務有所延遲，則「規劃完成日期」亦無法派上用場。

所建立的運算式是 ADDDAYS({actualStartDate},{durationMinutes}/480)

儲存在「期間」欄位的時間以分鐘為單位。因此，在此運算式中，如果時間要以天數為單位，則「期間」不能是獨立的欄位。因此，「期間」必須除以 480 分鐘 (480 分鐘 = 8 小時 = 1 天)

這就是第二個值槽包含 (Duration/480) 的原因。


**發票完成日期**

此範例不但使用 ADDDAYS 運算式，還使用之前建立並儲存在自訂表單中的自訂欄位。

客戶透過標題為「發票提交日期」的自訂日期欄位取得發票提交的日期。

發票提交後，必須在 30 天內完成並歸檔。為了自動產生完成和歸檔日期，ADDDAYS 計算欄位與「發票提交日期」自訂欄位一起使用。運算式如下所示：

ADDDAYS({DE:Invoice Submission Date},30)
