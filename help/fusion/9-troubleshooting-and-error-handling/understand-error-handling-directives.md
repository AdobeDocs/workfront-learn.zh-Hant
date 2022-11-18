---
title: 了解錯誤處理指令
description: 了解允許執行繼續的錯誤處理程式指令，以及可停止執行的錯誤處理程式指令，位於 [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
kt: Jira ticket
exl-id: cb8d0880-73d2-4118-b800-a126f8509309
source-git-commit: 58a545120b29a5f492344b89b77235e548e94241
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 0%

---

# 了解錯誤處理指令

在此影片中，您將學習：

* 允許執行繼續的三個錯誤處理程式指令
* 停止執行的兩個錯誤處理程式指令

>[!VIDEO](https://video.tv.adobe.com/v/335305/?quality=12)

## 指令 — 方案繼續

### 繼續

* 指定替換輸出，並提供給遇到錯誤的模組。
* 處理後續模組。
* 方案執行狀態會標示為「成功」。

![恢復指令的映像](assets/troubleshooting-and-error-handling-2.png)

### 插播

* 方案執行的狀態儲存在未完成執行的佇列中，可以手動解決錯誤。 但是，這裡提到了一些例外。
* 不會處理後續模組。
* 如果有未處理的套件組合，則方案執行會正常繼續。
* 方案執行狀態標籤為「警告」。

![Break指令的影像](assets/troubleshooting-and-error-handling-3.png)

### 忽略

* 系統會忽略錯誤，且不會處理後續模組。
* 如果有未處理的套件組合，則方案執行會正常繼續。
* 方案執行狀態會標示為「成功」。

![忽略指令的映像](assets/troubleshooting-and-error-handling-4.png)

## 指令 — 方案停止

### 回復

* 方案執行立即停止，並在所有模組上啟動回滾階段，以嘗試將所有模組恢復到其初始狀態。
* 不會處理後續模組。
* 除非有一些錯誤類型，否則藍本會在「藍本」設定下指定的「連續錯誤數」後停用。
* 方案執行狀態被標籤為「錯誤」。

>[!NOTE]
>
>如果未將錯誤處理程式路由附加到模組，且未選中「方案」設定下的「允許儲存不完整的執行」設定，則此為預設行為。

![回滾指令的映像](assets/troubleshooting-and-error-handling-5.png)

### 認可

* 系統會忽略錯誤，且不會處理後續模組。
* 如果有未處理的套件組合，則方案執行會正常繼續。
* 方案執行狀態會標示為「成功」。

![提交指令的映像](assets/troubleshooting-and-error-handling-6.png)
