---
title: 建立自訂提示
description: 了解什麼是自訂提示、如何使用文字模式建立自訂是示，以及可供 Workfront 之報告功能使用的範例。
activity: use
feature: Reports and Dashboards
thumbnail: 336822.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
last-substantial-update: 2025-08-05T00:00:00Z
jira: KT-9087
exl-id: 1bb0832e-e888-4154-b78d-24c6d69f629f
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 99%

---

# 建立自訂提示

觀看這段影片，您將會了解：

* 什麼是自訂提示
* 如何使用文字模式來建立自訂提示
* 您可以在報告中使用的一些範例

>[!VIDEO] (https://video.tv.adobe.com/v/336822/?quality=12&learn=on&enablevpops=0

## 「建立自訂提示」活動


### 活動：建立自訂提示

1. 建立自訂提示並在提示下拉式選單中顯示下列專案狀態：
   * 計畫
   * 目前
   * 已完成
   * 廢棄
1. 修改提示以顯示本月到期的目前項目。

### 解答

1. 您的自訂提示應與下圖相似，且具有以下文字模式：

   ![影像顯示在文字模式中建立新篩選器的畫面](assets/cp-01.png)

   您儲存自訂提示之後，提示下拉式選單應如下所示：

1. 您的自訂提示中的文字模式應如下所示：

![影像顯示在文字模式中建立新篩選器的畫面](assets/cp-02.png)

```
   status=CUR&plannedCompletionDate=$$TODAYbm&plannedCompletionDate_Mod=between&plannedCompletionDate_Range=$$TODAYem 
```

使用中提示的下拉式標籤應該更新以反映程式碼的變更，如下所示：

![影像顯示在文字模式中建立新篩選器的畫面](assets/cp-02a.png)
