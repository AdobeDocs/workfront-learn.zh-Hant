---
title: 瞭解錯誤處理指示
description: 瞭解  [!DNL Adobe Workfront Fusion] 中允許繼續執行以及使執行停止的錯誤處理常式指示。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9064
exl-id: cb8d0880-73d2-4118-b800-a126f8509309
recommendations: noDisplay,catalog
doc-type: video
source-git-commit: bbdf99c6bc1be714077fd94fc3f8325394de36b3
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 100%

---

# 瞭解錯誤處理指示

觀看這段影片，您將會瞭解：

* 允許繼續執行的三個錯誤處理常式指示
* 使執行停止的兩個錯誤處理常式指示

>[!VIDEO](https://video.tv.adobe.com/v/335305/?quality=12&learn=on&enablevpops=1)

## 指示 — 情境繼續

### 繼續

* 指定替代輸出並提供給發生錯誤的模組。
* 接著處理後續的模組。
* 情境執行狀態標記為「成功」。

![影像顯示「繼續」指示](assets/troubleshooting-and-error-handling-2.png)

### 中斷

* 情境執行的狀態儲存在未完成執行作業的佇列中，而錯誤可以手動解決。不過也有一些例外狀況，如此處所述。
* 後續的模組並未進行處理。
* 若有未處理的套件，情境執行將按正常情況繼續。
* 情境執行狀態標記為「警告」。

![影像顯示「中斷」指示](assets/troubleshooting-and-error-handling-3.png)

### 忽略

* 忽略錯誤，而且不處理後續的模組。
* 若有未處理的套件，情境執行將按正常情況繼續。
* 情境執行狀態標記為「成功」。

![影像顯示「忽略」指示](assets/troubleshooting-and-error-handling-4.png)

## 指示 — 情境停止

### 復原

* 情境執行立即停止，並在所有模組上啟動復原階段，試圖將它們全部恢復到初始狀態。
* 後續的模組並未進行處理。
* 除少數錯誤類型外，在到達「情境」設定下指定的「連續錯誤數」之後，該情境將被停用。
* 情境執行狀態標記為「錯誤」。

>[!NOTE]
>
>如果模組上並未附加任何錯誤處理常式，而且未勾選「情境」設定之下的「允許儲存未完成的執行作業」設定，這是預設的行為。

![影像顯示「復原」指示](assets/troubleshooting-and-error-handling-5.png)

### 認可

* 忽略錯誤，而且不處理後續的模組。
* 若有未處理的套件，情境執行將按正常情況繼續。
* 情境執行狀態標記為「成功」。

![影像顯示「認可」指示](assets/troubleshooting-and-error-handling-6.png)
