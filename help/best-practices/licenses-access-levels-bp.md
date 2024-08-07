---
title: 最佳實務 - 授權與存取層級
description: 探索 Adobe Workfront 專家提供的有關設定、管理和使用 Workfront 授權與存取層級的最佳實務建議。
feature: System Setup and Administration
role: Admin, Leader, User
level: Beginner
jira: KT-10914
exl-id: 6be3fab9-16a1-4ab9-89ce-8c53f8358e62
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '1253'
ht-degree: 100%

---

# 最佳實務 - 授權與存取層級

## 什麼是 Adobe Workfront「最佳實務」？

最佳實務是代表有效果、有效率之行動方針的準則；您和公司的使用者可以輕鬆採用；並且可以成功複製到整個組織。

當您檢閱這些建議時，請記住，有一些 Workfront 最佳實務是通用的，而其他做法可能針對特定主題。將這些最佳實務視為框架，作為設定和使用 Workfront 系統時的指引。

## 導覽此頁面

當您捲動瀏覽此頁面時，您會先找到該主題所有最佳實務的高層次清單。這樣您便可以檢視建議而無需深入瞭解詳細的「原因」。

「為什麼這些是最佳實務？」區域，位在高層次清單之後，詳細說明一部分的最佳實務，以及為什麼這些實務被認定為您的 Workfront 執行個體應該考慮執行的流程、工具等。

</br>
</br>

## 授權與存取層級最佳實務

* 在設定存取層級時，開始時應授予使用者較少的權限。

* 指派「檢閱」和「請求」授權時，一般會預設為「檢閱」，因為它授予使用者更多使用 Adobe Workfront 的權限。

* 在所有存取層級中，取消勾選每個物件的「全系統共用」核取方塊，除非您特別允許那些使用者執行。

* 考慮在某個存取層級的「設定其他限制」之下，啟動「絕不允許使用者刪除評論」設定。

* 限制系統管理員的數量，偏好使用群組管理員。

* 複製現有存取層級並進行修改，而不是從頭開始建立新的存取層級。

* 在「說明」方塊中記錄每個存取層級可以做的事。

* 限制自己的存取層級，僅限完成工作目標所需的存取，最好是能夠符合系統中大部分使用者需求的四到五個層級。

* 至少給兩位使用者指派全域系統管理者存取層級。

* 透過共用來限制使用者可以使用 Workfront 項目做什麼，而不是移除存取層級中的某個能力。

</br>
</br>


## 為什麼這些是最佳實務？

**最佳實務**

在設定存取層級時，開始時應授予使用者較少的權限。



**原因說明**

開始時僅授予使用者完成工作所需的最低權限。若他們因為存取權限不足而無法執行工作，他們通常會要求額外的存取權。立即授予使用者過多的存取權限，可能導致安全問題。另外，給予使用者更多存取權限，總是比取消他們的存取權限來得更好。

</br>
</br>



**最佳實務**

指派「檢閱」和「請求」授權時，一般會預設為「檢閱」，因為它授予使用者更多使用 Adobe Workfront 的權限。



**原因說明**

雖然「檢閱」和「請求」授權可以指派給 Workfront 中無限多位使用者，但「請求」授權僅有提出請求和更新請求的權限而已。「檢閱」授權對專案和任務擁有比「請求」授權更多的存取權，也可以檢視專案組合和方案、編輯文件以及存取資源管理工具。

</br>
</br>

**最佳實務**

在所有存取層級中，取消選取每個物件上的「全系統共用」核取方塊，除非使用者基於特定理由需要全系統共用。



**原因說明**

與全系統共用物件，通常是為了允許特定使用者查看 Workfront 中的項目。這是在缺乏 Workfront 群組結構或是大家並未完全理解共用權限時的做法。與全系統共用項目時，表示每個人都看得見所共用的項目。根據系統中保存的資訊類型而定，這可能導致隱私權問題。



例如，您可能在 Workfront 中與多個供應商合作來確認進度、提供核准等。如果「全系統共用」核取方塊是一個選項，可供選取或設為預設，則會讓所有供應商皆可取用資訊。



一併取消選取選項的話，則具有共用權限的使用者必須決定要與哪些特定的人員共用物件，無論是透過公司、群組或團隊。

</br>
</br>

**最佳實務**

考慮在某個存取層級的「設定其他限制」之下，啟動「絕不允許使用者刪除評論」設定。



**原因說明**

啟用這個選項會確保 Workfront 不移除過去的通訊。有些組織要求保留完整的註解歷史記錄以供稽核。

</br>
</br>

**最佳實務**

限制系統管理員的數量，偏好使用群組管理員。



**原因說明**

系統管理員可以存取 Workfront 中所有內容，包括全域系統設定。群組管理員可以存取的設定，由系統管理員控制並且僅適用於該特定群組。



系統管理員可以把許多責任委派給群組管理員，讓自己可以專心處理格局更大的事情，而不是忙於 Workfront 的日常維護工作。群組管理員能夠更輕鬆掌握其群組的需求，進而為使用者提供更好的服務。

</br>
</br>


**最佳實務**

複製現有存取層級並進行修改，而不是從頭開始建立新的存取層級。



**原因說明**

複製現有存取層級，能讓新的存取層級保有一致的基礎，確保具有相同的初始設定。這樣也可以節省時間，因為系統管理員不必從頭開始設定存取層級。

</br>
</br>

**最佳實務**

在「說明」方塊中記錄每個存取層級可以做的事。



**原因說明**

請提供詳細的說明，列出每個物件類型的設定。這樣可以協助現在和未來的系統管理員清楚知道每個存取層級有什麼能力，而不必深入研究存取層級來檢閱相關設定。



透過報告的形式檢閱存取層級時，也更容易進行比較。您可以在視圖中迅速新增說明欄位，馬上瞭解之間的差異，以及可能的話，瞭解為什麼要建立不同的存取層級。

</br>
</br>

**最佳實務**

限制自己的存取層級，僅限完成工作目標所需的存取，最好是能夠符合系統中大部分使用者需求的四到五個層級。


**原因說明**

存取層級可確保與使用者共用 Workfront 物件時，該使用者具有所需的編輯、刪除等權限。您可以設定概括性的存取層級，因為共用個別項目可進行較為具體的設定。


此外，存取層級較少，維護無叢集系統與實施策略的工作會變得更簡單，而在人員加入公司或更換部門時，也可以加速入職流程。

</br>
</br>

**最佳實務**

至少給兩位使用者指派全域系統管理者存取層級。

**原因說明**

應有不止一個人理解為什麼 Workfront 以這樣的方式設定、如何管理/維護這些設定，以及如何支援使用者。若有人不在辦公室、離開組織、忙碌等，仍可確保有其他人擁有能夠成功管理系統的資訊和知識。

</br>
</br>

**最佳實務**

透過共用來限制使用者可以使用 Workfront 項目做什麼，而不是移除存取層級中的某個能力。


**原因說明**

存取層級在全域的層級上控制使用者可以對特定項目做什麼事。每個專案、任務、專案組合、文件等的共用權限則控制個別使用者能夠對該特定項目做什麼事。與其針對具有特定存取層級的每個人移除一項能力，不如調整特定項目的共用權限，來限制使用者的控制權。
