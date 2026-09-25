---
title: 自訂表單問題解答
description: 取得自訂表單常見問題的解答
feature: Custom Forms
type: Tutorial
role: Admin, Leader, User
level: Beginner, Intermediate
activity: use
team: Technical Marketing
jira: KT-10058
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
    internal-label: Leader
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
source-git-commit: 54883ad8c8df3aaee06ba8f8dca64227594c1c77
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 88%
---
# 自訂表單相關常見問題

**我在建立欄位之後可否變更其顯示類型？ 例如，我可以把下拉式選單變更為核取方塊嗎？**

是。 顯示型別可以切換為另一個類似的顯示型別 — 文字到段落、下拉式清單到核取方塊或選項按鈕等。如需變更顯示型別的詳細資訊，請參閱「建立自訂表單」文章。


**我可以對多個物件使用相同的自訂表單嗎？ 例如，我為任務建立的表單亦供專案使用？**

否。 自訂表單與物件是一對一的關係。 但是，您可以複製自訂表單並按照需要變更物件。


**自訂表單可以附加到專案範本嗎？**

是。 這樣一來，使用該範本建立的任何專案均會附加自訂表單。


**自訂表單上的欄位數量是否有限制？**

您可以在單一自訂表單上新增最多 500 個欄位。 但是，視自訂表單的複雜度而定，當表單上擁有超過 100 個欄位時，效能可能會下降。 複雜表單的例子包括具有逐層傳遞參數的表單、計算自訂資料欄位以及特定欄位有多個值選項。


**我可以附加到專案的自訂表單是否有數量限制？**

是。 您可以在一個物件上附加最多 10 個自訂表單。 如需更多資訊，請參閱此文章「套用自訂表單至物件」。


**我可以停用自訂表單嗎？**

是。 在自訂表單的「表單設定」標籤中，取消勾選「使用中」方塊。 這樣一來，整個 Workfront 中的任何下拉式選單均會移除自訂表單。 但是，如果自訂表單已附加到專案上，則該表單會保留並保存已經輸入的任何資料。