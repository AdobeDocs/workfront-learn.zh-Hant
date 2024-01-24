---
title: 瞭解電子郵件警報和校訂通知
description: 瞭解  [!DNL  Workfront] 中電子郵件警報和校訂通知之間的區別。
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
thumbnail: email-alert-vs-proof-notifications.png
jira: KT-10174
last-substantial-update: 2024-01-23T00:00:00Z
exl-id: 51423110-960c-46ed-8b4e-6e73c67c42e0
source-git-commit: 731005176bc02e3a4d26d00373931fa7444afeea
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 65%

---

# 瞭解電子郵件警報和校訂通知

電子郵件警報與校訂通知電子郵件不同。當您將新校訂指派給您審閱、校訂延遲，或當有新版本的校訂供您檢視時，您將收到校訂通知電子郵件。

![影像顯示校訂通知電子郵件表示有新校訂內容需要檢閱。](assets/email-alert-1.png)

如果您在上傳校訂時關閉通知選項，則沒有人會收到來自 [!DNL Workfront] 說明有新校訂內容待檢閱的通訊。

電子郵件警報是依據每一位檢閱者/核准者進行設定，最常見是在上傳校訂時設定。預設電子郵件警報型別可能會指派給您的校訂收件者，因此您不需要每次上傳校訂時都進行設定。 請與您的系統管理員討論如何設定這些預設值。

![影像顯示電子郵件警報表示已對校訂做出決定而且有註解待檢閱。](assets/email-alert-2.png)

即使電子郵件警報設為[!UICONTROL 停用]，校訂收件者仍會因為新校訂或新版本而收到通知。

## 最佳實務

| 最佳實務 | 原因如下 |
|---|---|
| 停用Workfront設定中的「當對校訂進行評論時從Workfront傳送電子郵件」設定 | 啟用這項設定後 (預設)，針對校訂上的每一個註解，使用者可能收到多個電子郵件通知，一則來自校訂功能，另一則來自 Workfront 本身。這些重複的通知會導致電子郵件通知中斷和混亂，而且通知會塞滿收件匣，最終可能導致使用者忽略所收到的校訂通知。這進而可能意味著錯過最後期限。 <br> <br>注意：此設定可在Workfront主要功能表>設定>電子郵件>檢閱和核准中找到。 |


