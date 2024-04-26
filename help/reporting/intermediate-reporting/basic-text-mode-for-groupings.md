---
title: 瞭解分組的基本文字模式
description: 瞭解什麼是文字模式、什麼是駝峰式大小寫，以及您可以在 Workfront 的分組中使用的一些「隨插即用」基本文字模式。
activity: use
feature: Text Mode Reporting
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
jira: KT-11369
exl-id: 5f45c64f-a22b-4983-91fd-9a1939f99fb1
doc-type: video
source-git-commit: 61b6971457198d2c39cc4dab67aebc6e8c6988f6
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 100%

---

# 瞭解分組的基本文字模式

>[!PREREQUISITES]
>
>* [瞭解報告元素](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-elements.html?lang=zh-Hant)
>* [瞭解報告元件](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/reporting-components.html?lang=zh-Hant)
>* [建立基本分組](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/create-a-basic-grouping.html?lang=zh-Hant)


>[!TIP]
>
>* 為了深入瞭解文字模式，我們建議觀看錄影版網路研討會活動「[詢問專家 - 文字模式報告簡介](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=zh-Hant)」，影片長度為 1 小時。
>* 若要更加深入瞭解文字模式，我們建議觀看「[進階報告](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=zh-Hant)」教學課程，全部課程總長 5 個半小時。
>* 按一下此處以存取 [[!UICONTROL API Explorer]](https://developer.adobe.com/workfront/api-explorer/)

觀看這段影片，您將會瞭解：

* 什麼是文字模式
* 什麼是駝峰式大小寫
* 可以在分組中使用的一些基本「隨插即用」文字模式

>[!VIDEO](https://video.tv.adobe.com/v/3410641/?quality=12&learn=on)

## 任務 - 4 個父系分組

以下文字模式將根據最多四個層級的父系把任務分組，並把不存在的父系留白。

```
textmode=true
group.0.name=Parents
group.0.valueexpression=CONCAT({parent}.{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{parent}.{name}),"",", "),{parent}.{parent}.{name},IF(ISBLANK({parent}.{parent}.{name}),"",", "),IF(ISBLANK({parent}.{name}),"No parent",{parent}.{name}))
group.0.linkedname=parent
group.0.namekeyargkey.0=parent
group.0.namekeyargkey.1=name
group.0.valueformat=string
```

![畫面影像顯示專案任務依 4 個父系分組](assets/4-parents-grouping.png)


## 任務 - 完成百分比分組

以下文字模式將根據任務的完成百分比進行分組。分組時，任務將屬於以下其中一個類別：

* 0%
* 1% 至 25%
* 26% 至 50%
* 51% 至 75%
* 76% 至 99%
* 100%

```
group.0.linkedname=direct
group.0.namekey=percentComplete
group.0.valueexpression=IF({percentComplete}<1,"0%",IF({percentComplete}<26,"1% to 25%",IF({percentComplete}<51,"26% to 50%",IF({percentComplete}<76,"51% to 75%",IF({percentComplete}<100,"76% to 99%",IF({percentComplete}=100,"100","***"))))))
group.0.valueformat=doubleAsString
textmode=true
```

![畫面影像顯示專案任務依完成百分比分組](assets/percent-complete-grouping.png)

## 任務 - 先根據 statusEquatesWith 再根據 status

以下文字模式會先根據 statusEquatesWith，再根據 status 把任務分組。

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

![畫面影像顯示專案任務依 statusEquatesWith 分組](assets/status-equates-with.png)


## 校訂核准 - 按專案名稱分組

```
group.0.valueformat=HTML
group.0.valuefield=documentVersion:document:project:name
group.0.displayname=Project Name
```

![畫面影像顯示校訂核准依專案名稱分組](assets/proof-approvals-grouped-by-project-name.png)


## 校訂核准 - 依文件名稱分組

```
group.0.displayname=Document Name
group.0.valuefield=documentVersion:document:name
group.0.valueformat=HTML
```

![畫面影像顯示校訂核准依專案名稱分組](assets/proof-approvals-grouped-by-doc-name.png)

