---
title: 最佳實務 - API Explorer
description: 探索 Adobe Workfront 專家提供的有關設定、管理和使用 Workfront API Explorer 的最佳實務建議。
feature: Workfront API
role: Admin, Leader, User
level: Beginner
jira: KT-10902
exl-id: 0f3fc5ba-d01a-4337-829f-def0830ddf81
TQID: https://experienceleague.adobe.com/RUQeNzEb0eg9DKSKepugb0HD4O2ODql-0mWBn-ptgxk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: bb1dd007-4a34-496d-9d3b-2278fdaadac1
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 410
ht-degree: 75%

---

# 最佳實務 - API Explorer

## 什麼是 Adobe Workfront「最佳實務」？

最佳實務是代表有效果、有效率之行動方針的準則；您和公司的使用者可以輕鬆採用；並且可以成功複製到整個組織。

當您審閱這些建議時，請記住，有一些 Workfront 最佳實務是通用的，而其他做法可能針對特定主題。 將這些最佳實務視為框架，作為設定和使用 Workfront 系統時的指引。

## 導覽此頁面

當您捲動瀏覽此頁面時，您會先找到該主題所有最佳實務的高層次清單。 這樣您便可以審閱建議而無需深入瞭解詳細的「原因」。

「為什麼這些是最佳實務？」區域會在高階清單後面找到，其中提供某些最佳實作的更詳細資料，以及為什麼這些被視為流程、工具等，您應考慮使用Workfront執行個體進行實施。

</br>
</br>

## API Explorer 最佳實務

* 針對與第三方系統整合功能搭配使用的自訂欄位建立命名慣例。

* 使用 Workfront 專案來追蹤整合功能中使用的所有自訂欄位。

* 在系統管理員使用的報告中新增物件 ID 欄位。

</br>
</br>

## 為什麼這些是最佳實務？

**最佳實務**

針對與第三方系統整合功能搭配使用的自訂欄位建立命名慣例。

**原因說明**

請確認建立自訂表單的每個人均知道命名慣例，以便他們不會意外使用供整合功能使用的保留欄位。 根據您的整合功能與工作流程而定，以多種方式使用相同的欄位，可能造成資料被修改或覆寫，並可能造成報告中使用的資料不正確。

</br>
</br>


**最佳實務**

使用 Workfront 專案來追蹤整合功能中使用的所有自訂欄位。

**原因說明**

專案是記錄自訂欄位名稱、其用途等的最佳位置。這可協助您避免建立多餘的自訂欄位，或避免使用具有多個整合的相同自訂欄位。

</br>
</br>


**最佳實務**

在系統管理員使用的報告中新增物件 ID 欄位。

**原因說明**

系統管理員在使用 API 或其他整合功能時，經常需要使用物件 ID 號碼來參照 Workfront 中的物件。 在您處理的物件（專案、任務、問題、範本、自訂表格等）的檢視中加入ID欄位 以方便存取和複製。
