---
title: 切換模組
description: 瞭解在您需要執行更複雜或動態的資料轉換時，如何使用交換器模組。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11052
thumbnail: KT11052.png
exl-id: 1b810168-582d-4d7d-b061-d152af546bc8
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 0%

---

# 切換模組

瞭解在您需要執行更複雜或動態的資料轉換時，如何使用交換器模組。

## 練習概述

在您的測試方案中搜尋直接郵件專案，然後根據附加至專案的自訂欄位中選取的值，變更每個專案的名稱。

![切換模組影像1](../12-exercises/assets/switch-module-walkthrough-1.png)

## 要遵循的步驟

1. 建立新情境，並將其命名為「使用交換器模組」。
1. 對於觸發程式模組，請使用Workfront搜尋模組。
1. 設定您的Workfront連線，並將記錄型別設定為「專案」。
1. 在「搜尋」條件中，指定您只想在「管道」自訂欄位中檢視具有值的專案。
1. 對於輸出，請選取ID、名稱、參考編號和管道自訂欄位。

   ![切換模組影像2](../12-exercises/assets/switch-module-walkthrough-2.png)

1. 從「工具」中新增「交換器」模組。
1. 對於「輸入」欄位，從搜尋模組對應「頻道」自訂欄位。

   ![切換模組影像3](../12-exercises/assets/switch-module-walkthrough-3.png)

1. 接下來，針對來自管道自訂欄位的每個可能值新增案例。 可能的值會進入「模式」欄位。 您希望輸出欄位包含特定的3個字母代碼，後面接著專案參考編號，然後是專案名稱。

   **您的對應面板應如下所示：**

   ![切換模組影像4](../12-exercises/assets/switch-module-walkthrough-4.png)

1. 您可以新增任意數量的其他案例。 請注意底部的「其他」欄位。 如果輸入值不符合任何大小寫，則會使用此值。

   **更新Workfront中的專案名稱。**

   ![切換模組影像5](../12-exercises/assets/switch-module-walkthrough-5.png)

1. 新增Workfront更新記錄模組。
1. 在ID欄位中，對應至觸發模組的ID。
1. 將記錄型別設定為專案。
1. 從「選擇要對應的欄位」區段中選取「名稱」欄位，並將其對應到「交換機」模組的輸出。
1. 儲存您的情境並執行一次。 檢視測試磁碟機中更新的專案名稱。
