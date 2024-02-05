---
title: 建立和管理問題的嚴重程度
description: 瞭解如何設定和管理問題的嚴重程度。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10020
exl-id: a5a9280b-0d48-413d-92de-f6a949e6b210
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: ht
source-wordcount: '368'
ht-degree: 100%

---

# 建立和管理問題的嚴重程度

## 問題嚴重程度簡介

嚴重程度可以指出一個問題有多嚴重，以及它對於所執行的工作可能有何影響。

![[!UICONTROL 嚴重程度]選單，位於[!UICONTROL 問題詳細資料]視窗](assets/admin-fund-severity-issue-details.png)

您可以在「[!UICONTROL 問題詳細資料]」中存取「[!UICONTROL 嚴重程度]」欄位。在各種清單和自訂報告的欄視圖中也可以包含這個欄位。

[!DNL Workfront] 有五種預設嚴重程度：

* [!UICONTROL 表面]
* [!UICONTROL 導致混淆]
* [!UICONTROL 有因應措施的錯誤]
* [!UICONTROL 無因應措施的錯誤]
* [!UICONTROL 致命錯誤]

如有需要，系統管理員可以重新命名這些預設嚴重程度或建立新的嚴重程度。

唯有 [!DNL Workfront] 中的問題才可以使用嚴重程度。

## 建立和管理問題的嚴重程度

作為系統管理員，若有必要，您可以建立新的嚴重程度，以利完成問題的工作流程。

![[!UICONTROL 嚴重程度]頁面，位於[!UICONTROL 設定]](assets/admin-fund-severity-section.png)

1. 在&#x200B;**[!UICONTROL 主選單]**&#x200B;中按一下「**[!UICONTROL 設定]**」。
1. 展開左側選單面板中的「**[!UICONTROL 專案偏好設定]**」區段。
1. 選取「**[!UICONTROL 嚴重程度]**」。
1. 按一下「**[!UICONTROL 新增一項嚴重程度]**」。
1. 為嚴重程度指定名稱，須與其預定用途相符。
1. 「**[!UICONTROL 重要性]**」的數字與問題的嚴重程度相符。最高的數字對應於最高的嚴重程度。「[!UICONTROL 重要性]」數字必須是唯一的。
1. 選取優先順序的顏色。在圖表報告和 [!DNL Workfront] 的其他地方可以使用這個顏色。
1. 將其中一個嚴重程度選項指定為「**[!UICONTROL 預設嚴重程度]**」。這會自動套用 Workfront 中的所有新問題。
1. 提供嚴重程度的描述，例如如何使用。
1. 按一下欄位以外的地方來儲存。

![[!UICONTROL 嚴重程度]清單](assets/admin-fund-severity-new.png)

### 修改嚴重程度

如果嚴重程度與您的問題工作流程不再相關，您可以將嚴重程度重新命名、隱藏或刪除。

若是不再需要某個嚴重程度，[!DNL Workfront] 建議隱藏該嚴重程度 (按一下「設定」區域中嚴重程度旁邊的「[!UICONTROL 隱藏]」方塊)。這樣一來，問題的下拉式選單便會移除該嚴重程度選項，但是會保留歷史記錄上的嚴重程度，以供報告用途使用。

![[!UICONTROL 隱藏]欄突顯標示，位於[!UICONTROL 嚴重程度]頁面，而此頁面位於[!UICONTROL 設定]](assets/admin-fund-severity-hide.png)

[!DNL Workfront] 建議&#x200B;**不要**&#x200B;刪除過去問題中使用過的嚴重程度。當您刪除一個嚴重程度時，它會要求您用另一個嚴重程度替換。這樣做可能會變更歷史資料並影響報告。

![刪除嚴重程度視窗](assets/admin-fund-severity-delete.png)

<!---
learn more URLs
Create and customize issue severities
Update issue severity
--->
