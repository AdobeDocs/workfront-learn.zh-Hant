---
title: 瞭解系統稽核記錄
description: 瞭解如何使用系統稽核記錄來檢閱何時發生變更以及項目何時變更。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner, Intermediate
thumbnail: 10040.jpeg
jira: KT-10040
exl-id: 9de6fd40-10fb-47a6-b186-3a38c411f1ac
source-git-commit: 4568e4e47b719e2dee35357d42674613112a9c43
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 100%

---

# 瞭解系統稽核記錄

系統稽核記錄是系統管理員密切留意 [!DNL Workfront] 上發生什麼事的最好方法。將記錄視為瞭解誰進行變更以及何時進行變更的事實來源。

存取稽核記錄請至「[!UICONTROL 設定]」區域的「[!UICONTROL 偏好設定]」區段。依預設，您看到過去七天的資料。變更篩選條件來查看日期範圍不同的資料。

當使用者執行某些動作時，[!UICONTROL Workfront] 把這些動作記錄在「[!UICONTROL 設定]」區域的「[!UICONTROL 稽核記錄]」區段。

![[!UICONTROL 記錄類型]下拉式選單，位於[!UICONTROL 稽核記錄]頁面，而此頁面位於[!UICONTROL 設定]](assets/admin-fund-audit-log-1.png)

每一個被記錄下來的動作，均顯示以下資料：

* 變更日期和時間
* 記錄類型
* 完成動作的使用者之名稱
* 物件
* 與動作相關的任何詳細資料
* IP 位址。

![[!UICONTROL 稽核記錄]清單](assets/admin-fund-audit-log-2.JPG)

## 匯出稽核記錄

藉由匯出稽核記錄資料，系統管理員能與內部/外部稽核人員或安全專家共用資訊。有些組織要求保留某些記錄，以利遵守網路安全法規。其他人需要把這些資訊匯入安全系統中進行分析。

稽核記錄可以匯出為 CSV (逗號分隔值) 檔案，此檔案可在試算表應用程式或純文字編輯器中開啟。匯出一次限最多 50,000 列，若總數超過 50,000 列，請使用篩選器來縮小清單範圍。

![[!UICONTROL 匯出]按鈕，位於[!UICONTROL 稽核記錄]頁面](assets/admin-fund-audit-log-3.png)

<!--
learn more URLs
Audit logs
Managing audit logs
-->
