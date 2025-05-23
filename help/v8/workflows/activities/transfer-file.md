---
audience: end-user
title: 使用傳輸檔案活動
description: 瞭解如何使用傳輸檔案工作流程活動
exl-id: a40c007e-c0c6-4e0f-aa0d-0260ecb74a03
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '1253'
ht-degree: 27%

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

**傳輸檔案**&#x200B;活動是&#x200B;**資料管理**&#x200B;活動。 它可讓您接收或傳送檔案、測試檔案是否存在，或列出伺服器上的檔案。 使用的通訊協定可以是伺服器對伺服器通訊協定或 HTTP 通訊協定。

>[!NOTE]
>
>使用Campaign網頁使用者介面，將&#x200B;**檔案傳輸**&#x200B;和&#x200B;**網頁下載**&#x200B;功能合併為兩個活動。 此合併不會以任何方式影響活動的功能。

請依照下列詳細步驟設定&#x200B;**傳輸檔案**&#x200B;活動。

## 選擇傳輸通訊協定和作業 {#protocol}

1. 將&#x200B;**傳輸檔案**&#x200B;活動新增至您的工作流程，然後根據您想要使用的通訊協定指定要執行的傳輸型別：

   * 針對HTTP通訊協定，選取&#x200B;**[!UICONTROL 網頁下載]**。 這可讓您執行GET或POST操作，以明確的URL、外部帳戶或Adobe Campaign執行個體下載檔案。
   * 對於其他伺服器對伺服器通訊協定和相關動作，請選取&#x200B;**[!UICONTROL 檔案傳輸]**。

1. 選取要對活動執行的動作。 可用的動作取決於您選取的轉移型別。 請展開下列各節以取得詳細資訊。

   +++可用於&#x200B;**檔案傳輸**&#x200B;型別活動的動作

   * **[!UICONTROL 檔案下載]**：從伺服器下載檔案。
   * **[!UICONTROL 檔案上傳]**：將檔案上傳至伺服器。
   * **[!UICONTROL 測試以檢視檔案是否存在]**：檢查伺服器上是否有指定的檔案。 在活動後產生兩個出站轉變：「檔案存在」和「檔案不存在」。
   * **[!UICONTROL 檔案清單]**：列出伺服器上所有可用的檔案。

   +++

   +++可用於&#x200B;**網頁下載**&#x200B;型別活動的動作

   * **[!UICONTROL 簡單傳輸(GET)]**：擷取檔案。
   * **[!UICONTROL 使用表單(POST)傳輸]**：上傳檔案和其他引數。

   +++

   ![熒幕擷圖顯示工作流程傳輸檔案動作選項](../assets/workflow-transfer-file-action.png)

1. 依預設，針對檔案上傳動作，活動會使用上一個活動中指定的檔案。 若要使用其他檔案，請關閉&#x200B;**[!UICONTROL 使用上一個活動的檔案]**&#x200B;選項，然後按一下&#x200B;**[!UICONTROL 新增檔案]**&#x200B;按鈕。

   在&#x200B;**[!UICONTROL Source]**&#x200B;欄位中，輸入所需的檔案名稱，或使用運算式編輯器使用事件變數計算檔案名稱。 [瞭解如何使用事件變數和運算式編輯器](../event-variables.md)。 重複此作業，視需要儘量新增檔案。

## 定義轉移目的地 {#destination}

1. 在&#x200B;**[!UICONTROL 遠端伺服器]**&#x200B;區段中，指定要使用下列其中一種方法連線的伺服器：

   * **[!UICONTROL 使用外部帳戶中定義的連線引數]**：使用外部帳戶的連線引數連線到伺服器。 在&#x200B;**[!UICONTROL 伺服器資料夾]**&#x200B;欄位中，指定檔案的路徑（或檔案清單動作資料夾的路徑）。
   * **[!UICONTROL 快速組態]**：輸入檔案的URL （或檔案清單動作的資料夾）。
   * **[!UICONTROL Adobe Campaign執行個體]** （網頁下載型別活動）：從Adobe Campaign執行個體伺服器下載檔案。

   ![熒幕擷圖顯示工作流程傳輸檔案伺服器組態選項](../assets/workflow-transfer-file-server.png)

1. 針對Web下載POST動作，您可以透過作業傳遞其他引數。 若要這麼做，請按一下&#x200B;**[!UICONTROL 新增引數]**&#x200B;按鈕，然後指定引數的名稱和值。 您可以視需要新增任意數量的引數。

1. 依預設，對於檔案上傳，會自動儲存上傳至伺服器的檔案。 如果您不想保留這個歷程記錄，請將&#x200B;**[!UICONTROL 保留已傳送檔案的歷程記錄]**&#x200B;選項切換為關閉。

## 歷史化設定 {#historization}

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_historization"
>title="檔案歷史化"
>abstract="每次執行「**[!UICONTROL 轉移檔案]**」活動時，都會將已上傳或已下載的檔案儲存在專用檔案夾中。工作流程的每個轉移檔案活動都會建立一個檔案夾。按照預設，檔案在處理之前會儲存在 Adobe Campaign 安裝資料夾 (`/vars`) 的預設儲存目錄。若要使用特定檔案夾，請關閉「**[!UICONTROL 使用預設儲存目錄]**」選項並輸入目錄路徑。"

每次執行「**[!UICONTROL 轉移檔案]**」活動時，都會將已上傳或已下載的檔案儲存在專用檔案夾中。工作流程的每個轉移檔案活動都會建立一個檔案夾。按照預設，檔案在處理之前會儲存在 Adobe Campaign 安裝資料夾 (`/vars`) 的預設儲存目錄。若要使用特定檔案夾，請關閉「**[!UICONTROL 使用預設儲存目錄]**」選項並輸入目錄路徑。

![熒幕擷圖顯示工作流程傳輸檔案歷史化設定](../assets/workflow-transfer-file-historization.png)

限制此資料夾的大小以保留伺服器上的實體空間很重要。 要執行此操作，請定義活動資料夾的檔案數目上限或總大小。 依預設，授權 100 個檔案和 50 MB。

每次執行活動時，都會檢查資料夾，如下所示：

* 只考慮在活動執行前 24 小時以上建立的檔案。
* 如果考慮的檔案數超過&#x200B;**[!UICONTROL 檔案數]**&#x200B;欄位的值，則會刪除最舊的檔案，直到達到允許的檔案數上限為止。
* 如果考慮的檔案總大小超過&#x200B;**[!UICONTROL 大小上限(MB)]**&#x200B;引數的值，則會刪除最舊的檔案，直到達到允許的大小上限。

>[!CAUTION]
>
>如果活動未再次執行，則不會檢查或清除其資料夾。 傳輸大型檔案時請務必小心。

## 進階和錯誤管理選項 {#advanced}

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_delete_file"
>title="轉移後刪除來源檔案"
>abstract="成功轉移後清除來源檔案。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_display_logs"
>title="顯示工作階段記錄"
>abstract="與轉移作業相關的資訊會顯示在工作流程記錄中。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_list_files"
>title="列出所有檔案"
>abstract="此選項會將伺服器上存在的所有檔案編成索引並儲存在 **vars.filenames** 事件變數中。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_missing_file"
>title="處理遺失的檔案"
>abstract="您可以使用這個選項，在活動後啟動「**無檔案**」傳出轉變。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_errors"
>title="處理錯誤"
>abstract="您可以利用這個選項，在活動後啟動「**錯誤**」傳出轉變。"

1. 在&#x200B;**[!UICONTROL 進階選項]**&#x200B;中，根據您設定的活動型別，有其他選項可供使用。 請展開下列各節以取得詳細資訊。

   +++其他&#x200B;**[!UICONTROL 檔案傳輸]**&#x200B;型別活動的選項

   * **[!UICONTROL 傳輸後刪除來源檔案]**：成功傳輸後清除來源檔案。
   * **[!UICONTROL 顯示工作階段記錄檔]**：啟動此選項時，工作流程記錄檔中會顯示與傳輸作業相關的資訊。
   * **[!UICONTROL 列出所有檔案]** （檔案清單動作）：此選項會索引`vars.filenames`事件變數中伺服器上存在的所有檔案，其中檔案名稱以`n`個字元分隔。 [瞭解如何使用事件變數](../event-variables.md)

   +++

   +++**[!UICONTROL 網頁下載]**&#x200B;型別活動的其他選項

   * **[!UICONTROL 遵循重新導向]**：檔案重新導向可讓您使用覆寫，將資料輸入或輸出導向到其他型別的裝置。
   * **[!UICONTROL 將HTTP標頭新增至檔案]**：在某些情況下，您可能想要將額外的HTTP標頭新增至檔案。 最常見的情況是，這些標頭將用於提供其他資訊以進行疑難排解、用於[跨原始資源共用(CORS)](https://developer.mozilla.org/docs/Web/HTTP/CORS)，或用於設定特定的快取指示。
   * **[!UICONTROL 忽略HTTP傳回碼]**： HTTP傳回碼（也稱為HTTP狀態碼）表示HTTP要求的結果。

1. 如果傳輸期間發生任何錯誤，**[!UICONTROL 處理錯誤]**&#x200B;選項可讓您在活動後啟動「錯誤」出站轉變。

   此外，對於&#x200B;**檔案傳輸**&#x200B;型別活動，**[!UICONTROL 處理遺漏檔案]**&#x200B;選項可讓您在活動後啟動「無檔案」出站轉變（如果指定路徑上沒有檔案）。