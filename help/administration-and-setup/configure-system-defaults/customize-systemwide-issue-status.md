---
title: 自訂全系統適用的問題狀態
description: 瞭解如何變更問題狀態名稱、控制用於某種狀態的問題類型，以及為進行群組層級自訂化而鎖定/解鎖狀態。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Intermediate, Experienced
jira: KT-10030
exl-id: c8f5677f-8d9d-4d1a-a1e3-d1a438878213
TQID: https://experienceleague.adobe.com/Wo7ObQJmkrsaYDXxaPMYQvDFfQx8wtC8qYi3Nvc6DkY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 36674ed53c8645f556862bb2d99f3bfd6c993c1e
workflow-type: tm+mt
source-wordcount: 392
ht-degree: 100%

---

# 自訂全系統適用的狀態

[!DNL Workfront] 提供各種預設狀態來滿足貴組織問題管理工作流程的需求。 這些狀態可以根據貴組織的術語重新命名。 而且狀態可以指派給特定的問題類型。

如有必要，也可以建立其他狀態。 唯有系統管理員才能建立全系統適用的狀態。 此外，系統管理員控制群組管理員可以編輯哪些狀態。

![[!UICONTROL 問題]標籤，位於[!UICONTROL 狀態]頁面，而此頁面位於[!UICONTROL 設定]](assets/admin-fund-all-issue-statuses.png)

## 修改現有狀態

[!DNL Workfront] 建議盡量使用最少數量的狀態。 這樣一來，使用者才能輕鬆選擇合適的狀態，而且要維護的狀態清單也比較簡短。

您可以編輯現有狀態來變更名稱、所指派的問題類型、相關顏色等。

![問題狀態清單的「[!UICONTROL 編輯]」選項突顯標示](assets/admin-fund-edit-issue-status.png)

1. 在&#x200B;**[!UICONTROL 主選單]**&#x200B;中按一下「**[!UICONTROL 設定]**」。
1. 展開左側選單面板中的「**[!UICONTROL 專案偏好設定]**」區段。
1. 選取「**[!UICONTROL 狀態]**」。
1. 選取「**[!UICONTROL 問題]**」標籤並確保「[!UICONTROL 系統狀態]」顯示在右上角。
1. 選取「**[!UICONTROL 主清單]**」來查看所有問題類型的狀態。 您可以在這裡建立或修改問題狀態。
1. 把游標懸停在想要重新命名的狀態右側，再按一下「**[!UICONTROL 編輯]**」。
1. 為狀態指定新名稱，或是依需要變更任何其他資訊。
1. 若是這些設定應套用至您在 [!DNL Workfront] 執行個體中的所有使用者，請鎖定狀態。
1. 解鎖狀態，讓群組管理員僅可編輯其群組的狀態。
1. 勾選應套用狀態的問題類型之方塊。
1. 按一下「**[!UICONTROL 儲存]**」。

![建立新狀態的視窗](assets/admin-fund-edit-issue-status-2.png)

### 狀態指派

並非所有狀態都可以指派給所有問題類型。 「[!UICONTROL 狀態]」頁面有多欄會顯示每個狀態可用於哪種問題類型。

![「狀態」頁面的「問題」標籤上「變更順序」突顯標示](assets/admin-fund-issue-type-statuses.png)


若要只查看指派給特定問題類型的狀態，請按一下視窗頂端的問題類型名稱。

![[!UICONTROL 問題]標籤，位於[!UICONTROL 狀態]頁面，其中突顯標示欄](assets/admin-fund-statuses-issue-type.png)

在這裡，您可以把拖曳問題使其按照您想要的順序出現在「[!UICONTROL 狀態]」下拉式選單中。

要編輯狀態，您必須回到「[!UICONTROL 主清單]」。
