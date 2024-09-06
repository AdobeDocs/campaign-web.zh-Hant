---
audience: end-user
title: 使用JavaScript程式碼工作流程活動
description: 瞭解如何使用JavaScript程式碼工作流程活動
exl-id: ca040ef8-5e0d-44e0-818d-08cfe99100be
source-git-commit: 040a7f68f072d5c3a7ce56a61d3383f0baccf8a8
workflow-type: tm+mt
source-wordcount: '948'
ht-degree: 26%

---

# JavaScript 程式碼 {#javascript-code}

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript"
>title="JavaScript 程式碼"
>abstract="「**JavaScript 程式碼**」活動可讓您在工作流程過程中執行 JavaScript 程式碼。這允許您執行動作或從資料庫收集資訊。使用「**簡單**」JavaScript 程式碼活動在工作流程執行時執行一個程式碼片段。「**進階**」Javascript 程式碼活動可讓您透過依序執行兩個不同的程式碼片段來執行更複雜的操作。第一次開始工作流程時，將執行第一次呼叫。工作流程每次重新執行時，會執行第二次呼叫中定義的程式碼。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_snippet"
>title="JavaScript 片段"
>abstract="定義執行活動時要執行的指令碼。如果您要設定「**進階**」JavaScript 活動，則需要編輯兩個程式碼片段：在第一次執行工作流程時執行的第一個呼叫程式碼，以及在工作流程的下一次呼叫時執行的下一個呼叫程式碼。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_execution"
>title="JavaScript 執行"
>abstract="設定執行延遲以在執行一段時間後停止活動。依預設，執行階段不能超過 1 小時。在這類延遲之後，此流程將中止並顯示錯誤訊息，並且活動執行會失敗。若要忽略此限制，請將值設為 0。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_transition"
>title="JavaScript 轉變"
>abstract="開啟&#x200B;**[!UICONTROL 處理錯誤]**&#x200B;選項，以便在其他輸出轉換中保留執行指令碼期間發生的錯誤。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_processerrors"
>title="處理錯誤"
>abstract="處理錯誤"

**JavaScript程式碼**&#x200B;活動是&#x200B;**資料管理**&#x200B;活動。 使用此活動可在工作流程內容中執行JavaScript指令碼。 這可讓您從資料庫收集資訊，或執行其他複雜的作業。

## 設定JavaScript程式碼活動 {#javascript-code-configuration}

請依照下列步驟設定&#x200B;**JavaScript程式碼**&#x200B;活動：

1. 將&#x200B;**JavaScript程式碼**&#x200B;活動新增至您的工作流程。

1. 選擇要建立的活動型別：

   * **簡單**：執行一個程式碼片段。
   * **進階**：此選項可讓您執行兩個不同的程式碼片段，以執行更進階的作業。 [瞭解如何設定進階JavaScript活動](#advanced)

   >[!NOTE]
   >
   >透過Campaign Web使用者介面，我們已合併&#x200B;**簡單**&#x200B;和&#x200B;**進階** JavaScript程式碼功能，將兩個活動合併為一個。 此合併不會以任何方式影響活動的功能。

1. 確認，然後按一下&#x200B;**[!UICONTROL 編輯代碼]**&#x200B;按鈕以開啟運算式編輯器。 左側窗格會提供預先定義的語法，讓您用來建置程式碼，包括事件變數。 [瞭解如何使用事件變數和運算式編輯器](../event-variables.md)

   ![](../assets/javascript-editor.png)

1. 在&#x200B;**[!UICONTROL 執行]**&#x200B;區段中，設定延遲以在執行期間後停止活動。 依預設，執行階段不能超過 1 小時。在這類延遲之後，此流程將中止並顯示錯誤訊息，並且活動執行會失敗。若要忽略此限制，請將值設為 0。

   ![](../assets/javascript-config.png)

1. 開啟&#x200B;**[!UICONTROL 處理錯誤]**&#x200B;選項，以便在其他輸出轉換中保留執行指令碼期間發生的錯誤。

## 進階JavaScript程式碼活動 {#advanced}

進階JavaScript活動可讓您執行複雜的作業。 它可讓您：

* 執行兩個不同的程式碼片段。 第一個程式碼片段會在第一次啟動工作流程時執行。 每次工作流程再次執行時，都會執行第二個呼叫中定義的程式碼片段。
* 新增多個輸出轉變，您可使用指令碼動態互動。

若要設定進階JavaScript程式碼活動，請遵循下列步驟：

1. 選取&#x200B;**進階**&#x200B;型別，然後設定要執行的程式碼片段：

   * 按一下&#x200B;**[!UICONTROL 編輯第一次呼叫代碼]**&#x200B;以定義要在第一次呼叫期間執行的指令碼。
   * 按一下&#x200B;**[!UICONTROL 編輯下一個呼叫代碼]**&#x200B;以定義要在工作流程下一次呼叫期間執行的指令碼。 （選擇性）

1. 若要新增一或多個輸出轉變，請按一下&#x200B;**[!UICONTROL 新增轉變]**&#x200B;按鈕，並為每個轉變指定標籤和內部名稱。

   在此範例中，我們已設定由程式碼片段中的指令碼根據特定條件啟動的兩個轉變。

   ![](../assets/javascript-transitions.png)

1. 完成活動的設定並啟動工作流程。

## 範例 {#javascript-code-example}

### 根據傳入母體初始化變數 {#example1}

此範例說明如何根據工作流程所定位的設定檔數初始化變數。

![](../assets/javascript-example1.png)

在此，我們正在從資料庫中鎖定VIP設定檔。 我們要建立名為「channel」的變數，其值取決於「建立對象」活動鎖定的設定檔數量：

* 如果目標設定檔超過1000個，請使用「電子郵件」值初始化變數。
* 否則，請使用值「sms」將其初始化。

要執行此操作，請依照下列步驟執行：

1. 在&#x200B;**建置對象**&#x200B;活動之後，新增型別為&#x200B;**Simple**&#x200B;的&#x200B;**JavaScript程式碼**&#x200B;活動。

1. 按一下&#x200B;**編輯程式碼**&#x200B;並設定程式碼片段，如下所示：

   ```
   if (vars.recCount > 1000)
       vars.channel ="email"
   else
       vars.channel = "sms"
   ```

1. 啟動工作流程。 「頻道」變數是以「電子郵件」或「簡訊」值建立，視&#x200B;**建置對象**&#x200B;活動鎖定的設定檔數量而定。

### 根據變數的值觸發轉變 {#example2}

此範例說明如何根據變數的值觸發轉變。

![](../assets/javascript-example2-transitions.png)

在此處，工作流程從&#x200B;**外部訊號**&#x200B;活動開始，從另一個工作流程傳入變數(`interest`)。 變數的值為「執行中」或「瑜伽」，視初始工作流程中執行的篩選作業而定。

我們想要根據變數的值，在工作流程中觸發不同的轉變。

要執行此操作，請依照下列步驟執行：

1. 在型別為&#x200B;**進階**&#x200B;的外部訊號活動後新增&#x200B;**JavaScript程式碼**&#x200B;活動。

1. 新增兩個轉變：每個可能的變數值（「執行中」、「瑜伽」）各一個。

1. 按一下&#x200B;**編輯第一個呼叫代碼**&#x200B;並設定程式碼片段，如下所示：

   ```
   if (vars.interest=="running")
       task.postEvent(task.transitionByName("running"));
   else
       task.postEvent(task.transitionByName("yoga"));
   ```

1. 完成每個轉變的設定以符合您的需求，然後開始工作流程。 已根據透過&#x200B;**外部訊號**&#x200B;活動傳遞的`interest`變數值，啟動兩個輸出轉換之一。
