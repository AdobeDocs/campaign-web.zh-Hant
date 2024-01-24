---
audience: end-user
title: 探索介面
description: Campaign v8 Web 使用者介面
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
badge: label="有限可用性"
source-git-commit: db318411c9271688b1982acd7f0a23349f18b984
workflow-type: tm+mt
source-wordcount: '1654'
ht-degree: 80%

---

# 探索介面 {#user-interface}

新的 Campaign v8 Web 介面提供了現代直覺的使用者體驗，可簡化行銷活動的設計和傳遞。這個新介面整合 Adobe Experience Cloud 應用程式和解決方案。

瞭解如何連線至Adobe Campaign並探索Experience Cloud導覽基本知識 [本文章](connect-to-campaign.md).


>[!NOTE]
>
>本文件會經常更新以反映產品使用者介面最近的變更。不過，有些螢幕擷取畫面可能會與您的使用者介面稍有不同。

## Campaign首頁 {#user-interface-home}

>[!CONTEXTUALHELP]
>id="acw_homepage_recent"
>title="最近項目"
>abstract="「**最近項目**」清單提供最近建立和修改之傳遞的快速鍵。此清單會顯示其管道、狀態、所有者、建立與修改日期。"

Campaign首頁可讓您快速輕鬆地瀏覽關鍵資源、指標和元件。

首頁的上半區段提供產品中最新更新和可用新功能的詳細資訊，以及發行說明和詳細檔案的連結。 使用向左箭頭捲動功能卡。

![](assets/home.png)

「**關鍵績效指標**」可讓您使用常見的 KPI 值來檢查平台的服務效率。在[本頁面](../reporting/kpis.md)中進一步瞭解這些 KPI。

「**最近項目**」清單提供最近建立和修改之傳遞的快速鍵。此清單會顯示其管道、狀態、所有者、建立與修改日期。按一下「**顯示更多**」連結以載入更多傳遞。

此外，您可以從存取Campaign v8網路金鑰說明頁面 **學習** 區段。

## 左側導覽功能表 {#user-interface-left-nav}

瀏覽左側連結可存取 Campaign v8 Web 功能。幾個連結會顯示可以排序和篩選的物件清單。您也可以設定欄以顯示所有您需要的資訊。請參閱本[章節](#list-screens)。有些清單畫面部分為唯讀。左側導覽功能表與清單中顯示的項目取決於您的使用者權限。若要了解權限的詳細資訊，請參閱[本章節](permissions.md)。


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

  ![](assets/more-actions.png){width="70%" align="left"}

* **工作流程** - 在此畫面中，您可以存取工作流程和工作流程範本的完整清單。您可以檢查其狀態、上次/下次執行日期，並建立新的工作流程或新的工作流程範本。您可以使用和其他物件相同的標準篩選清單。此外，您可以篩選工作流程，無論其是否屬於行銷活動。若要了解工作流程的詳細資訊，請參閱[本章節](../workflows/gs-workflows.md)。


### 內容管理 {#user-interface-content-management}

在內容管理區段中，您可以檢視您的內容範本和片段。

* **內容範本**  — 為了加速及改善設計流程，您可以建立獨立的範本，以便輕鬆重複使用中的自訂內容 [!DNL Adobe Campaign]. 此功能僅適用於電子郵件，可讓內容導向的使用者使用獨立範本，讓行銷使用者可以重複使用並在其自己的電子郵件行銷活動中調整範本。 若要了解詳細資訊，請參閱[本章節](../email/create-email-templates.md)。

<!--
* **Fragments** -
-->

### 客戶管理 {#user-interface-customer-management}

在客戶管理區段中，您可以檢視您的設定檔、對象和訂閱。 這些是唯讀清單。

* **設定檔**  — 建立和管理設定檔，並存取收件者資料庫。 依預設，您可以檢視其電子郵件地址、名字和姓氏。進一步瞭解中的設定檔 [本節](../audience/about-recipients.md).
* **對象** - 這是您的對象清單。依預設，您可以檢視其類型、來源、建立/最後修改日期和標籤。您可以依據來源篩選清單。若要了解對象與清單的詳細資訊，請參閱[本章節](../audience/about-recipients.md)。
* **訂閱服務**  — 瀏覽您的訂閱清單。 預設情況下，您可以檢視其類型、模式和標籤。若要了解如何管理訂閱和取消訂閱，請參閱 [Adobe Campaign v8 (主控台) 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html?lang=zh-Hant){target="_blank"}。
* **預先定義的篩選器**  — 預先定義的篩選器是建立和儲存以供日後使用的自訂篩選器。 在使用查詢模組化工具進行任何篩選作業期間（例如，篩選資料清單或建立傳送的對象時），都可將這些區段當作捷徑。 若要了解詳細資訊，請參閱[本章節](predefined-filters.md)。


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

* **報表** - **報告** 專案提供行銷活動環境中每個管道的流量和參與量度的整合整體摘要。 這些報表包含各種Widget，各可提供行銷活動或傳遞績效的不同觀點。 若要了解詳細資訊，請參閱[本章節](../reporting/global-reports.md)。


## 內容說明 {#user-interface-help}

介面中會提供內容關聯式說明。若有提供，請按一下 `?` 圖示以顯示說明資訊和相關文件的連結。

![](assets/do-not-localize/context-help.png){width="40%" align="left"}

目前已發佈為新Campaign網頁UI的Beta版本， **AI支援的知識助理** 內嵌在內容說明中的內容，革新了檔案搜尋和回答操作方法問題，讓您能夠輕鬆地在龐大的檔案存放庫中篩選，立即找到您需要的精確資訊。

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

<!-- Workflows-->


<!-- delivery template settings-->


>[!CONTEXTUALHELP]
>id="acw_global_reporting_sending"
>title="全球報告傳送"
>abstract="此畫面中會顯示追蹤報告指標"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_tracking"
>title="全球報告追蹤"
>abstract="此畫面中會顯示追蹤報告指標"

>[!CONTEXTUALHELP]
>id="acw_campaign_workflow_list"
>title="活動中的工作流程清單"
>abstract="活動中的工作流程清單"

<!-- delivery settings-->






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
>id="acw_recipients_readonlyprofile"
>title="收件者唯讀設定檔"
>abstract="收件者唯讀設定檔"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_delivery_template"
>title="訂閱傳遞範本"
>abstract="訂閱傳遞範本"

>[!CONTEXTUALHELP]
>id="acw_landingpages_menu"
>title="登陸頁面"
>abstract="登陸頁面"

>[!CONTEXTUALHELP]
>id="acw_landingpages_properties"
>title="登陸頁面屬性"
>abstract="登陸頁面屬性"

>[!CONTEXTUALHELP]
>id="acw_landingpages_pages_list"
>title="登陸頁面頁面"
>abstract="登陸頁面頁面"

>[!CONTEXTUALHELP]
>id="acw_landingpages_schedule"
>title="登陸頁面排程"
>abstract="登陸頁面排程"

>[!CONTEXTUALHELP]
>id="acw_landingpages_primarypage"
>title="登陸頁面主要頁面"
>abstract="登陸頁面主要頁面"

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="登陸頁面訂閱"
>abstract="登陸頁面訂閱"

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="登陸頁面行動號召"
>abstract="登陸頁面行動號召"

>[!CONTEXTUALHELP]
>id="acw_landingpages_simulate"
>title="登陸頁面模擬"
>abstract="登陸頁面模擬"




>[!CONTEXTUALHELP]
>id="acw_orchestration_query_enrichment_noneditable"
>title="活動不可編輯"
>abstract="活動不可編輯"




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

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_profiles_selection"
>title="模擬測試設定檔選擇"
>abstract="模擬測試設定檔選擇"

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_send_testprofiles"
>title="模擬測試設定檔傳送中"
>abstract="模擬測試設定檔傳送中"

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_email_log"
>title="模擬電子郵件記錄"
>abstract="模擬電子郵件記錄"


>[!CONTEXTUALHELP]
>id="acw_directmail_content"
>title="直接郵件的內容"
>abstract="直接郵件的內容"

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_file"
>title="直接郵件的檔案屬性"
>abstract="直接郵件的檔案屬性"

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_content"
>title="直接郵件的內容屬性"
>abstract="直接郵件的內容屬性"


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
>title="此範本僅就緒"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_generatesubsets"
>title="在相同表格中產生所有子集"
>abstract="待定"
