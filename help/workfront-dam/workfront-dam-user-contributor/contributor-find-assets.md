---
title: 在中尋找及組織資產 [!UICONTROL WORKFRONT DAM]
description: 瞭解如何搜尋資產、在資料夾中搜尋、簡化搜尋結果、使用中繼資料和關鍵字作為搜尋篩選條件，以及更多關於 [!UICONTROL WORKFRONT DAM].
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8993
exl-id: 28b60118-a471-48bf-ae9b-3a2aed6a6130
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# 投稿人：尋找資產

在本影片中，您將瞭解如何：

* 搜尋資產
* 在資料夾中搜尋
* 簡化搜尋結果
* 使用中繼資料和關鍵字作為搜尋篩選器
* 檢視資料夾詳細資訊
* 檢視和更新資產中繼資料和關鍵字

>[!VIDEO](https://video.tv.adobe.com/v/335253/?quality=12&learn=on)

## 基本搜尋條件

基本搜尋會檢視檔案名稱、中繼資料欄位、關鍵字和資產內容（視資產型別而定）。 其中不包含資料夾名稱。

大部分的搜尋結果都是完全相符的。 此「完全符合」規則的例外情況是 [!UICONTROL WORKFRONT DAM] 會搜尋檔案名稱欄位。 [!UICONTROL WORKFRONT DAM] 傳回符合的檔案名稱部分，而不只是完全符合的檔案名稱。

## 搜尋時的使用者運運算元

雖然基本搜尋功能通常會找到您需要的資產，但您有時仍需要使用其他搜尋引數。

### 部分符合

若要尋找部分相符專案，請在搜尋字詞中加入星號。 星號只能用於單詞的結尾。

### AND運運算元

若要尋找包含多個搜尋字詞的結果，請在字詞之間輸入AND。 這些字詞可以任意順序找到。 在所有欄位中搜尋時，兩個字詞可能不會出現在同一個欄位中。 例如，Paris AND Tower會找到在任何欄位中都包含這兩個字詞的資產。

### OR運運算元

使用OR運運算元來尋找包含任何搜尋字詞的資產。 例如，Paris OR Arc會找到具有其中一個字詞，但不一定同時具有這兩個字詞的資產。

### 片語

若要尋找確切的片語，請在字詞前後加上雙引號。 所有字詞將一起依序找到。 例如，「埃菲爾鐵塔」會依照該順序找到這些字詞。

### 負值運運算元

如果您要從搜尋結果中排除某個字詞，請在該字詞前加上減號(-)。 請確定減號與單字之間沒有空格。 例如，若要排除中繼資料中含有單字「tower」的資產，您的搜尋可設定為Paris -tower。

### 空白欄位運運算元

若要尋找在特定中繼資料欄位中沒有資訊的資產，請以此格式輸入您要搜尋的欄位： ？[xxxxx]. 例如，如果您要尋找未指派關鍵字的資產，請輸入？[關鍵字] 在搜尋欄位中。
