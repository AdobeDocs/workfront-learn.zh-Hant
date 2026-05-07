---
title: 瞭解未完成的執行作業
description: 瞭解在  [!DNL Adobe Workfront Fusion] 中什麼是未完成的執行作業，以及如何處理造成執行作業未完成的錯誤。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9066
exl-id: 3b7bf669-4736-4ba5-bcec-0d3fe0b2ce74
recommendations: noDisplay,catalog
doc-type: video
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
autotag-review: '2026-05-06T16:07:51.152Z'
source-git-commit: 9f00285646af281d6c4d93eb792f4c38eedefb40
workflow-type: tm+mt
source-wordcount: 280
ht-degree: 93%

---

# 瞭解未完成的執行作業

未完成的執行作業可以儲存在 Workfront Fusion 中，稍後可以進行審閱並解決問題。 瞭解如何善用這項驚人的功能。

觀看這段影片，您將會瞭解：

* 什麼是未完成的執行作業
* 如何處理造成執行作業未完成的錯誤

>[!VIDEO](https://video.tv.adobe.com/v/335307/?quality=12&learn=on&enablevpops=1)

## 導致執行作業未完成的錯誤

有數種類別的錯誤會造成儲存未完成的執行作業。

根據您所連接的 API，會收到不同類型的錯誤。 該錯誤可能是因為資料不完整或錯誤而引起的驗證錯誤，主要是因為缺少一個本該出現的項目，而我們需要該項目才能成功處理經過模組的所有資料。 或者，可能是最後目標因為連線暫時性或長時間故障 (例如在連線期間連接電子郵件或遠端 FTP 伺服器) 而無法使用所導致的錯誤。

若是情境中第一個模組發生錯誤，會馬上停止執行，不會儲存任何未完成的執行作業。

如果是任何其他模組發生錯誤，而且並未附加任何錯誤處理常式，則：

* 如果錯誤類型是「ConnectionError」、「RateLimitError」、「OutOfSpaceError」或 「ModuleTimeoutError」，則會儲存包含自動重試的未完成執行記錄。
* 如果錯誤類型為「DataError」、「InvalidConfigurationError」、「InvalidAccessTokenError」、「UnexpectedError」、「MaxFileSizeExceededError」或「MaxResultsExceededError」，則儲存不包含自動重試的未完成執行記錄。
* 如果錯誤類型不是上述任何一項，則執行失敗。

## 想要瞭解更多嗎？ 我們建議參閱以下資訊：

[Workfront Fusion 文件](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)
