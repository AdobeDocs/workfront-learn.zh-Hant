---
title: 初始情境設計
description: 瞭解當您首次登入Workfront Fusion以及建立您的第一個案例時的一些基本導覽提示。
activity: use
team: Technical Marketing
type: Tutorial
feature: Workfront Fusion
role: User
level: Beginner
jira: KT-11038
thumbnail: KT11038.png
exl-id: 8ecf4979-f291-4788-bdaa-ab5485fb0849
source-git-commit: a25a49e59ca483246271214886ea4dc9c10e8d66
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 0%

---

# 初始情境設計

瞭解當您首次登入Workfront Fusion以及建立您的第一個案例時的一些基本導覽提示。

## 練習概述

在Workfront中為專案清單CSV檔案中的每一列建立一個新專案。

![初始情境設計圖1](../12-exercises/assets/initial-scenario-design-1.png)

## 要遵循的步驟

1. 在「案例」區段中建立名為「Fusion啟用練習」的資料夾。
1. 按一下資料夾，然後按一下「建立新情境」。

   ![初始情境設計影像2](../12-exercises/assets/initial-scenario-design-2.png)

1. 在下一個頁面，搜尋Workfront並選取該應用程式。 然後按一下「繼續」。
1. 在情境設計工具畫面的左上方，將情境重新命名為「初始情境設計」
1. 按一下畫面中央的空白觸發程式模組，然後選取Workfront應用程式，再選取「下載檔案」模組。

   **驗證模組與您的Workfront帳戶的連線。**

1. 若要第一次建立連線，請按一下「新增」按鈕。

   ![初始情境設計影像3](../12-exercises/assets/initial-scenario-design-3.png)

1. 為連線命名，例如「我的Workfront 2020」

   ![初始情境設計影像4](../12-exercises/assets/initial-scenario-design-4.png)

1. 輸入Workfront執行個體的URL，然後按一下「下一步」。

   ![初始情境設計圖5](../12-exercises/assets/initial-scenario-design-5.png)

1. 輸入您的密碼，然後按一下「登入」。

   **連線已建立。 現在輸入您要從Workfront下載之檔案的檔案ID。**

   ![初始情境設計圖7](../12-exercises/assets/initial-scenario-design-7.png)

1. 返回Workfront。 在「Fusion Experience Files」資料夾中，選取「_Fusion2020_Project List.csv」，然後按一下左側面板中的「檔案詳細資訊」。 從URL位址複製檔案ID號碼（這是URL中的第一個長數字）。

   ![初始情境設計圖8](../12-exercises/assets/initial-scenario-design-8.png)

1. 返回Fusion，並在「檔案ID」欄位中貼上數字，然後按一下「確定」。
1. 最佳實務是在建立模組時重新命名模組。 以滑鼠右鍵按一下Workfront模組，然後選擇「重新命名」。 將模組命名為「取得專案清單」。

   **接下來，您將剖析您剛才下載的CSV檔案，以便存取檔案中的每一列。 當您從每一列建立專案時，將會使用此資訊。**

1. 按一下Workfront模組的右側以新增另一個模組。 搜尋CSV應用程式並選取「剖析CSV」模組。
1. 設定剖析CSV為6欄、CSV包含標題、逗號分隔符號型別，並將資料放入CSV欄位中。 然後按一下「確定」。

   ![初始情境設計影像9](../12-exercises/assets/initial-scenario-design-9.png)

1. 將此模組重新命名為「剖析專案清單」。
1. 在情境設計工具底部，按一下儲存以儲存情境。
1. 按一下「執行一次」以檢視輸出。

   >[!NOTE]
   >
   >忽略轉換器不應是最後一個模組的警告（這為true，但在此測試中並不重要）。 按一下[Run Anyway]。

   ![初始情境設計影像10](../12-exercises/assets/initial-scenario-design-10.png)

1. 開啟「剖析CSV 」模組上的執行檢測器，檢視模組的輸入和輸出。 有一個套件（CSV檔案）作為輸入，多個套件作為輸出（CSV檔案中的每一列有一個套件）。 它應該看起來像這樣：

   ![初始情境設計影像11](../12-exercises/assets/initial-scenario-design-11.png)

   **新增模組以為CSV檔案中的每一列建立專案。**

1. 新增另一個模組。 選取Workfront應用程式，然後選擇建立記錄模組。
1. 將記錄型別設定為專案。

   >[!TIP]
   >
   >開始輸入幾個字母來搜尋它，例如 *專案*，即可直接使用。

1. 然後使用Cmd/Ctrl+G來尋找名稱（專案名稱）。 勾選「名稱」旁的方塊；欄位會顯示在下方。
1. 現在勾選「計劃開始日期」和「優先順序」旁的方塊。
1. 按一下「名稱」欄位以顯示對應面板。 按一下「剖析CSV 」模組中的「欄1 」欄位，將其新增到「名稱」欄位。 這是CSV檔案中的專案名稱。
1. 對於規劃開始日期，按一下「剖析CSV 」模組中的「欄5」。
1. 針對「優先順序」，請從下拉式選單中選擇「一般」。

   **您的對應面板應如下所示：**

   ![初始情境設計影像12](../12-exercises/assets/initial-scenario-design-12.png)

1. 按一下「確定」。

   >[!NOTE]
   >
   >如果您沒有按一下「確定」，然後不小心按回設計工具，您的工作不會儲存，您將必須再次對應。

1. 以滑鼠右鍵按一下Workfront模組，並將其重新命名為「建立Workfront專案」。
1. 儲存情境並按一下「執行一次」按鈕。
1. 按一下最後一個模組右上角的執行檢測器。

   + 您會看到已執行20個作業。 每個作業都會從CSV檔案中取出一個套件，表示一列作為輸入和輸出一個套件，這是在Workfront中建立的專案。 所建立專案的專案ID會隨輸出組合一起顯示。

   ![初始情境設計影像13](../12-exercises/assets/initial-scenario-design-13.png)

   **使用附註**

1. 附註可協助建立案例設計的可見度。 若要在「建立Workfront專案」模組中新增附註，請以滑鼠右鍵按一下並選取「新增附註」。 設計工具視窗右側的面板會彈出，讓您可以將註記新增至模組。 輸入「建立專案，其名稱、規劃開始日期和優先順序均對應自CSV檔案」。
1. 新增其他附註以說明觸發程式模組(第一個Workfront模組)正在執行的工作。
1. 按一下右上角的X關閉附註面板。

   + 按一下底部工具列中的「附註」按鈕，或用滑鼠右鍵按一下任何模組並新增附註，可再次存取附註。
   + 附註會以反向時間順序排序。
   + 新增附註後，「附註」按鈕上就會出現橘色圓點。

   ![初始情境設計影像14](../12-exercises/assets/initial-scenario-design-14.png)

1. 按一下控制項工具列中的「儲存」按鈕以儲存情境。
1. 您可以檢視在Workfront執行個體中建立的專案。
