---
title: 設定預設校訂角色
description: 瞭解在建立新使用者時或是有人開啟校訂時，要如何設定所指派的預設校訂角色。
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
ht-degree: 52%

---

# 設定預設校訂角色



第一個預設設定是在建立新使用者或有人員開啟校訂時，決定要指派哪一種預設校訂角色。

校訂角色決定使用者可以對校訂執行什麼動作，例如只能檢視、留下註解、核准等。[!DNL Workfront] 建議預設校訂角色應該適用於全部使用者，讓新增校訂收件者及設定工作流程的工作更快速且輕鬆。

![上傳校訂時可以選取校訂角色](assets/proof-system-setups-proof-role-example.png)

但是，在上傳個別的校訂時可以變更這個預設校訂角色，確保每個人都能夠履行他們在檢閱和核准流程中所負責的角色。


## 設定預設校訂角色

1. 在[!UICONTROL 主選單]中選取「**設定**」。
1. 從左側選單選取「**檢閱與核准**」。
1. 按一下兩個新專案的所需預設校樣角色旁的按鈕 [!DNL Workfront] 「指定收件者」的使用者和訪客校訂使用者 — 手動或透過工作流程範本新增到校訂工作流程的任何人。
1. 按一下兩個新專案的所需預設校樣角色旁的按鈕 [!DNL Workfront] 「非收件者」使用者的使用者和訪客校訂使用者。 這些通常是 [!DNL Workfront] 有權存取校訂但未獲指派工作流程的使用者。
1. 儲存變更。

![Workfront 中的檢閱與核准設定](assets/proof-system-setups-workfront-defaults.png)

考慮大部分使用者和訪客被新增到校訂工作流程時，預期會執行的工作。這些應該是您的預設值。

## 最佳實務

| 最佳實務 | 原因如下 |
|---|---|
| 對Workfront中的「開啟檔案校訂的非收件者角色」設定使用唯讀或檢閱者。 | 此設定的其他選項都要求做出校訂決定，這可能會破壞您的校訂工作流程。 一般而言，未新增至校訂工作流程的人只需要檢視校訂或發表評論，實際上並不核准校訂，因此「唯讀」或「檢閱者」選項是您的最佳選擇。 <br> <br>注意：此設定可在Workfront的主要功能表>設定>檢閱和核准中找到。 |
