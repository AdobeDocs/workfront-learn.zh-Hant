---
title: 了解分組的基本文字模式
description: 了解哪些文字模式、駝峰式大小寫，以及一些基本的「即插即用」文字模式，可在Workfront的分組中使用。
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 11369
exl-id: 5f45c64f-a22b-4983-91fd-9a1939f99fb1
source-git-commit: 818ee105af32589cb0e297e6f419a4a449a60052
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# 了解分組的基本文字模式

>[!IMPORTANT]
>
>必要條件：
>
>* 了解報表元素
>* 了解報表元件
>* 建立基本分組


>[!TIP]
>
>* 若要更深入了解文字模式，建議您觀看錄影的網路研討會活動 [詢問專家 — 文字模式報表簡介](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=en)，長度為一小時。
>* 若要進一步了解文字模式，建議您觀看 [進階報表](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) 教學課程，總共需要5.5小時。


在此影片中，您將學習：

* 什麼是文字模式
* 駝峰是什麼
* 您可在群組中使用一些基本的「即插即用」文字模式

>[!VIDEO](https://video.tv.adobe.com/v/3410641/?quality=12)

## 任務 — 4個父組

以下文本模式將根據最多四個父級對任務進行分組，並將不存在的父級留空。

```
textmode=true
group.0.name=Parents
group.0.valueexpression=CONCAT({parent}.{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{name}),"",", "),IF(ISBLANK({parent}.{name}),"No parent",{parent}.{name}))
group.0.linkedname=parent
group.0.namekeyargkey.0=parent
group.0.namekeyargkey.1=name
group.0.valueformat=string
```

![顯示按4個父項分組的項目任務的螢幕影像](assets/4-parents-grouping.png)


## 任務 — 完成百分比分組

下列文字模式會根據工作完成百分比來分組工作。 分組後，任務將分為以下類別之一：

* 0%
* 1%至25%
* 26%至50%
* 51%至75%
* 76%至99%
* 100%

```
group.0.linkedname=direct
group.0.namekey=percentComplete
group.0.valueexpression=IF({percentComplete}<1,"0%",IF({percentComplete}<26,"1% to 25%",IF({percentComplete}<51,"26% to 50%",IF({percentComplete}<76,"51% to 75%",IF({percentComplete}<100,"76% to 99%",IF({percentComplete}=100,"100","***"))))))
group.0.valueformat=doubleAsString
textmode=true
```

![顯示依完成百分比分組的專案工作的螢幕影像](assets/percent-complete-grouping.png)

## 任務 — statusAccussWith，然後是status

以下文本模式將按statusEqualsWith，然後按status對任務進行分組。

```
group.0.enumclass=com.attask.common.constants.TaskStatusEnum
group.0.enumtype=TASK
group.0.linkedname=direct
group.0.name=State
group.0.type=enum
group.0.valuefield=statusEquatesWith
group.0.valueformat=val
group.1.enumclass=com.attask.common.constants.TaskStatusEnum
group.1.enumtype=TASK
group.1.linkedname=direct
group.1.namekey=status
group.1.type=enum
group.1.valuefield=status
group.1.valueformat=val
textmode=true
```

![螢幕影像，顯示依statusEqualsWith分組的專案任務](assets/status-equates-with.png)


## 校樣核准 — 依專案名稱分組

```
group.0.valueformat=HTML
group.0.valuefield=documentVersion:document:project:name
group.0.displayname=Project Name
```

![螢幕影像，顯示依專案名稱分組的校樣核准](assets/proof-approvals-grouped-by-project-name.png)

