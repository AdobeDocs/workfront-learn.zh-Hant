---
title: 使用自動化工作流程上傳校樣
description: 瞭解何時使用自動化校訂工作流程、如何使用校訂範本套用工作流程，以及如何從頭開始設定自動化工作流程。
activity: use
feature: Workfront Proof
type: Tutorial
role: User
level: Beginner
team: Technical Marketing
thumbnail: 335133.png
jira: KT-8833
exl-id: 8301ef00-1f47-4779-aa35-c735b66fdcac
doc-type: video
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '575'
ht-degree: 0%

---

# 使用自動化工作流程上傳校樣

在本影片中，您將瞭解：

* 何時可以使用自動化校樣工作流程
* 如何使用校樣範本套用工作流程
* 如何從頭開始設定自動化工作流程

>[!VIDEO](https://video.tv.adobe.com/v/335133/?quality=12&learn=on)



## 其他校訂工作流程設定

校樣上傳視窗底部的設定是選用的，因此請洽詢您的組織，以瞭解是否以及如何使用它們。

![的影像 [!UICONTROL 新校訂]視窗的 [!UICONTROL 階段設定] 反白顯示。](assets/additional-proof-workflow-settings.png)

* **[!UICONTROL 鎖定階段] —** 這可防止此工作流程階段中的人在工作流程階段完成之後發表評論或變更決定。
* **[!UICONTROL 將主要決定權轉移至] —** 指定主要決策者，加速校訂程式。 設定後， [!DNL Workfront] 將這個人的證明決定視為決定。 一旦該人員做出決定，階段就會結束，不需要其他決定。
* **[!UICONTROL 此階段只需要一個決定] —** 另一種簡化校訂流程的方法是只需對校訂做出一個決定。 開啟此功能後，無論您在該階段擁有多少核准者，一旦其中任何一位核准者做出決定，該階段即已完成。
* **[!UICONTROL 將此階段設為私人] —** 依預設，所有階段中的每個人都可以看到校訂上的註解。 按一下方塊，以防止其他階段的校樣收件者看到在此階段所做的評論。

在校樣上傳視窗的底部是幾個會影響校樣安全性的校樣設定，例如要求登入才能檢視校樣。

<!--
Learn more about these in the Proof settings section of the Configure a proof article.
-->

![的影像 [!UICONTROL 校訂設定] 區域上傳校樣。](assets/additional-proof-workflow-settings-2.png)

<!--
### Learn more
* Automated workflow overview
* Automated workflow stages overview
-->

<!--
### Guides
* Plan an advanced workflow worksheet
-->

## 你為什麼在校訂工作流程中？

您會注意到您位於校樣收件者清單中，因為上傳校樣的是您。 這也讓您成為校訂所有者，這可讓您編輯校訂、允許您變更工作流程設定或上傳新版本等。

![校樣上傳視窗的影像中，校樣擁有者在收件者清單中反白顯示。](assets/proof-owner.png)

如果您只是上傳校樣，但其他人將管理工作流程，您可以按一下 [!UICONTROL 所有者] 連結並輸入其名稱。 如果除了原始上傳程式以外的其他人要上傳版本，則建議使用此選項。

## 輪到你了

>[!IMPORTANT]
>
>別忘了提醒您的同事，作為Workfront培訓的一部分，您向他們傳送了證明。


使用進階工作流程上傳校訂。 如果您的組織已設定校訂範本，請選取您的團隊使用的範本，然後進行一些調整。

* 調整電子郵件警示，以便在校樣上發生活動時不會通知任何人。
* 第一個階段應有2名稽核者/核准者。
* 第二個階段應該只有1個檢閱者/核准者。

如果您的組織尚未建立校訂範本，請從頭開始設定兩階段工作流程。

* 將您自己和您最愛的同事指派到第一個階段。
* 將建立校樣後的第一個階段期限設定為1天。
* 將另一個最愛的同事指派給第二個階段。
* 當第一個階段的截止日期已過時，讓階段開始。
* 給此階段的人2天時間完成審查，但必須在中午前完成。


