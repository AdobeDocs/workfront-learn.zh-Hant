---
title: 建立和管理問題嚴重性
description: 了解如何設定和管理問題嚴重性。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
kt: 10020
exl-id: a5a9280b-0d48-413d-92de-f6a949e6b210
source-git-commit: 5d385de5cdcee0d433304c09507ba6bb5b0a10e6
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 3%

---

# 建立和管理問題嚴重性

## 問題嚴重性簡介

嚴重性可用來指出問題的嚴重性，或可能如何影響正在進行的工作。

![[!UICONTROL 嚴重性] 功能表 [!UICONTROL 問題詳細資訊] 視窗](assets/admin-fund-severity-issue-details.png)

此 [!UICONTROL 嚴重性] 欄位可在 [!UICONTROL 問題詳細資訊]. 它也可包含在清單的欄檢視中，以及自訂報表中。

[!DNL Workfront] 有五個預設性質：

* [!UICONTROL 輕微]
* [!UICONTROL 導致混淆]
* [!UICONTROL 有因應措施的錯誤]
* [!UICONTROL 無因應措施的錯誤]
* [!UICONTROL 致命錯誤]

系統管理員可以更名這些預設的嚴重性，或視需要建立新的嚴重性。

嚴重性僅適用於 [!DNL Workfront].

## 建立和管理問題嚴重性

作為系統管理員，您可以視需要建立新的嚴重性，以完成問題的工作流程。

![[!UICONTROL 嚴重性] 頁面 [!UICONTROL 設定]](assets/admin-fund-severity-section.png)

1. 按一下 **[!UICONTROL 設定]** 在 **[!UICONTROL 主菜單]**.
1. 展開 **[!UICONTROL 專案偏好設定]** 區段。
1. 選擇 **[!UICONTROL 嚴重性]**.
1. 按一下 **[!UICONTROL 添加新嚴重性]**.
1. 請為嚴重性指定與其預期用途相符的名稱。
1. 此 **[!UICONTROL 重要性]** 數字與問題的嚴重性相符。 最高數與最高嚴重性相對應。 此 [!UICONTROL 重要性] 數字必須是唯一的。
1. 選取優先順序的顏色。 這可用於圖表報表和 [!DNL Workfront].
1. 指定其中一個嚴重性選項作為 **[!UICONTROL 預設嚴重性]**. 這會自動套用至Workfront中的所有新問題。
1. 包括嚴重性的說明，如使用方式。
1. 按一下要儲存的欄位外部。

![[!UICONTROL 嚴重性] 清單](assets/admin-fund-severity-new.png)

### 修改嚴重性

如果嚴重性不再與您的問題工作流程相關，可以重新命名、隱藏或刪除。

如果不再需要嚴重性， [!DNL Workfront] 建議您隱藏嚴重性(按一下 [!UICONTROL 隱藏] 框中)。 這會從問題的下拉式功能表中移除嚴重性選項，但仍會保留歷史資料的嚴重性，因此仍可用於報表用途。

![[!UICONTROL 隱藏] 突出顯示的列 [!UICONTROL 嚴重性] 頁面 [!UICONTROL 設定]](assets/admin-fund-severity-hide.png)

[!DNL Workfront] 建議您 **不** 刪除過去問題上使用的嚴重性。 刪除嚴重性時，系統會要求您替代另一個嚴重性。 這可以變更歷史資料並影響報告。

![刪除嚴重性窗口](assets/admin-fund-severity-delete.png)

<!---
learn more URLs
Create and customize issue severities
Update issue severity
--->
