---
audience: end-user
title: 設定工作流程設定
description: 瞭解如何使用Adobe Campaign Web進行工作流程設定
exl-id: 3aef912b-086b-4aa4-9556-c09396112313
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '1048'
ht-degree: 16%

---

# 設定工作流程設定 {#workflow-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="工作流程屬性"
>abstract="在此畫面中，選擇用於建立工作流程的範本並指定標籤。展開&#x200B;**其他選項**&#x200B;區段以設定更多設定，例如工作流程內部名稱、其資料夾、時區和主管群組。 強烈建議選取一個主管群組，以便在發生錯誤時警告操作者。"

在畫布中建立工作流程或協調工作流程活動時，請存取與工作流程相關的進階設定。 例如，為工作流程設定特定時區、管理工作流程在發生錯誤時的行為方式，或管理清除工作流程歷史記錄的延遲。

這些設定在建立工作流程時，會在選取的範本中預先設定，但可視需要為此特定工作流程進行編輯。

![工作流程設定按鈕介面](assets/workflow-settings-button.png){zoomable="yes"}{width="70%" align="left"}

## 工作流程屬性 {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="工作流程屬性"
>abstract="本區段提供一般工作流程屬性，在建立工作流程時也可以存取這些屬性。您可以選擇用於建立工作流程的範本並指定標籤。展開其他選項區段以設定特定設定，例如工作流程儲存資料夾或時區。"

**[!UICONTROL 屬性]**&#x200B;區段提供一般設定，可在建立工作流程時進行設定。 若要存取現有工作流程的內容，請按一下工作流程畫布上方動作列中的&#x200B;**[!UICONTROL 設定]**&#x200B;按鈕。

![工作流程設定介面](assets/workflow-settings.png){zoomable="yes"}{width="70%" align="left"}

這些屬性包括：

* 顯示在清單中的工作流程的&#x200B;**[!UICONTROL 標籤]**。
* 工作流程的&#x200B;**[!UICONTROL 內部名稱]**。
* 工作流程應儲存的&#x200B;**[!UICONTROL 資料夾]**。
* 用於工作流程所有活動的預設&#x200B;**[!UICONTROL 時區]**。 依預設，工作流程的時區是為目前的Campaign運運算元定義的時區。
可能的值包括：
   * **伺服器時區**，以使用Adobe Campaign應用程式伺服器的時區。
   * **操作員時區**，使用執行工作流程之Adobe Campaign操作員的時區，如使用者端主控台中操作員的設定檔所定義。
   * **資料庫**&#x200B;的時區，以使用資料庫伺服器的時區。
   * 特定時區。
* 當工作流程失敗時，屬於&#x200B;**[!UICONTROL 監督員]**&#x200B;欄位中所選操作員群組的操作員會收到電子郵件通知。
* 輸入工作流程的&#x200B;**[!UICONTROL 描述]**。

當工作流程是與行銷活動](create-workflow.md)相關聯的[時，會顯示在&#x200B;**[!UICONTROL 連結的行銷活動]**&#x200B;欄位中。 從該欄位開啟關聯的行銷活動。

## 細分設定 {#segmentation-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="細分設定"
>abstract="在此區段中，您可以選取目標維度來定位工作流程中的設定檔，並選擇在兩個執行之間保留工作流程結果。 此選項應僅用於測試目的，絕不能在生產工作流程中啟用。"

* **[!UICONTROL 目標維度]**：選取目標維度，以用於目標定位設定檔，例如收件者、合約受益者、操作員、訂閱者等。 [進一步瞭解目標維度](../audience/targeting-dimensions.md)。

* **[!UICONTROL 保留兩個執行之間的臨時母體結果]**：依預設，僅保留工作流程最後執行的工作表。 技術工作流程會清除先前執行的工作表（每天執行）。

  如果啟用此選項，即使執行工作流程後，也會保留工作表格。 將其用於測試目的，並確保僅在開發或中繼環境中&#x200B;**使用**。 絕不可在生產工作流程中勾選該專案。

## 執行設定 {#exec-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="執行設定"
>abstract="您可以在此段落中設定與執行工作流程相關的設定，例如保留工作流程記錄的天數。"

* **[!UICONTROL 歷程記錄（以天為單位）]**：指定必須清除歷程記錄的天數。 歷史記錄包含與工作流程相關的元素，例如記錄、任務和事件（連結至工作流程操作的技術物件）。 現成的工作流程範本預設值為30天。 清除歷史記錄是由資料庫清理技術工作流程執行，每日執行。

  >[!IMPORTANT]
  >
  >如果&#x200B;**[!UICONTROL History in days]**&#x200B;欄位留空，其值將視為「1」，表示歷史記錄將在1天後清除。

* **[!UICONTROL 預設相似性]**：如果您的安裝包含數個工作流程伺服器，請使用此欄位指定工作流程執行所在的伺服器。 這會在特定伺服器上強制執行該工作流程。 選擇任何現有的相似性名稱，但請確保不要使用空格或標點符號。 如果您使用不同的伺服器，請指定以逗號分隔的不同名稱。

  >[!IMPORTANT]
  >
  >如果此欄位中定義的值不存在於任何伺服器上，工作流程將維持擱置狀態。

* **[!UICONTROL 將SQL查詢儲存在記錄檔中]**：核取此選項以將工作流程中的SQL查詢儲存在記錄檔中。 此功能保留給進階使用者使用。它適用於包含目標定位活動的工作流程，例如&#x200B;**[!UICONTROL 建立對象]**。 啟用此選項後，工作流程執行期間傳送到資料庫的SQL查詢會顯示在工作流程的日誌中，可讓您分析這些查詢以最佳化查詢或診斷問題。

## 錯誤管理設定 {#error-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="錯誤管理設定"
>abstract="在此區段中，您可以定義工作流程在執行期間應如何管理錯誤。您可以選擇暫停流程、忽略一定數量的錯誤，或是停止工作流程執行。"

* **[!UICONTROL 錯誤管理]**：此欄位可讓您定義工作流程任務發生錯誤時要採取的動作。 有三個可能的選項：

   * **[!UICONTROL 暫停處理序]**：工作流程已自動暫停，其狀態變更為&#x200B;**[!UICONTROL 失敗]**。 問題解決後，請使用&#x200B;**[!UICONTROL 繼續]**&#x200B;按鈕繼續工作流程。
   * **[!UICONTROL 忽略]**：觸發錯誤的工作狀態變更為&#x200B;**[!UICONTROL 失敗]**，但工作流程會保留&#x200B;**[!UICONTROL 已啟動]**&#x200B;狀態。<!-- TO ADD ONCE SCHEDULER IS AVAILABLE This configuration is relevant for recurring tasks: if the branch includes a scheduler, it will start normally next time the workflow is executed.-->
   * **[!UICONTROL 中止處理序]**：工作流程已自動停止，其狀態變更為&#x200B;**[!UICONTROL 失敗]**。 問題解決後，請使用&#x200B;**[!UICONTROL 開始]**&#x200B;按鈕重新啟動工作流程。

* **[!UICONTROL 連續錯誤]**：在&#x200B;**[!UICONTROL 發生錯誤]**&#x200B;欄位中選取&#x200B;**[!UICONTROL 忽略]**&#x200B;值時，此欄位將可供使用。 指定程式停止前可忽略的錯誤數目。 一旦達到此數目，工作流程狀態就會變更為&#x200B;**[!UICONTROL 失敗]**。 如果此欄位的值為 0，則無論錯誤數為何，工作流程都不會停止。

## 初始化指令碼 {#initialization-script}

**初始化指令碼**&#x200B;可讓您初始化變數或修改活動屬性。 按一下&#x200B;**編輯程式碼**&#x200B;按鈕，然後輸入要執行的程式碼片段。 執行工作流程時會呼叫指令碼。 請參閱與[事件變數](../workflows/event-variables.md)相關的章節。