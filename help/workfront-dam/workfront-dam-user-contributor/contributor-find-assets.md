---
title: 以貢獻者身分瞭解如何尋找資產
description: 瞭解在 [!UICONTROL Workfront DAM] 中如何搜尋資產、在資料夾內搜尋、簡化搜尋結果、使用中繼資料和關鍵字作為篩選器。
activity: use
feature: Digital Content and Documents
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
jira: KT-8993
exl-id: 28b60118-a471-48bf-ae9b-3a2aed6a6130
doc-type: video
source-git-commit: 2cb3cc67f4f1fcd1345f178bf525d7b00f6271cf
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 100%

---

# 以貢獻者身分瞭解如何尋找資產

觀看這段影片，您將瞭解如何：

* 搜尋資產
* 在資料夾內搜尋
* 簡化搜尋結果
* 使用中繼資料和關鍵字作為搜尋篩選器
* 檢視資料夾詳細資料
* 檢視及更新資產中繼資料和關鍵字

>[!VIDEO](https://video.tv.adobe.com/v/335253/?quality=12&learn=on)

## 基本搜尋條件

基本搜尋的尋找範圍包括檔案名稱、中繼資料欄位、關鍵字和資產內容 (根據資產類型而定)。但是不包括資料夾名稱。

大部分搜尋結果均是完全符合的內容。[!UICONTROL Workfront DAM] 搜尋檔案名稱欄位時是此一「完全符合」規則的例外情況。[!UICONTROL Workfront DAM] 傳回與檔案名稱部分符合而不是完全符合的結果。

## 使用者的搜尋運算子

雖然基本搜尋功能通常都能找到您需要的資產，但是也有偶爾需要使用其他搜尋參數的時候。

### 部分相符

要尋找部分相符的結果，請在搜尋字詞中加入星號。星號只能放在字詞的尾端。

### AND 運算子

要尋找包含多個搜尋字詞的結果，請在字詞之間輸入 AND。這些字詞可以依任何順序尋找。在搜尋所有欄位時，兩個字詞可能不會出現在相同的欄位中。例如，「Paris AND tower」將尋找任何欄位中同時包含兩個字詞的資產。

### OR 運算子

使用 OR 運算子來尋找含有任一搜尋字詞的資產。例如，「Paris OR Arc」將尋找含有其中一個字詞，但不必要是兩者兼有的資產。

### 字句

要尋找完全符合的字句，請在字詞前後加上雙引號。系統將按照指定順序同時尋找所有字詞。例如，「Eiffel Tower」將會完全按照這樣的順序尋找這些字詞。

### 減號運算子

如果您要在搜尋結果中排除某個字詞，請在字詞前面放上減號 (-)。請確保減號與字詞之間沒有任何空格。例如，要排除在中繼資料中含有字詞「tower」的資產，您的搜尋必須設為「Paris -tower」。

### 空白欄位運算子

要尋找在特定中繼資料欄位沒有任何資訊的資產，請用以下格式輸入您要搜尋的欄位：?[xxxxx]。例如，若您要搜尋未指派任何關鍵字的資產，請在搜尋欄位輸入 ?[keyword]。
