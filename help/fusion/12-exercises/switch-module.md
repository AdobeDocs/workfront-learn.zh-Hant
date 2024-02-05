---
title: 切換模組
description: 瞭解在必須執行比較複雜或動態的資料轉換時，如何使用「切換」模組。
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
workflow-type: ht
source-wordcount: '319'
ht-degree: 100%

---

# 切換模組

瞭解在必須執行比較複雜或動態的資料轉換時，如何使用「切換」模組。

## 練習概觀

在產品試用中搜尋直接郵件專案，然後根據附加在專案上的自訂欄位中選取的值，變更每個專案的名稱。

![切換模組影像 1](../12-exercises/assets/switch-module-walkthrough-1.png)

## 執行步驟

1. 建立新情境並命名為「使用切換模組」
1. 對於觸發模組，請使用 Workfront「搜尋」模組。
1. 設定您的 Workfront 連線，並設定記錄類型為「專案」。
1. 在「搜尋條件」中，指定您只要檢視在「通路」自訂欄位中有值的專案。
1. 對於輸出，選取「ID」、「名稱」、「參考編號」和「通路」自訂欄位。

   ![切換模組影像 2](../12-exercises/assets/switch-module-walkthrough-2.png)

1. 新增來自「工具」的「切換」模組。
1. 對於「輸入」欄位，對應來自「搜尋」模組的「通路」自訂欄位。

   ![切換模組影像 3](../12-exercises/assets/switch-module-walkthrough-3.png)

1. 接著針對來自「通路」自訂欄位的每個可能值新增案例。可能的值會存入「模式」欄位。您希望輸出欄位包含特定的 3 個字母代碼，而後面接著是專案參考編號和專案名稱。

   **您的對應面板應如下所示：**

   ![切換模組影像 4](../12-exercises/assets/switch-module-walkthrough-4.png)

1. 您可以根據需要新增更多案例，數量不限。請注意底部的「否則」欄位。若輸入值不符合任一案例時便會使用此欄位。

   **更新 Workfront 中的專案名稱。**

   ![切換模組影像 5](../12-exercises/assets/switch-module-walkthrough-5.png)

1. 新增 Workfront「更新記錄」模組。
1. 在「ID」欄位中，對應到來自觸發模組的 ID。
1. 將「記錄類型」設為「專案」。
1. 從「選取對應欄位」區段選取「名稱」欄位，然後對應到來自「切換」模組的輸出。
1. 請儲存您的情境並按一下「執行一次」。在您的產品試用中檢視已更新的專案名稱。
