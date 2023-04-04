---
title: 建立和共用自訂表單
description: 了解如何建立自訂表單、新增唯一欄位至表單、使用區段和邏輯來組織欄位，以及和使用者共用表單。
feature: System Setup and Administration
type: Tutorial
role: Admin, Leader, User
level: Beginner, Intermediate
activity: use
team: Technical Marketing
thumbnail: 335172.png
kt: 8909
exl-id: b37334c7-67d0-4359-9537-dc26843582d1
doc-type: video
source-git-commit: 650e4d346e1792863930dcebafacab4c88f2a8bc
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 5%

---

# 建立和共用自訂表單

在此影片中，您將學習如何：

* 確定用於表單的對象
* 以各種格式新增唯一欄位
* 使用區段和邏輯組織欄位
* 與其他使用者共用表單

>[!VIDEO](https://video.tv.adobe.com/v/335172/?quality=12&learn=on)

## 自訂表單可搭配多種物件類型使用

當您按一下 [!UICONTROL 新自訂表單] 按鈕，您可以選擇任意數量的對象，以便用於單個自定義表單。 自定義表單附加到任何選定對象時，您添加到此表單的所有欄位都將可用。

![顯示 [!UICONTROL 新自訂表單] 對象選項](assets/create-custom-form.png)

編輯自訂表單時，您可以看到選取的所有物件類型。 您可以從此清單中添加或刪除對象類型。

![自訂表單視窗，顯示在表單編輯期間選取的物件類型](assets/edit-custom-form.png)

您可能需要建立專案和問題類型的自訂表單。 附加至問題時，您可以填寫與問題相關的任何欄位。 稍後，如果您決定將期刊轉換為專案，自訂表單會自動載入專案，而您在期刊自訂表單欄位中放入的資料，將可供在專案自訂表單中檢視或編輯。

## 自訂欄位選項

**[!UICONTROL 標籤] 和 [!UICONTROL 名稱] 欄位**

此 [!UICONTROL 標籤] 和 [!UICONTROL 名稱] 自訂欄位上的欄位的用途不同。 [!UICONTROL 標籤] 是使用者在中看到的欄位名稱 [!DNL Workfront]. [!UICONTROL 名稱] 是可與整合搭配使用的項目，例如API。

![自訂表單視窗顯示 [!UICONTROL 標籤] 和 [!UICONTROL 名稱] 欄位](assets/custom-forms-field-label-and-name.png)

這提供變更使用者對應標籤的彈性，以符合組織中的變更，而不會影響整合或依賴特定欄位名稱的其他連線。

**[!UICONTROL 含格式的文字欄位]**

此 [!UICONTROL 具有格式的文本欄位 ]包含基本文字標籤工具，可讓使用者在自訂表單的欄位中填入時，在文字上新增粗體、斜體或底線。

![自訂表單視窗顯示 [!UICONTROL 具有格式的文本欄位] 選項](assets/custom-forms-text-field-with-formatting.png)

該欄位還有15,000個字元的限制，可提供大量空間以提供重要資訊，並使用格式設定，讓其他人更容易閱讀。

**[!UICONTROL Typeahead] 欄位**

此 [!UICONTROL Typeahead] 欄位可讓系統根據為欄位選取的物件自動填入選項清單。

![自訂表單視窗顯示 [!UICONTROL Typeahead] 欄位選項](assets/custom-forms-typeahead-1.png)

例如，若您建立 [!UICONTROL Typeahead] 名為「行銷經理核准名稱」的欄位，並選取 [!UICONTROL 使用者] 作為引用的對象類型，當用戶在自定義表單上填入該欄位時，將顯示用戶名清單。 此 [!UICONTROL Typeahead] 欄位的用途是連結您的自訂資料與系統中擷取的資訊，而無須在下拉式欄位中手動維護許多選項。

![自訂表單視窗顯示 [!UICONTROL Typeahead] 下拉式功能表](assets/custom-forms-typeahead-2.png)
