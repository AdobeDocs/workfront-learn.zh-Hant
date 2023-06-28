---
title: 篩選器
description: 瞭解如何在模組之間使用篩選器，以僅允許特定型別的套件組合通過。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11040
thumbnail: KT1101.png
exl-id: d2cec1ea-7ff9-48ae-8bfb-0c767d346079
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# 篩選器

瞭解如何在模組之間使用篩選器，以僅允許特定型別的套件組合通過。

## 練習概述

在「超出基本對應」情境中的兩個模組之間新增篩選器，以僅建立在CSV檔案中具有「紅色」專案顏色的專案。

![濾鏡影像1](../12-exercises/assets/filters-walkthrough-1.png)

## 要遵循的步驟

1. 建立「超出基本對應」情境的原地復製版，並將其命名為「使用強大的篩選器」。

   **在建立Workfront專案模組之前新增篩選器，以僅允許建立紅色專案。**

   ![濾鏡影像2](../12-exercises/assets/filters-walkthrough-2.png)

1. 按一下連線模組的虛線，或按一下扳手並選取「設定篩選器」，以新增篩選器。
1. 使用「標籤」欄位將篩選器命名為「僅限紅色專案」。
1. 在「條件」欄位中，對應「專案顏色」欄位（CSV檔案中的「欄3」）。 選取「等於」（不區分大小寫）運運算元，然後輸入「紅色」。
1. 按一下「確定」。

   ![濾鏡影像3](../12-exercises/assets/filters-walkthrough-3.png)

   **測試篩選器並驗證結果。**

1. 按一下「儲存」以儲存情境，然後按一下「執行一次」。
1. 按一下篩選的執行檢查器，檢視篩選如何檢查每個套件組合，以及篩選如何通過或無法繼續前往「建立Workfront專案」模組。

   ![濾鏡影像4](../12-exercises/assets/filters-walkthrough-4.png)

1. 尋找在您的Workfront執行個體中建立的專案。
