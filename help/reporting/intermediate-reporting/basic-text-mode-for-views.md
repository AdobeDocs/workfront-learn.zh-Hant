---
title: 了解檢視的基本文字模式
description: 了解哪些文字模式、駝峰式大小寫，以及一些基本的「即插即用」文字模式，可在Workfront的檢視中使用。
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 11367
exl-id: 156e5510-4a51-449f-9c8c-e16fdd8ea23d
source-git-commit: 818ee105af32589cb0e297e6f419a4a449a60052
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# 了解檢視的基本文字模式


>[!IMPORTANT]
>
>必要條件：
>
>* 了解報表元素
>* 了解報表元件
>* 建立基本檢視


>[!TIP]
>
>* 若要更深入了解文字模式，建議您觀看錄影的網路研討會活動 [詢問專家 — 文字模式報表簡介](https://experienceleague.adobe.com/docs/workfront-events/events/reporting-and-dashboards/introduction-to-text-mode-reporting.html?lang=en)，長度為一小時。
>* 若要進一步了解文字模式，建議您觀看 [進階報表](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/advanced-reporting/welcome-to-advanced-reporting.html?lang=en) 教學課程，總共需要5.5小時。


在此影片中，您將學習：

* 什麼是文字模式
* 駝峰是什麼
* 您可以在檢視中使用一些基本的「即插即用」文字模式

>[!VIDEO](https://video.tv.adobe.com/v/3410571/?quality=12)

## 任務 — 4個父視圖

首先為「任務名」和「父名」建立列，然後使用以下文本模式建立其他三列。

### 任務 — 父代名稱的父代

```
displayname=Parent of Parent Name
linkedname=parent
namekey=view.relatedcolumn
namekeyargkey.0=parent
namekeyargkey.1=name
querysort=parent:parent:name
textmode=true
valuefield=parent:parent:name
valueformat=HTML
```

### 任務 — 父代名稱的父代

```
displayname=Parent of Parent of Parent Name
linkedname=parent
namekey=view.relatedcolumn
namekeyargkey.0=parent
namekeyargkey.1=name
querysort=parent:parent:parent:name
textmode=true
valuefield=parent:parent:parent:name
valueformat=HTML
```

### 任務 — 父代的父代的父代的父代名稱

```
displayname=Parent of Parent of Parent of Parent Name
linkedname=parent
namekey=view.relatedcolumn
namekeyargkey.0=parent
namekeyargkey.1=name
querysort=parent:parent:parent:parent:name
textmode=true
valuefield=parent:parent:parent:parent:name
valueformat=HTML
```

![顯示4個父視圖的螢幕影像](assets/4-parents-view.png)

## 使用者 — 在使用者檢視中顯示清單的迭代

### 用戶 — 所有作業角色

```
displayname=All job roles
listdelimiter=<p>
listmethod=nested(userRoles).lists
textmode=true
type=iterate
valuefield=role:name
valueformat=HTML
```

### 用戶 — 顯示主要的所有作業角色

```
displayname=All Job Roles showing primary
listdelimiter=<p> 
listmethod=nested(userRoles).lists 
textmode=true
type=iterate 
valueexpression=IF({user}.{roleID}={role}.{ID},CONCAT("** ",{role}.{name}," **"),{role}.{name})
valueformat=HTML
```

### 使用者 — 所有團隊

```
displayname=All teams
listdelimiter=<p>
listmethod=nested(teams).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

>[!NOTE]
>
>透過UI可存取「團隊」欄位，顯示所有團隊（以逗號分隔），但使用上述文字模式時，會將每個團隊顯示在個別行上。


### 用戶 — 所有組

```
displayname=All groups
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valuefield=group:name
valueformat=HTML
```

### 用戶 — 顯示首頁組的所有組

```
displayname=All groups showing home group
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valueexpression=IF({user}.{homeGroupID}={group}.{ID},CONCAT("** ",{group}.{name}," **"),{group}.{name})
valueformat=HTML
```


### 使用者 — 直接報表

```
displayname=Direct reports
listdelimiter=<p>
listmethod=nested(directReports).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

### 用戶 — 未來PTO

```
displayname=Future PTO
listdelimiter=<br>
listmethod=nested(reservedTimes).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=IF({startDate}>$$TODAY,CONCAT({startDate}," - ",{endDate}),"")
valueformat=HTML
width=150
```

![顯示「用戶清單」視圖的螢幕影像](assets/user-lists-view-large.png)

## 任務 — 如何顯示任務分配和處理狀態

```
displayname=Assignments and Status
listdelimiter=<br>
listmethod=nested(assignments).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=CONCAT({assignedTo}.{name},IF(ISBLANK({assignedTo}.{name}),"",IF({status}="AA"," - Requested",IF({status}="AD"," - Working"," - Done"))))
valueformat=HTML
width=150
```

![顯示「分配」和「狀態」視圖的螢幕影像](assets/assignments-and-status-view.png)


## 任務 — 如何在多個任務分配上顯示角色和分配

### 任務 — 角色+小時

```
displayname=Role+hours
listdelimiter=<li>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT({role}.{name}," (",round({workRequired}/60,2),")")
valueformat=HTML
```

### 任務 — 分配+百分比分配

```
displayname=Assignment+percent
valueexpression=CONCAT({assignedTo}.{name}," (",{assignmentPercent},")")
listdelimiter=<li>
listmethod=nested(assignments).lists
valueformat=HTML
textmode=true
type=iterate
```

![顯示「分配」和「角色」視圖的螢幕影像](assets/assignments-roles-and-percent-view.png)

## 任務 — 跨項目前置任務和後置任務

### 任務篩選器（可選）

**向我顯示至少有一個跨項目前身的所有任務**

```
predecessorsMM:ID_Mod=notblank
predecessorsMM:projectID=FIELD:projectID
predecessorsMM:projectID_Mod=ne
```

### 任務 — 顯示前置名稱和項目前置名稱

```
displayname=Predecessor names
listdelimiter=<br>
listmethod=nested(predecessors).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=CONCAT("TASK = ",{predecessor}.{name}," >> PROJECT = ",{predecessor}.{project}.{name})
valueformat=HTML
width=150
```

### 任務 — 顯示後繼名稱和項目後繼項在

```
displayname=Successor names
listdelimiter=<br>
listmethod=nested(successors).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=CONCAT("TASK = ",{successor}.{name}," >> PROJECT = ",{successor}.{project}.{name})
valueformat=HTML
width=150
```

### 任務 — 顯示前置任務的預計完成日期

```
displayname=Predecessor projected completion dates
valueformat=atDate
listdelimiter=
textmode=true
width=90
stretch=0
valuefield=predecessor:projectedCompletionDate
type=iterate
listmethod=nested(predecessors).lists
shortview=false
```

### 任務 — 顯示前置任務的進度狀態

```
displayname=Predecessor progress status
listdelimiter=<br>
listmethod=nested(predecessors).lists
shortview=false
stretch=0
textmode=true
type=iterate
valueexpression=IF({predecessor}.{progressStatus}="OT","On Time",IF({predecessor}.{progressStatus}="LT","Late",IF({predecessor}.{progressStatus}="BH","Behind","At Risk")))
valueformat=HTML
width=90
```

### 任務 — 顯示跨項目前置項目的完成百分比

```
displayname=Predecessor project percent complete
listdelimiter=<br>
listmethod=nested(predecessors).lists
namekey=group.plural
textmode=true
type=iterate
valueexpression=IF({isCP}=true,CONCAT({predecessor}.{project}.{percentComplete},"%"),"")
valueformat=HTML
width=150
```

![顯示「交叉項目前置項和後置項」視圖的螢幕影像](assets/cross-project-predecessors-and-successors.png)


## 任務 — 小版本，顯示所有已分配的人員以及每個人員的分配

```
displayname=All assignees and requesters
listdelimiter=<p>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT("Assigned To: ",{assignedTo}.{name},"; Requested By: ",{assignedBy}.{name})
valueformat=HTML
```

![螢幕影像，顯示所有指派的人員以及指派給每個人員的人員](assets/all-assignees-and-requesters.png)

## 任務/項目 — 顯示項目或任務上所有自定義表單的迭代

```
displayname=All Forms Assigned
listdelimiter=<p>
listmethod=nested(objectCategories).lists
textmode=true
type=iterate
valuefield=category:name
valueformat=HTML
```

![顯示專案中所有自訂表單的螢幕影像](assets/all-custom-forms-on-a-project.png)


## 項目 — 在項目視圖中顯示可解析項的所有主要聯繫人的小版本

```
displayname=Requestor
listdelimiter=<br>
listmethod=nested(resolvables).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=owner:name
valueformat=HTML
width=150
```

![螢幕影像，顯示可解析度的主要接觸點](assets/primary-contacts-for-resolvables.png)

## 項目 — 顯示所有項目組成員的小版本

```
displayname=Project Team Members
listdelimiter=<br>
listmethod=nested(projectUsers).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=user:name
valueformat=HTML
```

![顯示所有專案團隊成員的螢幕影像](assets/all-project-team-members.png)

## 項目 — 顯示項目所有可解決問題的entryDate的小版本

```
displayname=Resolvables entry date
linkedname=direct
listdelimiter=<br>
listmethod=nested(project.resolvables).lists
listsort=string(description)
querysort=description
section=0
textmode=true
type=iterate
valuefield=entryDate
valueformat=HTML
```

![螢幕影像，顯示專案所有可解決問題的entryDate](assets/resolvables-entry-date.png)

## 專案 — 顯示原始專案請求者的首頁群組

```
displayname=Requestor home group
linkedname=direct
namekey=name
querysort=convertedOpTaskOriginator:homeGroup:name
textmode=true
valuefield=convertedOpTaskOriginator:homeGroup:name
valueformat=HTML
```

![顯示專案要求者首頁群組的螢幕影像](assets/requestor-home-group.png)

## 專案 — 顯示專案是否為請求佇列

```
querysort=queueDef:isPublic
valueformat=val
description=0 (None), 1 (Public), 2 (Private), 3 (Company), 4 (Group)
linkedname=direct
textmode=true
enumtype=PROJ
valuefield=queueDef:isPublic
namekey=status
type=enum
enumclass=com.attask.common.constants.ProjectStatusEnum
displayname=Public Selection
```

![顯示專案是否為請求佇列的畫面影像](assets/project-is-a-request-queue.png)

## 問題 — 顯示所有解決的項目組成員的小版本

```
displayname=Resolve Project: Team Members
listdelimiter=<br>
listmethod=nested(resolveProject.projectUsers).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=user:name
valueformat=HTML
width=150
```

![顯示所有解析項目組成員的螢幕影像](assets/all-resolve-project-team-members.png)

## 問題 — 顯示問題主要聯繫人的所有團隊的小版本

```
displayname=Requestor Teams
listdelimiter=<br>
listmethod=nested(owner.teams).lists
namekey=group.plural
textmode=true
type=iterate
valuefield=name
valueformat=HTML
width=150
```

![顯示所有主要聯絡團隊的螢幕影像](assets/all-primary-contact-teams.png)

## 文檔 — 顯示文檔報告中資料夾的小版本

```
displayname=Folder
listdelimiter=<br><br>
listmethod=nested(folders).lists
textmode=true
type=iterate
valuefield=name
valueformat=HTML
```

![顯示文檔報告中資料夾的螢幕影像](assets/folder-in-a-document-report.png)

## 文檔 — 顯示文檔報表中父資料夾的小版本

```
displayname=Parent Folder
listdelimiter=<br><br>
listmethod=nested(folders).lists
textmode=true
type=iterate
valuefield=parent:name
valueformat=HTML
```

![在文檔報表中顯示父資料夾的螢幕影像](assets/parent-folder-in-a-document-report.png)

## 文檔 — 文檔批准日期

```
displayname=Document Approval Dates
valueformat=HTML
listdelimiter=<br>
linkedname=direct
textmode=true
listsort=string(description)
valuefield=approvalDate
type=iterate
listmethod=nested(approvals).lists
shortview=false
section=0
```

![顯示「文檔批准日期」視圖的螢幕影像](assets/document-approval-dates.png)

## 校訂核准

### 校樣核准 — 顯示專案名稱

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name 
valueformat=HTML
```

### 校樣批准 — 顯示任務名稱

```
displayname=Task Name
textmode=true 
valuefield=documentVersion:document:task:name 
valueformat=HTML
```

![顯示專案和校樣核准工作的螢幕影像](assets/proof-approval-project-and-task.png)
