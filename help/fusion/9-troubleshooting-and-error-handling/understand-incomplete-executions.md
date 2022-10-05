---
title: 了解未完成的執行
description: 了解何謂不完整的執行，以及如何處理導致中執行不完整的錯誤 [!DNL Adobe Workfront Fusion].
activity: use
doc-type: feature video
team: Technical Marketing
kt: Jira ticket
exl-id: 3b7bf669-4736-4ba5-bcec-0d3fe0b2ce74
source-git-commit: a0aa8328842d2db1235edc42664eb0b18f4038e4
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# 了解未完成的執行

不完整的執行可儲存在Workfront Fusion中，以供稍後審核和解決。 了解如何善用這項令人驚異的功能。

在此影片中，您將學習：

* 未完成的執行
* 如何處理導致執行不完整的錯誤

>[!VIDEO](https://video.tv.adobe.com/v/335307/?quality=12)

## 導致執行不完整的錯誤

存在幾類錯誤，導致儲存不完整的執行。

收到的不同錯誤類型取決於您所連線的API。 錯誤可能是因不完整或錯誤資料所導致的驗證錯誤，主要是因為遺漏了預期的項目，而這是為了成功處理通過模組的所有資料。 或者，由於暫時或長期連線失敗（例如連線至電子郵件或遠端FTP伺服器），最終目的地無法使用而造成錯誤。

如果情境中的第一個模組發生錯誤，則執行會立即停止，且不會儲存不完整的執行。

如果任何其他模組發生錯誤且未附加錯誤處理程式路由，則：

* 如果錯誤類型為ConnectionError、RateLimitError、OutOfSpaceError或ModuleTimeoutError，則會儲存不完整的執行記錄WITH auto-retry。
* 如果錯誤類型為DataError、InvalidConfigurationError、InvalidAccessTokenError、UnimpedError、MaxFileSizeExceededError或MaxResultsExceededError，則會儲存不完整的執行記錄WITH auto-retry。
* 如果錯誤類型不是上述任何值，則執行會失敗。

## 想要進一步了解嗎？ 我們建議下列項目：

[Workfront Fusion檔案](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
