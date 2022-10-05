---
title: 了解篩選器的基本文字模式
description: 了解哪些文字模式、駝峰式大小寫，以及一些基本的「即插即用」文字模式，可用於 [!DNL  Workfront].
activity: use
feature: Reports and Dashboards
thumbnail: 336820.png
type: Tutorial
role: User
level: Intermediate
team: Technical Marketing
kt: 9086
exl-id: b3f16468-b720-468d-887a-b313fc32bd89
source-git-commit: 83c7379a5398c78cea31a4571b34fd5b64bce027
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# 了解篩選器的基本文字模式

在此影片中，您將學習：

* 什麼是文字模式
* 駝峰是什麼
* 您可以在報表篩選器中使用一些基本的「即插即用」文字模式

>[!VIDEO](https://video.tv.adobe.com/v/336820/?quality=12)

以下文本模式將排除用戶已標籤為「完成我的部件」的任務。 您只需建立任務篩選器，添加任何需要的篩選規則，然後切換到文本模式，並將代碼貼到您在篩選器中看到的任何文本模式之後。

```
EXISTS:1:$$OBJCODE=ASSGN  
EXISTS:1:taskID=FIELD:ID  
EXISTS:1:status=DN  
EXISTS:1:status_Mod=notin  
EXISTS:1:assignedToID=$$USER.ID 
```

## 活動：文字模式問題

1. 您如何為標題為「由ID輸入」的欄位撰寫駝峰大小寫？
1. 在「問題」報表中，建立篩選器以顯示標示為已結束但待核准的問題。

## 答案

1. 「Entered By ID」欄位的駝峰大小寫應如下 — enteredByID
1. 文字模式在問題報表篩選器中應如下所示：

   ![在文本模式中建立新篩選器的螢幕影像](assets/btm-answer.png)
