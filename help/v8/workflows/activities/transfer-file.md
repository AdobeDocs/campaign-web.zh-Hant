---
audience: end-user
title: 使用傳輸檔案活動
description: 瞭解如何使用傳輸檔案工作流程活動
exl-id: a40c007e-c0c6-4e0f-aa0d-0260ecb74a03
source-git-commit: 1494db73b1a91825a2ca57ea1881eb04e95d8da2
workflow-type: tm+mt
source-wordcount: '1177'
ht-degree: 18%

---

# 傳輸檔案 {#transfer-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile"
>title="傳輸檔案"
>abstract="「**傳輸檔案**」活動可讓您接收或傳送檔案、測試檔案是否存在或列出伺服器上的檔案。使用的通訊協定可以是伺服器對伺服器通訊協定或 HTTP 通訊協定。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_options"
>title="傳輸檔案選項"
>abstract="傳輸檔案選項"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_activity"
>title="傳輸檔案活動"
>abstract="傳輸檔案活動"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_remoteserver"
>title="傳輸檔案遠端伺服器"
>abstract="指定要連線的伺服器。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_source"
>title="傳輸檔案來源"
>abstract="輸入所需的檔案名稱。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_delete_file"
>title="傳輸後刪除來源檔案"
>abstract="成功傳輸後清除來源檔案。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_display_logs"
>title="顯示工作階段記錄"
>abstract="與傳輸作業相關的資訊會顯示在工作流程記錄中。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_list_files"
>title="列出所有檔案"
>abstract="此選項會將伺服器上存在的所有檔案編成索引並儲存在 **vars.filenames** 事件變數中。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_historization"
>title="檔案歷史化"
>abstract="檔案歷史化"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_missing_file"
>title="處理遺失的檔案"
>abstract="您可以使用這個選項，在活動後啟動「**無檔案**」傳出轉變。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_errors"
>title="處理錯誤"
>abstract="您可以利用這個選項，在活動後啟動「**錯誤**」傳出轉變。"

此 **傳輸檔案** 活動是 **資料管理** 活動。 它可讓您接收或傳送檔案、測試檔案是否存在，或列出伺服器上的檔案。 使用的通訊協定可以是伺服器對伺服器通訊協定或 HTTP 通訊協定。

>[!NOTE]
>
>透過Campaign Web使用者介面，我們已將兩個活動合併為一個 **檔案傳輸** 和 **網頁下載** 功能。 此合併不會以任何方式影響活動的功能。

請依照下列詳細步驟設定 **傳輸檔案** 活動。

## 選擇傳輸通訊協定和作業 {#protocol}

1. 新增 **傳輸檔案** 活動進入工作流程，然後根據您要使用的通訊協定指定要執行的傳輸型別：

   * 若為HTTP通訊協定，請選取 **[!UICONTROL 網頁下載]**. 這可讓您以明確URL、外部帳戶或Adobe Campaign執行個體執行GET或POST下載檔案。
   * 對於其他伺服器對伺服器通訊協定和相關動作，請選取 **[!UICONTROL 檔案傳輸]**.

1. 選取要對活動執行的動作。 可用動作取決於您選取的轉移型別。 請展開下列各節以取得詳細資訊。

   +++動作可用於 **檔案傳輸** 型別活動

   * **[!UICONTROL 檔案下載]**：從伺服器下載檔案。
   * **[!UICONTROL 檔案上傳]**：在伺服器上上傳檔案。
   * **[!UICONTROL 測試以檢視檔案是否存在]**：檢查伺服器上是否有指定的檔案。 在活動後產生兩個出站轉變：「檔案存在」和「檔案不存在」。
   * **[!UICONTROL 檔案清單]**：列出伺服器上可用的所有檔案。

+++

   +++動作可用於 **網頁下載** 型別活動

   * **[!UICONTROL 簡單傳輸(GET)]**：擷取檔案。
   * **[!UICONTROL 使用表單轉移(POST)]**：上傳檔案和其他引數。

+++

   ![](../assets/workflow-transfer-file-action.png)

1. 依預設，針對檔案上傳動作，活動會使用上一個活動中指定的檔案。 若要使用其他檔案，請切換 **[!UICONTROL 使用上一個活動的檔案]** 選項關閉，然後按一下 **[!UICONTROL 新增檔案]** 按鈕。

   在 **[!UICONTROL 來源]** 欄位，輸入所需的檔案名稱，或使用運算式編輯器使用事件變數計算檔案名稱。 [瞭解如何使用事件變數和運算式編輯器](../event-variables.md). 重複此作業，視需要儘量新增檔案。

## 定義轉移目的地 {#destination}

1. 在 **[!UICONTROL 遠端伺服器]** 段落中，指定要使用下列其中一種方法連線的伺服器：

   * **[!UICONTROL 使用外部帳戶中定義的連線引數]**：使用外部帳戶的連線引數連線至伺服器。 在 **[!UICONTROL 伺服器資料夾]** 欄位，指定檔案的路徑（或檔案清單動作資料夾的路徑）。
   * **[!UICONTROL 快速設定]**：輸入檔案的URL （或檔案清單動作的資料夾）。
   * **[!UICONTROL Adobe Campaign執行個體]** （網頁下載型別活動）：從Adobe Campaign執行個體伺服器下載檔案。

   ![](../assets/workflow-transfer-file-server.png)

1. 針對Web下載POST動作，您可以透過作業傳遞其他引數。 若要這麼做，請按一下 **[!UICONTROL 新增引數]** 按鈕，然後指定引數的名稱和值。 您可以視需要新增任意數量的引數。

1. 依預設，對於檔案上傳，會自動儲存伺服器上上傳的檔案。 如果您不想保留此歷史記錄，請切換 **[!UICONTROL 保留已傳送檔案的歷史記錄]** 選項關閉。

## 歷史化設定 {#historization}

每次 **[!UICONTROL 傳輸檔案]** 活動執行時，會將上傳或下載的檔案儲存在專用的資料夾中。 系統會為工作流程的每個傳輸檔案活動建立一個資料夾。 依預設，檔案會儲存在Adobe Campaign安裝資料夾的預設儲存目錄中(`/vars`)。 若要使用特定資料夾，請切換 **[!UICONTROL 使用預設儲存目錄]** 選項關閉，然後輸入目錄的路徑。

![](../assets/workflow-transfer-file-historization.png)

為了保留伺服器上的實體空間，請務必限制此資料夾的大小。 要執行此操作，您可以定義活動資料夾的檔案數目上限或總大小。 依預設，授權 100 個檔案和 50 MB。

每次執行活動時，都會檢查資料夾，如下所示：

* 只考慮在活動執行前 24 小時以上建立的檔案。
* 如果考慮的檔案數大於 **[!UICONTROL 檔案數]** 欄位中，會刪除最舊的檔案，直到達到允許的最大檔案數為止。
* 如果考慮的檔案總大小大於 **[!UICONTROL 大小上限(MB)]** 引數)，刪除最舊的檔案，直到達到允許的大小上限(MB)為止。

>[!CAUTION]
>
>如果活動未再次執行，則不會檢查或清除其資料夾。考慮到這一點，在傳輸大型檔案時請務必小心。

## 進階與錯誤管理選項 {#advanced}

1. 在 **[!UICONTROL 進階選項]**，根據您設定的活動型別，會有其他選項可用。 請展開下列各節以取得詳細資訊。

   +++其他選項 **[!UICONTROL 檔案傳輸]** 型別活動

   * **[!UICONTROL 傳輸後刪除來源檔案]**：在成功傳輸後清除來源檔案。
   * **[!UICONTROL 顯示工作階段記錄]**：啟動此選項時，執行工作流程後，工作流程記錄中會顯示與傳輸作業相關的資訊。
   * **[!UICONTROL 列出所有檔案]** （檔案清單動作）：此選項會索引 `vars.filenames` 事件變數，其中檔案名稱以 `n` 個字元。 [瞭解如何使用事件變數](../event-variables.md)

+++

   +++其他選項 **[!UICONTROL 網頁下載]** 型別活動

   * **[!UICONTROL 追隨重新導向]**：檔案重新導向可讓您使用覆寫，將資料輸入或輸出導向不同型別的裝置。
   * **[!UICONTROL 將HTTP標頭新增至檔案]**：在某些情況下，您可能想要將其他HTTP標頭新增到檔案中。 最常見的情況是，這些標題將用於提供其他資訊以進行疑難排解，目的是 [跨原始資源共用(CORS)](https://developer.mozilla.org/docs/Web/HTTP/CORS)，或來設定特定的快取指示。
   * **[!UICONTROL 忽略HTTP傳回碼]**：HTTP傳回碼（也稱為HTTP狀態碼）會指出HTTP要求的結果。

1. 此 **[!UICONTROL 處理錯誤]** 選項可讓您在傳輸期間發生任何錯誤時，在活動後啟動「錯誤」出站轉變。

   此外，對於 **檔案傳輸** 型別活動， **[!UICONTROL 處理遺失的檔案]** 選項可讓您在活動後啟動「沒有檔案」出站轉變，如果指定的路徑上沒有檔案。
