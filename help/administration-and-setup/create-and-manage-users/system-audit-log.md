---
title: 了解系統審核日誌
description: 了解如何使用系統稽核記錄來檢閱變更的時間及項目的執行時間。
feature: System Setup and Administration
activity: deploy
type: Tutorial
team: Technical Marketing
role: Admin
level: Beginner, Intermediate
thumbnail: 10040.jpeg
kt: 10040
exl-id: 9de6fd40-10fb-47a6-b186-3a38c411f1ac
source-git-commit: adf12d7846d2a1b4c32513a3955c080905044576
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---

# 了解系統稽核記錄

系統審核日誌是系統管理員監視中發生情況的最佳方式 [!DNL Workfront]. 請將日誌視為您的真相來源，了解誰做了哪些變更，以及何時進行了哪些變更。

前往 [!UICONTROL 偏好設定] 區段 [!UICONTROL 設定] 的上界。 依預設，您會看到過去七天的資料。 變更篩選條件，以查看不同日期範圍的資料。

當使用者執行特定動作時， [!UICONTROL Workfront] 記錄在 [!UICONTROL 稽核記錄] 區段 [!UICONTROL 設定] 的上界。

![[!UICONTROL 記錄類型] 下拉式功能表 [!UICONTROL 稽核記錄] 頁面 [!UICONTROL 設定]](assets/admin-fund-audit-log-1.png)

記錄或記錄的每個動作都會顯示：

* 變更的日期和時間
* 記錄類型
* 完成動作的使用者名稱
* 物件
* 與動作相關聯的任何詳細資料
* IP位址

![[!UICONTROL 稽核記錄] 清單](assets/admin-fund-audit-log-2.JPG)

## 導出審核日誌

導出審核日誌資料可讓系統管理員與內部/外部審計員或安全專家共用資訊。 一些組織要求保留某些日誌以遵守網路安全法規。 其他人需要將資訊導入安全系統進行分析。

稽核記錄檔可匯出為CSV（逗號分隔值）檔案，並可開啟至試算表應用程式或純文字編輯器。 匯出一次限制為50,000列，因此如果總數超過50,000，請使用篩選器來縮小清單。

![[!UICONTROL 匯出] 按鈕 [!UICONTROL 稽核記錄] 頁面](assets/admin-fund-audit-log-3.png)

<!---
learn more URLs
Audit logs
Managing audit logs
--->
