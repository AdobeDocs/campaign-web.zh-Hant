---
audience: end-user
title: 探索介面
description: Adobe Campaign Web 使用者介面
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
source-git-commit: 145fce5cfaafd0178ca9e85aea6996370c36da9d
workflow-type: tm+mt
source-wordcount: '2295'
ht-degree: 99%

---

# 探索介面 {#user-interface}

新的 Adobe Campaign Web 介面提供了現代直覺的使用者體驗，可簡化行銷活動的設計和傳遞。這個新介面整合 Adobe Experience Cloud 應用程式和解決方案。

[在本文中](connect-to-campaign.md)了解如何連線至 Adobe Campaign，並探索 Experience Cloud 導覽基礎知識。


>[!NOTE]
>
>本文件會經常更新以反映產品使用者介面最近的變更。不過，有些螢幕擷取畫面可能會與您的使用者介面稍有不同。

## Campaign 首頁 {#user-interface-home}

>[!CONTEXTUALHELP]
>id="acw_homepage_recent"
>title="最近項目"
>abstract="「**最近項目**」清單為建立和修改的傳遞提供捷徑。此清單會顯示其管道、狀態、所有者、建立與修改日期。"

Campaign 首頁可讓您快速輕鬆地瀏覽關鍵資源、指標和元件。

首頁的上半區段提供有關產品中可用的最新更新和新功能的詳細資料，以及發行說明和詳細文件的連結。 使用向左箭頭捲動功能卡片。

![](assets/home.png){zoomable=&quot;yes&quot;}

「**關鍵績效指標**」可讓您使用常見的 KPI 值來檢查平台的服務效率。在[本頁面](../reporting/kpis.md)中進一步瞭解這些 KPI。

「**最近項目**」清單為建立和修改的傳遞提供捷徑。此清單會顯示其管道、狀態、所有者、建立與修改日期。按一下「**顯示更多**」連結以載入更多傳遞。

此外，您可以從頁面的「**學習**」區段存取 Adobe Campaign Web 重要說明頁面。

## 左側導覽功能表 {#user-interface-left-nav}

瀏覽左側連結可存取 Adobe Campaign Web 功能。幾個連結會顯示可以排序和篩選的物件清單。您也可以設定欄以顯示所有您需要的資訊。請參閱本[章節](#list-screens)。有些清單畫面部分為唯讀。左側導覽功能表與清單中顯示的項目取決於您的使用者權限。若要了解權限的詳細資訊，請參閱[本章節](permissions.md)。


### 探索工具 {#user-interface-explorer}

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="探索工具"
>abstract="**探索工具**&#x200B;選單會顯示所有 Campaign 元件以及和用戶端主控台中的物件有相同資料夾階層的物件。瀏覽所有 Campaign v8 元件、資料夾和方案，檢查相關聯的權限，並從此選單建立資料夾和子資料夾。"

「**探索工具**」選單會顯示所有 Campaign 資源以及和用戶端主控台中的物件有相同資料夾階層的物件。瀏覽您所有的 Campaign v8 元件、資料夾和結構描述，並建立傳遞、工作流程和行銷活動。

「**探索工具**」中顯示的項目取決於您的使用者權限。如果有適當的權限，您也可以新增資料夾和子資料夾。若要了解權限的詳細資訊，請參閱[本章節](permissions.md)。

您可以設定欄來自訂顯示，以便檢視您需要的所有資訊。請參閱本[章節](#list-screens)。您也可以新增資料夾和子資料夾，請參閱[本章節](permissions.md#folders)以取得詳細資訊。

如需 Campaign 探索工具、資料夾階層和資源的詳細資訊，請參閱此 [Campaign v8 (主控台) 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/campaign-ui.html?lang=zh-Hant#ac-explorer-ui){target="_blank"}。

### 行銷活動管理 {#user-interface-campaign-management}

在「行銷活動管理」區段中，您可以存取行銷活動、傳遞以及工作流程。

* **行銷活動** - 這是您的行銷活動清單以及行銷活動範本。預設情況下，您可以針對每個行銷活動檢視開始/結束/建立/最後修改日期、目前狀態以及建立該活動之行銷活動操作人員的姓名。您可以依狀態、開始/結束日期、資料夾篩選清單，或建立進階篩選以定義您自己的篩選標準。若要了解行銷活動的詳細資訊，請參閱[本章節](../campaigns/gs-campaigns.md)。

* **傳遞** - 瀏覽您的傳遞清單。依預設，您可以檢視其狀態、最後修改日期，以及 KPI。您可以依狀態、聯絡日期或管道篩選清單。按一下電子郵件傳遞來開啟其儀表板以取得傳遞詳細資料概觀。其他管道上的傳遞是唯讀的。若要了解傳遞的詳細資訊，請參閱[本章節](../msg/gs-messages.md)。

  使用「**更多動作**」按鈕來刪除或複製傳遞。

  ![](assets/more-actions.png){zoomable=&quot;yes&quot;}{width="70%" align="left"}

* **工作流程** - 在此畫面中，您可以存取工作流程和工作流程範本的完整清單。您可以檢查其狀態、上次/下次執行日期，並建立新的工作流程或新的工作流程範本。您可以使用和其他物件相同的標準篩選清單。此外，您可以篩選工作流程，無論其是否屬於行銷活動。若要了解工作流程的詳細資訊，請參閱[本章節](../workflows/gs-workflows.md)。


### 內容管理 {#user-interface-content-management}

在「內容管理」區段中，您可以檢視內容範本和片段。

* **內容範本** - 為了加快和改進設計流程，您可以建立獨立範本，以輕鬆地在 [!DNL Adobe Campaign] 重複使用自訂內容。此功能僅適用於電子郵件，讓內容導向的使用者能夠使用獨立範本，以便行銷使用者在自己的電子郵件行銷活動中重複使用和予以調整。 若要了解詳細資訊，請參閱[本章節](../email/create-email-templates.md)。

<!--
* **Fragments** -
-->

### 客戶管理 {#user-interface-customer-management}

在「客戶管理」區段中，您可以檢視設定檔、對象和訂閱。這些是唯讀清單。

* **設定檔** - 建立和管理設定檔，以及存取收件者資料庫。依預設，您可以檢視其電子郵件地址、名字和姓氏。若要深入了解設定檔的詳細資訊，請參閱[本章節](../audience/about-recipients.md)。
* **對象** - 這是您的對象清單。依預設，您可以檢視其類型、來源、建立/最後修改日期和標籤。您可以依據來源篩選清單。若要了解對象與清單的詳細資訊，請參閱[本章節](../audience/about-recipients.md)。
* **訂閱服務** - 瀏覽訂閱清單。預設情況下，您可以檢視其類型、模式和標籤。若要了解如何管理訂閱和取消訂閱，請參閱 [Adobe Campaign v8 (主控台) 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html?lang=zh-Hant){target="_blank"}。
* **預先定義的篩選器** - 預先定義的篩選器是已建立並儲存以供未來使用的自訂篩選器。在使用查詢建模工具進行任何篩選作業時 (例如篩選資料清單或建立傳遞對象時)，可以將它們當作捷徑使用。若要了解詳細資訊，請參閱[本章節](predefined-filters.md)。


### 決策管理 {#decision-management}

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="優惠"
>abstract="瀏覽已使用「**互動**」模組在主控台中建立的優惠清單和優惠範本。這些是唯讀清單。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/offers.html?lang=zh-Hant" text="將優惠新增到傳遞"

在「決策管理」部分，您可以檢視優惠和優惠範本。這些是唯讀清單。

* **優惠** - 瀏覽透過使用「**互動**」模組在主控台建立的優惠清單和優惠範本。依預設，您可以檢視其狀態、開始/結束日期和環境。您可以依狀態和開始/結束日期來篩選清單。也提供優惠範本。

若要了解如何在電子郵件和簡訊中建立和傳送優惠，請參閱[本章節](../msg/offers.md)。

### 報告 {#left-nav-reporting}

* **報告** - 此&#x200B;**報告**&#x200B;項目提供 Campaign 環境中每個管道的流量和參與量度的綜合整體摘要。這些報告是由各種小工具所組成，每個小工具都提供有關您的行銷活動或傳遞績效的獨特觀點。若要了解詳細資訊，請參閱[本章節](../reporting/global-reports.md)。


## 內容說明 {#user-interface-help}

介面中會提供內容關聯式說明。若有提供，請按一下 `?` 圖示以顯示說明資訊和相關文件的連結。

![](assets/do-not-localize/context-help.png){zoomable=&quot;yes&quot;}{width="40%" align="left"}

目前在新的 Campaign Web 使用者介面中發行為 Beta 版本，內嵌於內容說明中&#x200B;**採用 AI 技術的知識助理**&#x200B;可輕鬆篩選大量文件存放庫，並立即找出所需的精確資訊，為文件搜尋和回答操作方法問題方面帶來全面革新。

透過 Campaign Gen AI 的功能，此助理將改變您的體驗，讓資訊檢索和問題解決變得輕而易舉。無論您是在複雜任務中尋求指引，還是導覽大量文件，AI 驅動的知識助理都是您的終極夥伴，在每次互動中提供無與倫比的效率和準確性。

若要了解詳細資訊，請參閱[本章節](using-ai.md)。


## 了解更多 {#learn-more}

了解如何瀏覽、搜尋和篩選 Campaign 環境中的可用清單 ([在此頁面](list-filters.md))。



<!--
######## This part stores the contextualHelp definition for WebUI BETA ###########
######## These blocks should be dispatched in the appropriate pages when available ###########
######## PLEASE DO NOT DELETE ###########
REFER TO 
https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=neolane&title=v8+WebUI+Contextual+Help+%3CALPHA%3E-+Official+list
-->

>[!CONTEXTUALHELP]
>id="acw_push_permission_for_segment"
>title="需要權限"
>abstract="您的管理員必須先授予您權限，然後您才能建立區段。"

>[!CONTEXTUALHELP]
>id="acw_push_overview_edit"
>title="需要權限"
>abstract="您的管理員必須先授予您權限，然後您才能建立區段。"

<!-- delivery template settings-->

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sending"
>title="全球報告傳送"
>abstract="此畫面中會顯示追蹤報告指標"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_tracking"
>title="全球報告追蹤"
>abstract="此畫面中會顯示追蹤報告指標"


<!-- FOR BETA (alignment) -->
<!--https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CBETA%3E-+Official+list-->


<!-- FOR GA -->
<!-- Aligned with https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CGA%3E-+Official+list -->

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_list"
>title="收件者建立"
>abstract="收件者建立"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_cardoverview"
>title="收件者卡片概觀"
>abstract="收件者卡片概觀"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_touchpoints"
>title="收件者接觸點"
>abstract="收件者接觸點"

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_selection"
>title="收件者訂閱選擇"
>abstract="收件者訂閱選擇"

>[!CONTEXTUALHELP]
>id="acw_recipients_offers_eligible_list"
>title="收件者優惠資格符合清單"
>abstract="收件者優惠資格符合清單"

>[!CONTEXTUALHELP]
>id="acw_recipients_offers_preview_proposition"
>title="收件者優惠預覽"
>abstract="收件者優惠預覽"

>[!CONTEXTUALHELP]
>id="acw_fragments_menu"
>title="片段"
>abstract="片段"

>[!CONTEXTUALHELP]
>id="acw_fragments_save"
>title="片段儲存"
>abstract="片段儲存"

>[!CONTEXTUALHELP]
>id="acw_fragments_create"
>title="片段建立"
>abstract="片段建立"

>[!CONTEXTUALHELP]
>id="acw_fragments_properties"
>title="片段屬性"
>abstract="片段屬性"

>[!CONTEXTUALHELP]
>id="acw_fragments_type"
>title="片段類型"
>abstract="片段類型"

>[!CONTEXTUALHELP]
>id="acw_fragments_list"
>title="片段清單"
>abstract="片段清單"

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="片段詳細資料"
>abstract="片段詳細資料"




>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_savefilter"
>title="條件式內容儲存篩選器"
>abstract="條件式內容儲存篩選器"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_selectfilter"
>title="條件式內容選取篩選器"
>abstract="條件式內容選取篩選器"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_subjectline"
>title="主旨行上的條件式內容"
>abstract="主旨行上的條件式內容"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_subjectlinecondition"
>title="條件式內容主旨行條件"
>abstract="條件式內容主旨行條件"


>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_testprofiles"
>title="模擬測試設定檔"
>abstract="模擬測試設定檔"

<!--ML: not visible in UI-->

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_profiles_selection"
>title="模擬測試設定檔選擇"
>abstract="模擬測試設定檔選擇"

<!-- ML: beta wiki page - not visible in UI-->

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_send_testprofiles"
>title="模擬測試設定檔傳送中"
>abstract="模擬測試設定檔傳送中"

<!-- ML: beta wiki page - not visible in UI-->

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_email_log"
>title="模擬電子郵件記錄"
>abstract="模擬電子郵件記錄"

<!-- ML: beta wiki page - not visible in UI-->

<!-- FOR POST-GA -->



<!--
Deprecated IDs - to remove in GA: -->

>[!CONTEXTUALHELP]
>id="acw_attributepicker_advancedfields"
>title="顯示進階屬性"
>abstract="依預設，屬性清單中只會顯示最常見的屬性。啟用「**顯示進階屬性**」開關，即可在規則產生器的左側調色盤中查看目前清單的所有可用屬性，例如節點、群組、1-1 連結、1-N 連結。"

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_advancedfields"
>title="規則產生器進階欄位"
>abstract="依預設，屬性清單中只會顯示最常見的屬性。啟用「**顯示進階屬性**」開關，即可在規則產生器的左側調色盤中查看目前清單的所有可用屬性，例如節點、群組、1-1 連結、1-N 連結。"

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_properties_advanced"
>title="規則產生器進階屬性"
>abstract="依預設，屬性清單中只會顯示最常見的屬性。啟用「**顯示進階屬性**」開關，即可在規則產生器的左側調色盤中查看目前清單的所有可用屬性，例如節點、群組、1-1 連結、1-N 連結。"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_readonlymode"
>title="此範本僅準備就緒"
>abstract="您沒有編輯此範本的權限。如果需要，請聯絡管理員為您授予存取權。"

<!-- Subscription activity-->

>[!CONTEXTUALHELP]
>id="acw_subscriptions_defaultlp"
>title="預設登陸頁面"
>abstract="選取與此訂閱服務關聯的預設登陸頁面。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription"
>title="訂閱服務活動"
>abstract="使用 Adobe Campaign 建立和監視您的服務 (例如電子報)，並檢查這些服務的訂閱或取消訂閱。訂閱僅適用於電子郵件和簡訊傳遞。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_general"
>title="訂閱服務參數"
>abstract="選取並確認訂閱服務的設定。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_outboundtransition"
>title="訂閱服務傳出轉變"
>abstract="切換「**產生傳出轉變**」選項，可在活動之後新增轉變。"


<!--Update file-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata"
>title="更新資料"
>abstract=" **更新資料**&#x200B;活動可執行資料庫欄位的大量更新。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_operationtype"
>title="選取如何更新資料"
>abstract="「**操作類型**」欄位可讓您選擇資料庫資料所要執行的程序。選取第一個選項來新增資料或更新 (如果已新增)。您也可以只新增資料、只更新資料或刪除資料。選取「**更新與合併集合**」，可選取要連結重複項目的主要記錄，並可安全刪除這些重複項目。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_recordid"
>title="記錄識別"
>abstract="指定如何識別資料庫中的記錄：如果資料與現有的目標定位維度相關，請選取「**使用目標定位維度**」選項，然後選取要更新的目標定位維度和欄位。否則，指定一或多個自訂連結來識別資料庫中的資料，或直接使用調和索引鍵。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_fieldsupdate"
>title="選取要更新的欄位"
>abstract="選取要更新的欄位以及調和設定。您可以使用「**自動對應**」選項，以自動識別要更新的欄位。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_advancedoptions"
>title="更新資料的進階選項"
>abstract="**進階選項**&#x200B;區段可讓您指定其他設定來管理資料和重複項目。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_outboundtransition"
>title="產生傳出轉變"
>abstract="切換「**產生傳出轉變**」選項，可新增在執行&#x200B;**更新資料**&#x200B;活動結束時將啟動的傳出轉變。更新通常是標示目標定位工作流程的結束，因此預設不會啟動該選項。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_outboundtransition_rejects"
>title="產生拒絕的傳出轉變。"
>abstract="切換「**產生拒絕的傳出轉變**」選項，可新增包含更新後未正確處理的記錄傳出轉變 (例如，如果有重複資料)。更新通常是標示在目標定位工作流程的結束，因此預設不會啟動該選項。"



<!--External Signal End-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal"
>title="外部訊號"
>abstract="透過&#x200B;**外部訊號**&#x200B;活動，您可以從 API 或其他工作流程觸發工作流程中一組任務的執行。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal_parameters"
>title="外部訊號參數"
>abstract="外部訊號參數"


>[!CONTEXTUALHELP]
>id="acw_orchestration_end_trigger"
>title="結束觸發程序"
>abstract="結束觸發程序"


<!--JavaScript-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript"
>title="JavaScript 程式碼"
>abstract="**JavaScript 程式碼**&#x200B;活動可在工作流程過程中執行 JavaScript 程式碼。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_snippet"
>title="JavaScript 片段"
>abstract="設定要執行的程式碼。"
>additional-url="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/api" text="閱讀 Campaign v8 (主控台) 文件並深入瞭解"


>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_execution"
>title="JavaScript 執行"
>abstract="依預設，執行階段不能超過 1 小時。在這類延遲之後，此流程將中止並顯示錯誤訊息，並且活動執行會失敗。切換「**停止執行於**」選項，可定義自訂延遲。若要忽略此限制，請將值設為 0。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_transition"
>title="處理錯誤"
>abstract="切換「**處理錯誤**」選項，可新增含有錯誤的傳出轉變。"



<!--ExtractFile-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile"
>title="擷取檔案"
>abstract="擷取檔案活動"

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_file"
>title="要擷取的檔案"
>abstract="選取要擷取的檔案。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_destinationformat"
>title="目的地格式"
>abstract="選取格式。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_postprocessing"
>title="後處理"
>abstract="定義後處理步驟"

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_outbound"
>title="傳出轉變"
>abstract="切換「**產生傳出轉變**」選項，可在目前活動之後新增傳出轉變。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_error"
>title="處理錯誤"
>abstract="切換「**處理錯誤**」選項，可新增含有錯誤的傳出轉變。"

<!-- Workflow settings -->

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_initscript"
>title="初始化指令碼"
>abstract="初始化指令碼"

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution_properties"
>title="執行屬性"
>abstract="執行屬性"

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution_error"
>title="執行錯誤"
>abstract="執行錯誤"

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution_initscript"
>title="執行初始化指令碼"
>abstract="執行初始化指令碼"


<!--incremental querry -->

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery"
>title="增量查詢"
>abstract="增量查詢"

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery_history"
>title="增量查詢歷史記錄"
>abstract="增量查詢歷史記錄"

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery_processeddata"
>title="增量查詢已處理的資料"
>abstract="增量查詢已處理的資料"


<!-- Transfer file activity -->

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile"
>title="傳輸檔案"
>abstract="傳輸檔案"

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
>abstract="傳輸檔案遠端伺服器"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_source"
>title="傳輸檔案來源"
>abstract="傳輸檔案來源"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_delete_file"
>title="傳輸後刪除來源檔案"
>abstract="傳輸後刪除來源檔案"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_display_logs"
>title="顯示工作階段記錄"
>abstract="顯示工作階段記錄"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_advancedoptions_list_files"
>title="列出所有檔案"
>abstract="列出所有檔案"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_historization"
>title="檔案歷史化"
>abstract="檔案歷史化"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_missing_file"
>title="處理遺失的檔案"
>abstract="處理遺失的檔案"

>[!CONTEXTUALHELP]
>id="acw_orchestration_transferfile_process_errors"
>title="處理錯誤"
>abstract="處理錯誤"

<!-- Delivery alerting -->

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria"
>title="傳遞警報條件儀表板"
>abstract="傳遞警報條件儀表板"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboards"
>title="傳遞警報儀表板"
>abstract="傳遞警報儀表板"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create"
>title="建立傳遞警報條件"
>abstract="建立傳遞警報條件"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_indicators"
>title="要在警報中新增的指標"
>abstract="要在警報中新增的指標"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_alert"
>title="警報類型"
>abstract="警報類型"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_frequency"
>title="條件頻率"
>abstract="條件頻率"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_criteria_add"
>title="傳遞警報條件"
>abstract="傳遞警報條件"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_general"
>title="傳遞警報一般參數"
>abstract="傳遞警報"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_criteria_parameters"
>title="傳遞警報條件參數"
>abstract="傳遞警報"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboard_alerts"
>title="已傳送的傳遞警報"
>abstract="已傳送的傳遞警報"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboard_history"
>title="傳遞警報歷史記錄"
>abstract="傳遞警報歷史記錄"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboard_create"
>title="建立傳遞警報儀表板"
>abstract="建立傳遞警報儀表板"
