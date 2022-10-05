---
title: 建立自定義提示
description: 了解自訂提示是什麼、如何使用文字模式建立自訂提示，以及可在 [!DNL  Workfront].
activity: use
feature: Reports and Dashboards
thumbnail: 336822.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9087
exl-id: 1bb0832e-e888-4154-b78d-24c6d69f629f
source-git-commit: 83c7379a5398c78cea31a4571b34fd5b64bce027
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 2%

---

# 建立自定義提示

在此影片中，您將學習：

* 自定義提示是
* 如何使用文字模式建立自訂提示
* 您可在報表中使用的一些範例

>[!VIDEO](https://video.tv.adobe.com/v/336822/?quality=12)

## 活動：建立自定義提示

1. 建立自訂提示，在提示下拉式功能表中顯示下列專案狀態：
   * 計畫
   * 目前
   * 已完成
   * 廢棄
1. 修改提示，以顯示本月到期的目前專案。

## 答案

1. 您的自訂提示應類似於此，且具有下列文字模式：

   ![在文本模式中建立新篩選器的螢幕影像](assets/cp-01.png)

   儲存自訂提示後，提示下拉式功能表應如下所示：

1. 自訂提示中的文字模式應如下所示：

![在文本模式中建立新篩選器的螢幕影像](assets/cp-02.png)

```
   status=CUR&plannedCompletionDate=$$TODAYbm&plannedCompletionDate_Mod=between&plannedCompletionDate_Range=$$TODAYem 
```

而且，應更新作用中提示的下拉式標籤，以反映程式碼中的變更，如下所示：

![在文本模式中建立新篩選器的螢幕影像](assets/cp-02a.png)
