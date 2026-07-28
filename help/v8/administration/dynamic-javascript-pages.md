---
title: 使用動態JavaScript頁面
description: 瞭解如何使用動態JavaScript頁面。
exl-id: b7de9f55-2aef-4ba9-a2a1-e9ca15deacfb
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 2df9759bb21eae0630bcbe9130a1a20b165e8cca
workflow-type: tm+mt
source-wordcount: 392
ht-degree: 26%

---

# 使用動態JavaScript頁面 {#dynamic-javascript-pages}

>[!CONTEXTUALHELP]
>id="acw_dynamic_javascript_pages_list"
>title="動態 JavaScript 頁面"
>abstract="您可以運用動態 JavaScript 頁面 (JSSP) 建置伺服器端頁面，這些頁面在透過 URL 存取時會產生動態內容，例如自訂 API、匯出或網頁應用程式邏輯。 您可以從這個清單中建立、修改、複製或刪除動態 JavaScript 頁面。"

>[!CONTEXTUALHELP]
>id="acw_dynamic_javascript_pages_create"
>title="建立動態 JavaScript 頁面"
>abstract="定義動態 JavaScript 頁面的命名空間、名稱和標籤，然後使用 JavaScript 程式碼編寫其內容。 命名空間和名稱在建立完成後即無法修改。"

## 關於動態JavaScript頁面 {#about}

您可以運用動態 JavaScript 頁面 (JSSP) 建置伺服器端頁面，這些頁面在透過 URL 存取時會產生動態內容，例如自訂 API、匯出或網頁應用程式邏輯。 這些頁面儲存在左側導覽窗格中的&#x200B;**[!UICONTROL 管理]** > **[!UICONTROL 動態JavaScript頁面]**&#x200B;功能表中。

![顯示可用選項的Dynamic JavaScript頁面清單介面](assets/dynamic-javascript-pages.png)

從動態JavaScript頁面清單中，您可以：

* **複製或刪除頁面**：按一下省略符號按鈕，然後選取所要的動作。
* **修改頁面**：按一下頁面的名稱以開啟其屬性、進行變更並儲存。
* **建立新的動態JavaScript頁面**：按一下&#x200B;**[!UICONTROL 建立動態JavaScript頁面]**&#x200B;按鈕。

<!--
>[!NOTE]
>
>In the Campaign console, dynamic JavaScript pages are available under **[!UICONTROL Administration]** > **[!UICONTROL Configuration]** > **[!UICONTROL Dynamic JavaScript pages]**. Although the menu location differs from the Web user interface, the list is identical and operates like a mirror.
-->

## 建立動態JavaScript頁面 {#create}

若要建立動態JavaScript頁面，請遵循下列步驟：

1. 導覽至&#x200B;**[!UICONTROL 動態JavaScript頁面]**&#x200B;功能表，然後按一下&#x200B;**[!UICONTROL 建立動態JavaScript頁面]**&#x200B;按鈕。

1. 定義頁面屬性：

   * **[!UICONTROL 名稱空間]**：指定與自訂資源相關的名稱空間。 預設的名稱空間為「cus」，但可能會依您的實施而有所不同。
   * **[!UICONTROL 名稱]**：用來參考頁面的唯一識別碼。
   * **[!UICONTROL 標籤]**：動態JavaScript頁面清單中顯示的描述性標籤。

   ![顯示名稱空間、名稱和標籤欄位的動態JavaScript頁面建立介面](assets/dynamic-javascript-pages2.png)

   >[!NOTE]
   >
   >建立後，**[!UICONTROL 名稱空間]**&#x200B;和&#x200B;**[!UICONTROL 名稱]**&#x200B;欄位就無法修改。 若要進行變更，請複製頁面並視需要更新。

1. 按一下&#x200B;**[!UICONTROL 建立程式碼]**&#x200B;按鈕以定義頁面的內容，然後使用`<%@ page %>`指令和`NL.require()`呼叫來撰寫JSSP程式碼以載入核心程式庫。

   ![動態JavaScript頁面程式碼編輯器](assets/dynamic-javascript-pages4.png)

1. 按一下&#x200B;**[!UICONTROL 確認]**&#x200B;以儲存您的程式碼。

1. 當您的動態JavaScript頁面準備就緒時，請按一下[建立]。**** 頁面現在可從名稱空間和名稱建立的URL存取，格式為`https://<your-instance>/<namespace>/<name>`。 例如，`cus`名稱空間中名為`recipientAPI.jssp`的頁面可在`https://<your-instance>/cus/recipientAPI.jssp`存取。

如需可重複使用JavaScript函式的詳細資訊，請參閱[使用JavaScript程式碼](javascript-codes.md)。
