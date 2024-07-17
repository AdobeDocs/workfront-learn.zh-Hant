---
title: 最佳實務 - 篩選器、視圖與分組
description: 探索 Adobe Workfront 專家提供的有關設定、管理和使用 Workfront 篩選器、視圖和分組的最佳實務建議。
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
jira: KT-10911
exl-id: 845aa0b4-3fe9-4bc1-9dde-2f22c537e758
source-git-commit: 0ff5accae867f07cc31ac2be7b0c12981412346e
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 100%

---

# 最佳實務 - 篩選器、視圖與分組

## 什麼是 Adobe Workfront「最佳實務」？

最佳實務是代表有效果、有效率之行動方針的準則；您和公司的使用者可以輕鬆採用；並且可以成功複製到整個組織。

當您檢閱這些建議時，請記住，有一些 Workfront 最佳實務是通用的，而其他做法可能針對特定主題。將這些最佳實務視為框架，作為設定和使用 Workfront 系統時的指引。

## 導覽此頁面

當您捲動瀏覽此頁面時，您會先找到該主題所有最佳實務的高層次清單。這樣您便可以檢視建議而無需深入了解詳細的「原因」。

「為什麼這些是最佳實務？」區域，位在高層次清單之後，詳細說明一部分的最佳實務，以及為什麼這些實務被認定為您的 Workfront 執行個體應該考慮執行的流程、工具等。

</br>
</br>

## 篩選器、視圖與分組最佳實務

* 在物件清單上利用篩選器、視圖和分組來取得所需的資料，減少您建立的自訂報告數量。

* 使用版本配置範本中的清單控制項來隱藏常用物件 (專案、任務、方案等) 的非必要篩選器、視圖和分組。

* 利用版本配置範本上的清單控制項來共用與貴組織之工作流程和程序相關的自訂篩選器、視圖和分組。

* 在建立專案狀態、任務狀態或問題狀態的篩選器時，請使用「(物件) >> 狀態等同於」欄位的來源/欄位名稱搭配「等於」修飾元，而不是使用「專案 >> 狀態」欄位的來源/欄位名稱。

</br>
</br>

## 為什麼這些是最佳實務？

**最佳實務**

在物件清單上利用篩選器、視圖和分組來取得所需的資料，減少您建立的自訂報告數量。

**原因說明**

針對您想查看每個段落的資料建立一次性的報告不但耗費時間，也讓 Workfront 系統切分成多個區塊。

有關如何建立附有提示的報告說明，請參閱「[了解報告設定](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/report-settings.html)」影片中標有「如何設定和使用報告提示」的章節。

有關如何建立附有自訂提示的報告說明，請參閱「[建立自訂提示](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/custom-prompts.html)」。

</br>
</br>

**最佳實務**

使用版本配置範本中的清單控制項來隱藏常用物件 (專案、任務、方案等) 的非必要篩選器、視圖和分組。

**原因說明**

數量越少，獲得越多。隱藏與使用者日常工作流程無關的篩選器、視圖和分組清單選項，可以縮小清單範圍，讓使用者更容易迅速找到他們需要的內容。

有關如何使用版本配置範本隱藏篩選器、視圖或分組的說明，請參閱「[使用版本配置範本自訂報告清單](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/administration-and-setup/layout-templates/customize-reporting-lists-with-layout-templates.html)」。

</br>
</br>

**最佳實務**

利用版本配置範本上的清單控制項來共用與貴組織之工作流程和程序相關的自訂篩選器、視圖和分組。

**原因說明**

若您已經建立篩選器、視圖和分組來顯示與使用者日常流程相關的特定資訊，透過版本配置範本可以輕鬆共用這些項目。這樣一來，便能確保獲得指派該版本配置範本的每個人擁有與其工作流程相關的篩選器、視圖和分組選項。

透過版本配置範本來自訂您要讓使用者看見的資訊，也節省系統和群組管理員的時間，因為他們不必分別共用每一個篩選器、視圖或分組。

有關如何使用版本配置範本共用篩選器、視圖或分組的說明，請參閱「[使用版本配置範本自訂報告清單](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/administration-and-setup/layout-templates/customize-reporting-lists-with-layout-templates.html)」。

</br>
</br>

**最佳實務**

在建立專案狀態、任務狀態或問題狀態的篩選器時，請使用「(物件) >> 狀態等同於」欄位的來源/欄位名稱搭配「等於」修飾元，而不是使用「專案 >> 狀態」欄位的來源/欄位名稱。

**原因說明**

使用「(物件) >> 等同於」，您包含了狀態設定中將該特定狀態指派給「等同於」欄位的所有自訂欄位。而把篩選器設定為「(物件)>> 狀態 > 等於」，會要求您為篩選器選取特定的狀態。若您必須考慮各個篩選器中的新狀態，則可能造成維護的難題。每個篩選器必須開啟並更新為新狀態。

例如，如果您想查看所有目前的專案，您可以將篩選器設定為讀取「專案 >> 狀態 > 等於 > 目前」。但是，如果有人新增名為「進行中」的自訂狀態並將其等同於「目前」，該篩選器無法找到具有「進行中」狀態的專案。但是，若您使用「專案 >> 狀態等同於 > 等於 > 目前」，則篩選器會尋找狀態為「目前」或「進行中」的物件，因為兩者在「等同於」欄位均是「目前」。
