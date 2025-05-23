---
audience: end-user
title: 工作流程事件變數
description: 瞭解如何在工作流程中善用事件變數。
exl-id: 526dc98f-391d-4f3f-a687-c980bf60b93b
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 1%

---

# 工作流程事件變數 {#event-variables}

有些工作流程活動可讓您在運算式編輯器中編輯指令碼以執行特定動作，例如從先前的活動中擷取資料、建置條件或根據事件變數計算檔案名稱。

## 什麼是事件變數 {#scripting}

在工作流程內容中執行的指令碼會存取一系列其他全域&#x200B;**物件**，例如正在執行的工作流程本身(`instance`)、其各種工作(`task`)，或啟動指定工作(`event`)的事件。

**物件**&#x200B;的每個型別都與&#x200B;**變數**&#x200B;的類別相關聯，在編輯活動中的指令碼時，這些變數可用於運算式編輯器，例如&#x200B;**[!UICONTROL JavaScript程式碼]**&#x200B;或&#x200B;**[!UICONTROL 測試]**。

* **執行個體變數** (`instance.vars.xxx`)可與全域變數比較。 所有活動都會共用這些區段。
* **工作變數** (`task.vars.xxx`)可與區域變數比較。 它們僅供目前任務使用。 持續性活動會使用這些變數來保留資料，這些變數有時也用於相同活動的不同指令碼之間交換資料。
* **事件變數** (`vars.xxx`)可在工作流程處理序的基本工作之間交換資料。 這些變數是由啟動進行中任務的任務所傳遞。 然後會傳遞至下列活動。 **事件變數**&#x200B;是最常使用的變數，應該優先使用它們而不是執行個體變數。

>[!NOTE]
>
>在[本區段](https://experienceleague.adobe.com/zh-hant/docs/campaign/automation/workflows/advanced-management/javascript-scripts-and-templates)的Campaign v8 （使用者端主控台）檔案中，有提供指令碼以及Adobe Campaign中公開之物件和變數的其他資訊。
>
>請注意，雖然此資源提供有價值的深入分析，但差異可能存在，因為其僅適用於使用者端主控台，而非Campaign Web使用者介面。

## 在運算式編輯器中善用事件變數 {#expression-editor}

預先定義的事件變數可用於運算式編輯器的左側窗格。 您也可以在程式碼中初始化新變數，以建立新的變數。

![在運算式編輯器的左側窗格中顯示預先定義之事件變數的熒幕擷圖](assets/event-variables.png)

除了這些事件變數之外，您也可以使用左窗格中的&#x200B;**[!UICONTROL 條件]**&#x200B;功能表來建置條件，並使用&#x200B;**[!UICONTROL 新增目前日期]**&#x200B;功能表來套用與日期格式相關的功能。