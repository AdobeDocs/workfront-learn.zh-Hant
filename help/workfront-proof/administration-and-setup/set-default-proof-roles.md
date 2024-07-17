---
title: 設定預設校訂角色
description: 了解在建立新使用者時或是有人開啟校訂時，要如何設定所指派的預設校訂角色。
activity: use
team: Technical Marketing
feature: Workfront Proof
type: Tutorial
role: User, Admin
level: Intermediate
thumbnail: set-default-proof-roles.png
jira: KT-10235
last-substantial-update: 2024-01-24T00:00:00Z
exl-id: 77dfb9f1-3242-47ca-a0ce-203b535af156
source-git-commit: 30748311c14fb8aa6b10c03a74e83f46bdb5dfbf
workflow-type: tm+mt
source-wordcount: '359'
ht-degree: 100%

---

# 設定預設校訂角色



第一個預設設定是在建立新使用者或有人員開啟校訂時，決定要指派哪一種預設校訂角色。

校訂角色決定使用者可以對校訂執行什麼動作，例如只能檢視、留下註解、核准等。[!DNL Workfront] 建議預設校訂角色應該適用於全部使用者，讓新增校訂收件者及設定工作流程的工作更快速且輕鬆。

![上傳校訂時可以選取校訂角色](assets/proof-system-setups-proof-role-example.png)

但是，在上傳個別的校訂時可以變更這個預設校訂角色，確保每個人都能夠履行他們在檢閱和核准流程中所負責的角色。


## 設定預設校訂角色

1. 在[!UICONTROL 主選單]中選取「**設定**」。
1. 從左側選單選取「**檢閱與核准**」。
1. 對於作為「指定收件者」的新 [!DNL Workfront] 使用者以及校訂訪客使用者，按一下所需的預設校訂角色旁邊的按鈕。「指定收件者」是指加入到校訂工作流程中的任何人，無論是手動或透過工作流程範本新增。
1. 對於作為「非收件者」的新 [!DNL Workfront] 使用者和校訂訪客使用者，按一下所需預設校訂角色旁邊的按鈕。這些通常是可以存取校訂但是並未獲得指派參與工作流程的 [!DNL Workfront] 使用者。
1. 儲存變更。

![Workfront 中的檢閱與核准設定](assets/proof-system-setups-workfront-defaults.png)

考慮大部分使用者和訪客被新增到校訂工作流程時，預期會執行的工作。這些應該是您的預設值。

## 最佳實務

| 最佳實務 | 原因說明 |
|---|---|
| 對於 Workfront 中「開啟文件校訂的非收件者之角色」設定，請僅使用「唯讀」或「檢閱者」。 | 這項設定的其他選項皆要求做出校訂決定，而這樣可能會破壞訂工作流程。一般而言，未加入校訂工作流程的人員只需要檢視校訂或留下註解，而不必實際核准校訂，因為「唯讀」或「檢閱者」選項是最佳選擇。 <br> <br>備註：這項設定位在 Workfront 主選單 >「設定」>「檢閱和核准」。 |
