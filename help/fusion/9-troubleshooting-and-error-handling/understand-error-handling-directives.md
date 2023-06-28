---
title: 瞭解處理指示詞的錯誤
description: 瞭解允許繼續執行的錯誤處理常式指令和停止執行的錯誤處理常式指令，請參閱 [!DNL Adobe Workfront Fusion].
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-9064
exl-id: cb8d0880-73d2-4118-b800-a126f8509309
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 0%

---

# 瞭解處理指示詞的錯誤

在本影片中，您將瞭解：

* 允許繼續執行的三個錯誤處理常式指令
* 停止執行的兩個錯誤處理常式指示詞

>[!VIDEO](https://video.tv.adobe.com/v/335305/?quality=12&learn=on)

## 指令 — 案例繼續

### 繼續

* 會指定替代輸出，並提供給發生錯誤的模組。
* 後續模組會進行處理。
* 案例執行狀態會標示為「成功」。

![Resume指示詞的影像](assets/troubleshooting-and-error-handling-2.png)

### 中斷

* 情境執行的狀態會儲存在未完成執行的佇列中，而錯誤可以手動解決。 不過，這裡有一些例外情況。
* 後續模組不會進行處理。
* 如果有未處理的組合，情境執行會正常繼續。
* 情境執行狀態會標示為「警告」。

![Break指示詞的影像](assets/troubleshooting-and-error-handling-3.png)

### 忽略

* 會忽略錯誤，且不會處理後續模組。
* 如果有未處理的組合，情境執行會正常繼續。
* 案例執行狀態會標示為「成功」。

![Ignore指示詞的影像](assets/troubleshooting-and-error-handling-4.png)

## 指示 — 案例停止

### 復原

* 案例執行會立即停止，並且所有模組上的復原階段會啟動，以嘗試將所有模組回復到其初始狀態。
* 後續模組不會進行處理。
* 除了一些錯誤型別，在「案例」設定下指定的「連續錯誤數」後，將停用案例。
* 案例執行狀態會標示為「錯誤」。

>[!NOTE]
>
>如果沒有將錯誤處理常式路由附加到模組，並且未勾選「案例」設定下的「允許儲存不完整的執行」設定時，此為預設行為。

![Rollback指令的影像](assets/troubleshooting-and-error-handling-5.png)

### 認可

* 會忽略錯誤，且不會處理後續模組。
* 如果有未處理的組合，情境執行會正常繼續。
* 案例執行狀態會標示為「成功」。

![認可指示詞的影像](assets/troubleshooting-and-error-handling-6.png)
