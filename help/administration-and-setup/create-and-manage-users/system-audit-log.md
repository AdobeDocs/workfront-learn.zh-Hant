---
title: 瞭解系統稽核記錄
description: 瞭解如何使用系統稽核記錄，以檢閱何時進行變更以及何時進行專案。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner, Intermediate
thumbnail: 10040.jpeg
jira: KT-10040
exl-id: 9de6fd40-10fb-47a6-b186-3a38c411f1ac
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---

# 瞭解系統稽核記錄

系統稽核記錄是系統管理員監視目前狀況的最佳方式 [!DNL Workfront]. 將記錄檔視為誰在何時做了哪些變更的真實來源。

前往以下位置存取稽核記錄： [!UICONTROL 偏好設定] 中的區段 [!UICONTROL 設定] 區域。 依預設，您會看到過去七天的資料。 變更篩選條件以檢視不同日期範圍內的資料。

當使用者執行某些動作時， [!UICONTROL Workfront] 記錄於 [!UICONTROL 稽核記錄] 部分 [!UICONTROL 設定] 區域。

![[!UICONTROL 記錄型別] 上的下拉式功能表 [!UICONTROL 稽核記錄] 第頁於 [!UICONTROL 設定]](assets/admin-fund-audit-log-1.png)

記錄或記錄的每個動作都會顯示：

* 變更的日期和時間
* 記錄型別
* 完成動作之使用者的名稱
* 物件
* 與動作關聯的任何詳細資訊
* ip位址

![[!UICONTROL 稽核記錄] 清單](assets/admin-fund-audit-log-2.JPG)

## 匯出稽核記錄

匯出稽核記錄資料可讓系統管理員與內部/外部稽核員或安全專家共用資訊。 有些組織會要求保留某些記錄檔，以符合網路安全法規。 其他則需要匯入安全性系統的資訊進行分析。

稽核記錄可以匯出為CSV （逗號分隔值）檔案，該檔案可以開啟至試算表應用程式或純文字編輯器。 匯出限製為一次最多50,000列，因此如果總數超過50,000，請使用篩選器縮小清單範圍。

![[!UICONTROL 匯出] 按鈕開啟 [!UICONTROL 稽核記錄] 頁面](assets/admin-fund-audit-log-3.png)

<!---
learn more URLs
Audit logs
Managing audit logs
--->
