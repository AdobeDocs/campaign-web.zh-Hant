---
audience: end-user
title: 工作流程事件變數
description: 瞭解如何在工作流程中善用事件變數。
source-git-commit: 313b5688eee169612007b9704036ce1d8b89dd86
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---

# 工作流程事件變數 {#event-variables}

有些工作流程活動可讓您在運算式編輯器中編輯指令碼，以執行特定動作，例如擷取來自先前活動的資料、建置條件或根據事件變數計算檔案名稱。

## 什麼是事件變數 {#scripting}

在工作流程內容中執行的指令碼會存取一系列其他全域 **物件** 例如正在執行的工作流程本身(`ìnstance`)，其各種工作(`task`)或啟動指定任務的事件(`event`)。

至每種型別 **物件** 與的類別相關聯 **變數** 可在運算式編輯器中用於編輯下列活動中的指令碼的活動： **[!UICONTROL javascript程式碼]** 或 **[!UICONTROL 測試]**.

* **執行個體變數** (`instance.vars.xxx`)與全域變數的可比性。 所有活動都會共用這些區段。
* **任務變數** (`task.vars.xxx`)與本機變數具有可比性。 它們僅供目前任務使用。 持續性活動會使用這些變數來保留資料，這些變數有時也用於在相同活動的不同指令碼之間交換資料。
* **事件變數** (`vars.xxx`)可在工作流程處理序的基本任務之間交換資料。 這些變數是由啟動進行中任務的任務所傳遞。 然後會傳遞至下列活動。 **事件變數** 是最常使用的變數，且使用方式應優於例項變數。

>[!NOTE]
>
>有關指令碼和Adobe Campaign中公開之物件和變數的其他資訊，請參閱的Campaign v8 （使用者端主控台）檔案 [本節](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/advanced-management/javascript-scripts-and-templates).
>
>請注意，雖然此資源提供有價值的深入分析，但差異可能存在，因為其僅適用於使用者端主控台，而非Campaign Web使用者介面。

## 在運算式編輯器中善用事件變數 {#expression-editor}

預先定義的事件變數可用於運算式編輯器左側窗格。 您也可以在程式碼中初始化新變數，以建立新的變數。

![](assets/event-variables.png)

除了這些事件變數以外，您也可以運用 **[!UICONTROL 條件]** 功能表，以建立條件和 **[!UICONTROL 新增目前日期]** 功能表，以使用與日期格式相關的功能。
