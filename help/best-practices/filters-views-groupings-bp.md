---
title: 最佳實務 - 篩選器、視圖與分組
description: 探索 Adobe Workfront 專家提供的有關設定、管理和使用 Workfront 篩選器、視圖和分組的最佳實務建議。
feature: Reports and Dashboards
role: Admin, Leader, User
level: Beginner
jira: KT-10911
exl-id: 845aa0b4-3fe9-4bc1-9dde-2f22c537e758
source-git-commit: 0c822b5be5272c5b638039d83294b00d25c32141
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 71%

---

# 最佳實務 - 篩選器、視圖與分組

## 什麼是 Adobe Workfront「最佳實務」？

最佳實務是代表有效果、有效率之行動方針的準則；您和公司的使用者可以輕鬆採用；並且可以成功複製到整個組織。

當您檢閱這些建議時，請記住，有一些 Workfront 最佳實務是通用的，而其他做法可能針對特定主題。將這些最佳實務視為框架，作為設定和使用 Workfront 系統時的指引。

## 導覽此頁面

當您捲動瀏覽此頁面時，您會先找到該主題所有最佳實務的高層次清單。這樣您便可以檢視建議而無需深入瞭解詳細的「原因」。

「為什麼這些是最佳實務？」區域，位在高層次清單之後，詳細說明一部分的最佳實務，以及為什麼這些實務被認定為您的 Workfront 執行個體應該考慮執行的流程、工具等。

</br>
</br>

## 篩選器、視圖與分組最佳實務

* 在物件清單上利用篩選器、視圖和分組來取得所需的資料，減少您建立的自訂報告數量。

* 使用版面範本中的清單控制項來隱藏常用物件 (專案、任務、方案等) 的非必要篩選器、視圖和分組。

* 透過版面配置範本的清單控制項，共用與貴組織工作流程和流程相關的自訂篩選器、檢視和群組。

* 在建立專案狀態、任務狀態或問題狀態的篩選器時，請使用「(物件) >> 狀態等同於」欄位的來源/欄位名稱搭配「等於」修飾元，而不是使用「專案 >> 狀態」欄位的來源/欄位名稱。

</br>
</br>

## 為什麼這些是最佳實務？

**最佳實務**

在物件清單上利用篩選器、視圖和分組來取得所需的資料，減少您建立的自訂報告數量。

**原因說明**

針對您想查看每個段落的資料建立一次性的報告不但耗費時間，也讓 Workfront 系統切分成多個區塊。

如需有關如何建立具有提示的報表的說明，請參閱中標示為「如何設定及使用報表提示」的章節。 [瞭解報表設定](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/basic-reporting/report-settings.html).

如需如何使用自訂提示建立報表的指示，請參閱 [建立自訂提示](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/reporting/intermediate-reporting/custom-prompts.html).

</br>
</br>

**最佳實務**

使用版面範本中的清單控制項來隱藏常用物件 (專案、任務、方案等) 的非必要篩選器、視圖和分組。

**原因說明**

數量越少，獲得越多。隱藏與您使用者的每日工作流程無關的篩選、檢視和分組清單選項會縮小清單範圍，讓使用者更容易更快找到所需專案。

如需如何使用版面配置範本隱藏篩選器、檢視或群組的說明，請參閱 [使用版面配置範本自訂報表清單](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/administration-and-setup/layout-templates/customize-reporting-lists-with-layout-templates.html).

</br>
</br>

**最佳實務**

透過版面配置範本的清單控制項，共用與貴組織工作流程和流程相關的自訂篩選器、檢視和群組。

**原因說明**

如果您已建立篩選器、檢視和群組，顯示使用者日常流程的特定資訊，可輕鬆透過版面配置範本共用這些資訊。 這樣一來，便能確保獲得指派該版面範本的每個人擁有與其工作流程相關的篩選器、視圖和分組選項。

透過版面範本來自訂您要讓使用者看見的資訊，也節省系統和群組管理員的時間，因為他們不必分別共用每一個篩選器、視圖或分組。

如需如何與版面配置範本共用篩選器、檢視或群組的說明，請參閱 [使用版面配置範本自訂報表清單](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/administration-and-setup/layout-templates/customize-reporting-lists-with-layout-templates.html).

</br>
</br>

**最佳實務**

在建立專案狀態、任務狀態或問題狀態的篩選器時，請使用「(物件) >> 狀態等同於」欄位的來源/欄位名稱搭配「等於」修飾元，而不是使用「專案 >> 狀態」欄位的來源/欄位名稱。

**原因說明**

藉由使用（物件）>「相等於」，您可以將具有特定狀態的所有自訂狀態指派給狀態設定中的「相等於」欄位。 而把篩選器設定為「(物件)>> 狀態 > 等於」，會要求您為篩選器選取特定的狀態。若您必須考慮各個篩選器中的新狀態，則可能造成維護的難題。每個篩選器必須開啟並更新為新狀態。

例如，如果您想查看所有目前的專案，您可以將篩選器設定為讀取「專案 >> 狀態 > 等於 > 目前」。但如果有人新增名為「作用中」的自訂狀態並將其等同於「目前」，該篩選器將無法找到具有「作用中」狀態的專案。 但是，若您使用「專案 >> 狀態等同於 > 等於 > 目前」，則篩選器會尋找狀態為「目前」或「進行中」的物件，因為兩者在「等同於」欄位均是「目前」。
