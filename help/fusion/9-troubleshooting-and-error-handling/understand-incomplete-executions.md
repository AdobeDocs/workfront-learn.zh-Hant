---
title: 瞭解未完成的執行
description: 瞭解執行不完整是什麼以及如何處理導致執行不完整的錯誤 [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9066
exl-id: 3b7bf669-4736-4ba5-bcec-0d3fe0b2ce74
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# 瞭解未完成的執行

未完成的執行可以儲存在Workfront Fusion中，以便稍後檢視和解決。 瞭解如何善用此令人驚豔的功能。

在本影片中，您將瞭解：

* 未完成的執行是什麼
* 如何處理導致執行不完整的錯誤

>[!VIDEO](https://video.tv.adobe.com/v/335307/?quality=12&learn=on)

## 導致執行不完整的錯誤

有幾種錯誤類別會導致儲存不完整的執行。

收到的不同錯誤型別將取決於您所連線的API。 此錯誤可能是由於不完整或錯誤的資料所導致的驗證錯誤，大部分是因為遺漏了預期的專案，而無法成功處理通過模組的所有資料。 或者，由於暫時或長期的連線失敗（例如，在連線至電子郵件或遠端FTP伺服器期間），最終目的地的可用性可能會發生錯誤。

如果情境中的第一個模組發生錯誤，執行會立即停止，且不會儲存不完整的執行。

如果任何其他模組發生錯誤，且沒有附加錯誤處理常式路由，則：

* 如果錯誤型別為ConnectionError、RateLimitError、OutOfSpaceError或ModuleTimeoutError，則會儲存不完整的執行記錄WITH自動重試。
* 如果錯誤型別為DataError、InvalidConfigurationError、InvalidAccessTokenError、UnexpectedError、MaxFileSizeExceededError或MaxResultsExceededError，則會儲存不完整的執行記錄（沒有自動重試）。
* 如果錯誤型別不是上述型別，則執行會失敗。

## 想要瞭解更多？ 我們建議採取下列步驟：

[Workfront Fusion檔案](https://experienceleague.adobe.com/docs/workfront/using/adobe-workfront-fusion/workfront-fusion-2.html?lang=en)
