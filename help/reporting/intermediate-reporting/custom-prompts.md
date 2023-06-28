---
title: 建立自訂提示
description: 瞭解自訂提示是什麼、如何使用文字模式建立自訂提示，以及可以在Workfront的報表中使用的一些範例。
activity: use
feature: Reports and Dashboards
thumbnail: 336822.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-9087
exl-id: 1bb0832e-e888-4154-b78d-24c6d69f629f
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 2%

---

# 建立自訂提示

在本影片中，您將瞭解：

* 什麼是自訂提示
* 如何使用文字模式建立自訂提示
* 您可在報告中使用的一些範例

>[!VIDEO](https://video.tv.adobe.com/v/336822/?quality=12&learn=on)

## 活動：建立自訂提示

1. 建立自訂提示，在提示下拉式選單中顯示以下專案狀態：
   * 計畫
   * 目前
   * 已完成
   * 廢棄
1. 修改提示以顯示本月到期的目前專案。

## 答案

1. 您的自訂提示應類似此，並具有以下文字模式：

   ![在文字模式中建立新濾鏡的熒幕影像](assets/cp-01.png)

   儲存自訂提示後，提示下拉式選單應如下所示：

1. 自訂提示中的文字模式應如下所示：

![在文字模式中建立新濾鏡的熒幕影像](assets/cp-02.png)

```
   status=CUR&plannedCompletionDate=$$TODAYbm&plannedCompletionDate_Mod=between&plannedCompletionDate_Range=$$TODAYem 
```

而且應該更新作用中提示的下拉式清單標籤，以反映程式碼中的變更，如下所示：

![在文字模式中建立新濾鏡的熒幕影像](assets/cp-02a.png)
