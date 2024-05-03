---
audience: end-user
title: 使用載入檔案工作流程活動
description: 瞭解如何使用載入檔案工作流程活動
exl-id: 230177e2-1926-451a-8a66-0db962ada514
source-git-commit: 4518f7a2f280eca70f799b941c5d28bdc39c1def
workflow-type: tm+mt
source-wordcount: '1227'
ht-degree: 14%

---

# 載入檔案 {#load-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="載入檔案活動"
>abstract="**載入檔案**&#x200B;活動為&#x200B;**資料管理**&#x200B;活動。使用此活動來處理儲存在外部檔案中的資料。 設定檔和資料不會新增至資料庫，但輸入檔案中的所有欄位都可用於個人化、更新設定檔或任何其他表格。 "

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition"
>title="拒絕管理傳出轉變"
>abstract="拒絕管理傳出轉變"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition_reject"
>title="拒絕管理拒絕的傳出轉變"
>abstract="拒絕管理拒絕的傳出轉變"


**載入檔案**&#x200B;活動為&#x200B;**資料管理**&#x200B;活動。使用此活動來處理儲存在外部檔案中的設定檔和資料。 設定檔和資料不會新增至資料庫，但輸入檔案中的所有欄位都可用於 [個人化](../../personalization/gs-personalization.md)，或更新設定檔或任何其他表格。

>[!NOTE]
>支援的檔案格式包括：文字 (TXT) 和逗號分隔值 (CSV)。您可以載入大小上限為50MB的檔案。

此活動可搭配 [調解](reconciliation.md) 活動，將未識別的資料連結至現有資源。 例如， **載入檔案** 活動可放置在 **調解** 活動（如果將非標準資料匯入資料庫）。

## 設定載入檔案活動 {#load-configuration}

此 **載入檔案** 活動設定涉及兩個步驟。 首先，您需要透過上傳範例檔案來定義預期的檔案結構。完成此操作後，您可以指定要匯入其資料的檔案原點。 請依照下列步驟設定活動。

![](../assets/workflow-load-file.png)

### 設定範例檔案 {#sample}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_samplefile"
>title="範例檔案"
>abstract="上傳範例檔案，選取預期的檔案結構。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_formatting"
>title="載入檔案活動的格式化"
>abstract="在 **格式化** 區段，指定檔案的格式，以確保資料正確匯入。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_valueremapping"
>title="載入檔案活動的值重新對應"
>abstract="使用此選項以新值對應載入檔案中的特定值。 例如，如果欄包含「True」/「False」值，您可以新增對應以自動將這些值取代為「0」/「1」字元。"

請依照下列步驟，設定用來定義預期檔案結構的範例檔案：

1. 新增 **載入檔案** 活動放入工作流程。

1. 選取要用來定義預期檔案結構的範例檔案。 若要這麼做，請按一下 **選取檔案** 中的按鈕 **[!UICONTROL 範例檔案]** 區段並選取要使用的本機檔案。

   >[!NOTE]
   >
   >範例檔案的資料用於設定活動，但不匯入。我們建議使用包含少量資料的範例檔案。 檔案格式必須與此對齊 [範例檔案](../../audience/file-audience.md#sample-file).

1. 此時會顯示範例檔案的預覽，最多顯示30行。

1. 在 **[!UICONTROL 檔案型別]** 下拉式清單，指定檔案是使用分隔欄還是固定寬度欄。

   ![](../assets/workflow-load-file-sample.png)

1. 對於分隔欄的檔案型別，請使用 **欄** 區段來設定每個欄的屬性。

   +++檔案欄的可用選項

   * **[!UICONTROL 標籤]**：為欄顯示的標籤。
   * **[!UICONTROL 資料型別]**：欄中包含的資料型別。
   * **[!UICONTROL 寬度]** （字串資料型別）：欄中可顯示的最大字元數。
   * **[!UICONTROL 資料轉換]** （字串資料型別）：將轉換套用至欄中所包含的值。
   * **[!UICONTROL 空格管理]** （字串資料型別）：指定如何管理欄中所包含的空格。
   * **[!UICONTROL 分隔符號]** （日期、時間、整數和數字資料型別）*：指定要作為分隔符號使用的字元。
   * **[!UICONTROL 允許NULL]**：指定如何管理欄中的空白值。 如果出現空值，「Adobe Campaign預設」選項會擲回錯誤。
   * **[!UICONTROL 處理時發生錯誤]** （字串資料型別）：指定其中一行發生錯誤時的行為。
   * **[!UICONTROL 值重新對應]**：此選項可讓您將特定值與新值對應。 例如，如果欄包含「True」/「False」值，您可以新增對應以自動將這些值取代為「0」/「1」字元。

+++

1. 在 **格式化** 區段，指定檔案的格式，以確保資料正確匯入。

### 定義要上傳的目標檔案 {#target}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetfile"
>title="載入檔案活動的目標檔案"
>abstract="在 **[!UICONTROL 目標檔案]** 區段，指定如何擷取檔案以上傳到伺服器上。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_nameofthefile"
>title="檔案名稱"
>abstract="指定要上傳到伺服器上的欄位名稱。 按一下 **[!UICONTROL 開啟個人化對話方塊]** 圖示利用運算式編輯器（包括事件變數）來計算檔案名稱。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetdb"
>title="Target 資料庫"
>abstract="如果您要存取 **[!UICONTROL 載入檔案]** 已在使用者端主控台中設定的活動，這是額外的 **[!UICONTROL 目標資料庫]** 如果您已將活動設定為上傳檔案至外部資料庫，則可使用「 」區段。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_command"
>title="載入檔案命令"
>abstract="允許任意命令進行預處理是一個安全性問題，停用安全選項 XtkSecurity_Disable_Preproc 以強制使用預先定義的命令清單。"

>[!CAUTION]
>
>在載入目標檔案之前，請確定它符合範例檔案格式。 檔案格式、欄結構或欄數的任何差異都可能導致工作流程執行期間發生錯誤。

若要定義要上傳的目標檔案，請執行下列步驟：

1. 在 **[!UICONTROL 目標檔案]** 部分，指定擷取要在伺服器上載的檔案時要執行的動作。

   * **[!UICONTROL 從本機電腦上傳檔案]**：選取要從電腦上傳的檔案。

   * **[!UICONTROL 已在轉變中指定]**：上傳入站轉變中指定的檔案，該轉變源自前一個活動，例如 **[!UICONTROL 傳輸檔案]**.

   * **[!UICONTROL 預先處理檔案]**：上傳上一個轉變中指定的檔案，並套用前置處理命令至該檔案，例如 **[!UICONTROL 解壓縮]** 或 **[!UICONTROL 解密]**.

   * **[!UICONTROL 已計算]**：上傳在中指定名稱的檔案 **[!UICONTROL 檔案名稱]** 欄位。 按一下 **[!UICONTROL 開啟個人化對話方塊]** 圖示利用運算式編輯器（包括事件變數）來計算檔案名稱。

   ![](../assets/workflow-load-file-config.png)

   >[!NOTE]
   >
   >如果您要存取 **[!UICONTROL 載入檔案]** 已在使用者端主控台中設定的活動，這是額外的 **[!UICONTROL 目標資料庫]** 如果您已將活動設定為上傳檔案至外部資料庫，則會顯示區段。 它可讓您指定要將檔案上傳至Campaign伺服器或外部資料庫。

### 其他選項 {#options}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_rejectmgt"
>title="拒絕載入檔案活動的管理"
>abstract="在 **拒絕管理** 區段，指定活動在出現錯誤時的行為方式。 您可以定義允許的最大錯誤數，並切換 **[!UICONTROL 將拒絕專案保留在檔案中]** 選項可在伺服器上下載包含匯入期間發生錯誤的檔案。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_delete"
>title="匯入後刪除檔案"
>abstract="切換「**匯入後刪除檔案**」在匯入檔案後，從伺服器刪除原始檔案。"


1. 在 **拒絕管理** 區段，指定活動在出現錯誤時的行為方式：

   * 在 **[!UICONTROL 刪除]** 欄位，指定處理要載入的檔案時授權的最大錯誤數量。 例如，如果該值設定為「20」，則當載入檔案時出現超過20個錯誤時，工作流程執行將失敗。

   * 若要保留載入檔案時發生的錯誤，請切換 **[!UICONTROL 將拒絕專案保留在檔案中]** 選項開啟，並在 **[!UICONTROL 拒絕檔案]** 欄位。

     啟用此選項後，會在活動後新增一個名為「補充」的額外輸出轉變。 匯入期間發生的任何錯誤都會儲存在伺服器上指定的檔案中。

1. 若要在工作流程執行後從伺服器刪除上傳的檔案，請切換 **[!UICONTROL 匯入後刪除檔案]** 選項。

   ![](../assets/workflow-load-file-options.png)

1. 當設定正確時，按一下「**確認**」。

## 範例 {#load-example}

外部檔案載入的範例，用於 **調解** 活動可在 [本節](reconciliation.md#reconciliation-example).
