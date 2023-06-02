---
audience: end-user
title: 使用 Adobe Campaign Web 建立工作流程
description: 了解如何使用 Adobe Campaign Web 建置工作流程
badge: label="Alpha" type="Positive"
exl-id: 7ac8eedf-c141-4a61-b4d3-d81f99247c6d
source-git-commit: 1a608d2042ae257d89acbd67d99a0ce05d89f382
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 24%

---

# 設定工作流程設定 {#workflow-settings}

在畫布中協調工作流程活動時，您可以存取與工作流程相關的進階設定。 例如，您可以為工作流程設定特定時區、管理工作流程在發生錯誤時的行為方式，或管理應清除工作流程歷史記錄的延遲。

這些設定是在建立工作流程時於所選範本中預先設定的，但可視需要為此特定工作流程進行編輯。

若要這麼做，請按一下 **[!UICONTROL 工作流程設定]** 圖示填入工作流程標籤旁。

![](assets/workflow-settings.png)

## 工作流程屬性 {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="工作流程屬性"
>abstract="待定"

此 **[!UICONTROL 屬性]** 區段提供一般設定，可在建立工作流程時存取。

* **[!UICONTROL 標籤]**：顯示在清單中的工作流程標籤。
* **[!UICONTROL 名稱]**：工作流程的內部名稱。
* **[!UICONTROL 資料夾]**：工作流程應儲存的資料夾。
* **[!UICONTROL 連結的行銷活動]**：如果工作流程已在行銷活動中建立，則會顯示此欄位。 它可讓您開啟關聯的行銷活動。
* **[!UICONTROL 時區]**：定義預設用於工作流程所有活動的特定時區。 依預設，工作流程的時區是為目前的 Campaign 操作者定義的時區。
* **[!UICONTROL 監督員]**：當工作流程發生錯誤時，只要屬於工作流程監督群組的操作員的電子郵件地址列在其設定檔中，就會透過電子郵件通知該操作員。
* **[!UICONTROL 說明]**：使用此欄位提供工作流程的說明。

## 細分設定

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="細分設定"
>abstract="待定"

* **[!UICONTROL 目標維度]**：選取用來鎖定設定檔的目標維度：收件者、合約受益者、操作員、訂閱者等。
* **[!UICONTROL 保留兩次執行之間的中期母體結果]**：依預設，只會保留上次執行工作流程的工作表。 技術工作流程會清除先前執行的工作表，每天都會執行。

   如果啟用此選項，即使工作流程已執行，也會保留工作表格。 您可以將其用於測試目的，因此必須僅用於開發或中繼環境。 絕不可在生產工作流程中勾選該專案。

## 執行設定

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="執行設定"
>abstract="待定"

* **[!UICONTROL 歷史記錄（天）]**：指定必須清除歷程記錄的天數。 歷史記錄包含與工作流程相關的元素：記錄、任務、事件（連結至工作流程操作的技術物件）。 立即可用工作流程範本的預設值為 30 天。歷史記錄的清除工作是由資料庫清除技術工作流程執行，預設每天執行

   >[!IMPORTANT]
   >
   >如果「**[!UICONTROL 歷史記錄 (天)]**」欄位為空白，欄位值將被視為「1」，表示歷史記錄將在 1 天後清除。

* **[!UICONTROL 預設相似性]**：如果您的安裝包含數個工作流程伺服器，請使用此欄位來選擇要執行工作流程的電腦。 如果此欄位中定義的值不存在於任何伺服器上，工作流程將維持擱置狀態。

* **[!UICONTROL 將SQL查詢儲存在記錄檔中]**：可讓您從工作流程將SQL查詢儲存至記錄中。 此功能保留給進階使用者使用。它適用於包含目標定位活動的工作流程，例如 **[!UICONTROL 建立對象]**. 啟用此選項後，工作流程執行期間傳送到資料庫的SQL查詢會顯示在Adobe Campaign中，讓您能夠分析這些查詢以最佳化查詢或診斷問題。

   如果啟用選項，在新增至工作流程 (行銷活動工作流程除外) 和&#x200B;**[!UICONTROL 屬性]**&#x200B;活動的「**[!UICONTROL SQL 記錄]**」索引標籤中會顯示查詢。<!-- where?-->

## 錯誤管理設定

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="錯誤管理設定"
>abstract="待定"

* **[!UICONTROL 錯誤管理]**：此欄位可讓您定義工作流程任務發生錯誤時應採取的動作。 您有兩個選擇：

   * **[!UICONTROL 暫停處理序]**：工作流程會自動暫停，其狀態會變更為 **[!UICONTROL 已失敗]**. 問題解決後，請使用繼續工作流程 **[!UICONTROL 繼續]** 按鈕。
   * **[!UICONTROL 忽略]**：觸發錯誤的工作狀態會變更為 **[!UICONTROL 已失敗]**，但工作流程會保留 **[!UICONTROL 已開始]** 狀態。 <!-- TO ADD ONCE SCHEUDLER IS AVAILABLE This configuration is relevant for recurring tasks: if the branch includes a scheduler, it will start normally next time the workflow is executed.-->
   * **[!UICONTROL 中止程式]**：工作流程會自動停止，其狀態會變更為 **[!UICONTROL 已失敗]**. 問題解決後，請使用重新啟動工作流程 **[!UICONTROL 開始]** 按鈕。

* **[!UICONTROL 連續錯誤]**：此欄位在下列情況下可供使用： **[!UICONTROL 忽略]** 值已選取於 **[!UICONTROL 發生錯誤時]** 欄位。 您可以指定程序停止之前可以忽略的錯誤數。達到此數目後，工作流程狀態會變更為 **[!UICONTROL 已失敗]**. 如果此欄位的值為 0，則無論錯誤數為何，工作流程都不會停止。
