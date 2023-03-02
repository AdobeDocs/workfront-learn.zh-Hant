---
title: 在中尋找和組織資產 [!UICONTROL Workfront DAM]
description: 了解如何搜尋資產、在資料夾內搜尋、簡化搜尋結果、使用中繼資料和關鍵字做為搜尋篩選器，以及 [!UICONTROL Workfront DAM].
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
kt: 8993
exl-id: 28b60118-a471-48bf-ae9b-3a2aed6a6130
doc-type: video
source-git-commit: d39754b619e526e1a869deedb38dd2f2b43aee57
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# 貢獻者：尋找資產

在此影片中，您將學習如何：

* 搜尋資產
* 在資料夾中搜尋
* 簡化搜索結果
* 使用中繼資料和關鍵字作為搜尋篩選器
* 查看資料夾詳細資訊
* 檢視及更新資產中繼資料和關鍵字

>[!VIDEO](https://video.tv.adobe.com/v/335253/?quality=12)

## 基本搜尋條件

基本搜尋會查看檔案名稱、中繼資料欄位、關鍵字和資產內容（視資產類型而定）。 不包含資料夾名稱。

大部分的搜尋結果都是完全相符的。 此「完全相符」規則的例外為 [!UICONTROL Workfront DAM] 搜索檔案名欄位。 [!UICONTROL Workfront DAM] 傳回部分檔案名稱符合，而非完全符合的檔案名稱。

## 搜索時的用戶運算子

雖然基本搜尋功能通常會找到您需要的資產，但您可能需要不時使用其他搜尋參數。

### 部分符合

若要尋找部分相符項目，請在搜尋詞中新增星號。 星號只能在單詞的結尾處使用。

### AND運算子

要查找包含多個搜索詞的結果，請在單詞之間輸入AND。 字詞可以按任意順序找到。 在所有欄位中搜索時，這兩個字可能不會出現在同一欄位中。 例如， Paris AND Tower會在任何欄位中尋找同時包含這兩個字的資產。

### OR運算子

使用OR運算子來尋找包含任何搜尋詞的資產。 例如， Paris OR Arc會尋找包含其中一個字詞的資產，但不一定同時包含這兩個字詞。

### 片語

若要尋找確切的片語，請在單字周圍使用雙引號。 所有的字詞都會按順序排列。 例如，「埃菲爾鐵塔」會按照同樣的順序找到這些詞。

### 負運算子

如果要從搜尋結果中排除字詞，請在字詞前面加上減號(-)。 確保減號和單詞之間沒有空格。 例如，若要排除中繼資料中含有「tower」字樣的資產，您的搜尋可設為「Paris-tower」。

### 空欄位運算子

若要尋找特定中繼資料欄位中沒有資訊的資產，請輸入您要以此格式搜尋的欄位：?[xxxx]. 例如，如果您想尋找未指派關鍵字的資產，請輸入？[關鍵字] 在搜尋欄位中。
