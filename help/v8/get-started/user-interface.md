---
audience: end-user
title: 探索介面
description: Campaign v8 Web 使用者介面
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
badge: label="Alpha"
source-git-commit: 970a7c7af8b94e96d33ef2e41f8ddcfda322252c
workflow-type: tm+mt
source-wordcount: '1726'
ht-degree: 99%

---

# 探索介面 {#user-interface}

>[!CONTEXTUALHELP]
>id="acw_homepage_learnmore"
>title="探索介面"
>abstract="新的 Campaign v8 Web 介面提供了整合、直覺和一致性的使用者體驗。"

新的 Campaign v8 Web 介面提供了現代直覺的使用者體驗，可簡化行銷活動的設計和傳遞。這個新介面與 Adobe Experience Platform 整合在一起。


>[!NOTE]
>
>本文件會經常更新以反映產品使用者介面最近的變更。不過，有些螢幕擷取畫面可能會與您的使用者介面稍有不同。


## 左側導覽功能表 {#user-interface-left-nav}

瀏覽左側連結可存取 Campaign v8 Web 功能。幾個連結會顯示可以排序和篩選的物件清單。您也可以設定欄以顯示所有您需要的資訊。請參閱本[章節](#list-screens)。所有清單畫面都是唯讀的，電子郵件傳遞清單除外。按一下清單項目以編輯/檢視的這個功能在 Alpha 版本未提供。在未來的版本，所有清單將可編輯。左側導覽功能表顯示的項目取決於您的使用者權限。

![](assets/home.png)

### 首頁 {#user-interface-home}

此畫面包含快速存取主要 Campaign v8 Web 功能的重要連結和資源。

「**最近項目**」清單提供最近建立和修改之傳遞的快速鍵。此清單會顯示其管道、狀態、所有者、建立與修改日期。

「**關鍵績效指標**」可讓您使用常見的 KPI 值來檢查平台的服務效率。

從首頁的「**學習**」區段存取 Campaign v8 Web 重要說明頁面。

### 探索工具 {#user-interface-explorer}

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="探索工具"
>abstract="**探索工具**&#x200B;選單會顯示所有 Campaign 元件以及和用戶端主控台中的物件有相同資料夾階層的物件。瀏覽您所有的 Campaign v8 元件、資料夾和結構描述，並建立傳遞、工作流程和行銷活動。所有其他清單都是唯讀。"

**探索工具**&#x200B;選單會顯示所有 Campaign 資源以及和用戶端主控台中的物件有相同資料夾階層的物件。瀏覽您所有的 Campaign v8 元件、資料夾和結構描述，並建立傳遞、工作流程和行銷活動。所有其他清單都是唯讀。

探索工具中顯示的項目取決於您的使用者權限。

如同任何清單畫面，您可以設定欄來個人化顯示以檢視所有您需要的資訊。請參閱本[章節](#list-screens)。

如需 Campaign 探索工具、資料夾階層和資源的詳細資訊，請參閱此 [Campaign v8 (主控台) 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/campaign-ui.html#ac-explorer-ui){target="_blank"}。

### 行銷活動管理 {#user-interface-campaign-management}

>[!CONTEXTUALHELP]
>id="acw_campaigns_list"
>title="行銷活動"
>abstract="這是您的行銷活動清單。您可以檢視有用的資訊，例如其開始/結束/最後修改日期，以及其狀態。您可以依狀態或開始/結束日期篩選清單。按一下「建立行銷活動」按鈕，即可新增行銷活動。選取行銷活動，檢視其內容、傳遞和詳細資料。瀏覽到「範本」標籤，檢視和建立範本。"



在「行銷活動管理」區段中，您可以存取行銷活動、傳遞以及工作流程。

* **行銷活動** - 這是您的行銷活動清單以及行銷活動範本。預設情況下，您可以針對每個行銷活動檢視開始/結束/建立/最後修改日期、目前狀態以及建立該活動之行銷活動操作人員的姓名。您可以依狀態、開始/結束日期、資料夾篩選清單，或建立進階篩選以定義您自己的篩選標準。若要了解行銷活動的詳細資訊，請參閱[本章節](../campaigns/gs-campaigns.md)。

* **傳遞** - 瀏覽您的傳遞清單。依預設，您可以檢視其狀態、最後修改日期，以及 KPI。您可以依狀態、聯絡日期或管道篩選清單。按一下電子郵件傳遞來開啟其儀表板以取得傳遞詳細資料概觀。其他管道上的傳遞是唯讀的。若要了解傳遞的詳細資訊，請參閱[本章節](../msg/gs-messages.md)。

  使用「**更多動作**」按鈕來刪除或複製傳遞。

  ![](assets/more-actions.png){width="70%" align="left"}

* **工作流程** - 在此畫面中，您可以存取工作流程和工作流程範本的完整清單。您可以檢查其狀態、上次/下次執行日期，並建立新的工作流程或新的工作流程範本。您可以使用和其他物件相同的標準篩選清單。此外，您可以篩選工作流程，無論其是否屬於行銷活動。若要了解工作流程的詳細資訊，請參閱[本章節](../workflows/gs-workflows.md)。


### 客戶管理 {#user-interface-customer-management}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="收件者"
>abstract="存取您的收件者資料庫。您可以檢視有用的資訊，例如其電子郵件地址、名字和姓氏。此為唯讀清單。"

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="對象"
>abstract="這是您的對象清單。您可以檢視其類型、來源、建立/最後修改日期和標籤。您可以依據來源篩選清單。此為唯讀清單。"

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="訂閱清單"
>abstract="瀏覽您的訂閱清單。您可以檢視其類型、模式和標籤。此為唯讀清單。"


在「客戶管理」區段中，您可以檢視您的收件者、對象和訂閱。這些是唯讀清單。

* **收件者** - 存取您的收件者資料庫。依預設，您可以檢視其電子郵件地址、名字和姓氏。若要了解收件者的詳細資訊，請參閱 [Adobe Campaign v8 (主控台) 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/gs-audiences.html){target="_blank"}。
* **對象** - 這是您的對象清單。依預設，您可以檢視其類型、來源、建立/最後修改日期和標籤。您可以依據來源篩選清單。若要了解對象和清單的詳細資訊，請參閱 [Adobe Campaign v8 (主控台) 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html){target="_blank"}。
* **訂閱** - 瀏覽您的訂閱清單。預設情況下，您可以檢視其類型、模式和標籤。若要了解如何管理訂閱和取消訂閱，請參閱 [Adobe Campaign v8 (主控台) 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html){target="_blank"}。

### 決策管理

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="優惠"
>abstract="瀏覽您的互動優惠清單。依預設，您可以檢視其狀態、開始/結束日期和環境。您可以依狀態和開始/結束日期來篩選清單。也提供優惠範本。這些是唯讀清單。"

* **優惠** - 覽您的互動優惠清單。依預設，您可以檢視其狀態、開始/結束日期和環境。您可以依狀態和開始/結束日期來篩選清單。也提供優惠範本。這些是唯讀清單。

若要了解如何建立管理優惠方案，請參閱 [Adobe Campaign v8 (主控台) 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html){target="_blank"}。

## 頂端列

使用介面的頂端列進行以下作業：

* 以 Alpha 測試人員身份分享您的意見回饋
* 在組織和實例之間切換
* 在 Adobe Experience Cloud 應用程式之間切換
* 存取說明頁面、聯絡支援人員和分享意見回饋。您可以從搜尋欄位搜尋說明文章和影片。

![](assets/unified-shell.png){width="50%" align="left"}
<!--
Org / Sub-org switcher to switch between instances. Only one for Alpha. Later: intermerdiate screen with Control Panel (beta). if v8 + ACS with one card per ACS instance. Maybe quickly explain the menu for Alpha?
-->

## 內容說明 {#contextual-help}

介面中會提供內容關聯式說明。若有提供，請按一下 `?` 圖示以顯示說明資訊和相關文件的連結。

![](assets/context-help.png){width="40%" align="left"}

<!--An on-boarding guide is also available to help you get started with Campaign v8 Web. Click the icon in the bottom right corner, choose one of the available step-by-step scenarios, and simply follow the instructions.

![](assets/onboarding.png){width="70%" align="left"}-->

## 支援的瀏覽器 {#browsers}

Campaign v8 Web 目的是要在最新版本的 Google Chrome、Safari 和 Microsoft Edge 中以最佳方式運作。您可能無法在舊版本或其他瀏覽器上使用某些功能。

## 語言偏好設定 {#language-pref}

Campaign v8 Web 目前提供以下語言版本：

<table>
<tr>
<td>
<p>英文 (US) - EN-US</p>
<p>法文 - FR</p>
<p>德文 - DE</p>
<p>義大利文 - IT</p>
</td>
<td>
<p>西班牙文 - ES</p>
<p>葡萄牙文 (巴西) - PTBR</p>
<p>日文 - JP</p>
</td>
<td>
<p>韓文 - KR</p>
<p>簡體中文 - CHS</p>
<p>繁體中文 - CHT</p>
</td>
</tr>
</table>

您的預設介面語言由使用者設定檔中指定的偏好語言決定。

若要變更您的語言：

1. 按一下右上角您的設定檔圖示，然後選取「**偏好設定**」。
1. 然後，按一下您電子郵件地址下顯示的語言連結。
1. 選取您偏好的語言，然後按一下「**儲存**」。您可以選取第二語言，以防您使用的元件沒有您第一語言的版本。


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
>id="acw_targetdata_personalization_enrichmentdata"
>title="擴充資料"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sending"
>title="報告傳送"
>abstract="參閱行銷活動報告的傳送指標。"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_tracking"
>title="報告追蹤"
>abstract="參閱行銷活動報告的追蹤指標。"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_overview"
>title="報告概觀"
>abstract="傳遞的關鍵量度。"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_target"
>title="報告目標統計資料"
>abstract="本章節會根據對象顯示特定的量度。"

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_selection"
>title="傳遞的彙總報告"
>abstract="選取至少兩個傳遞，以顯示彙總的資料報告。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="重複資料刪除 - 重複欄位"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="重複資料刪除 - 重複設定"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="重複資料刪除 - 重複補充"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="維度補充"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_push_permission_for_segment"
>title="需要權限"
>abstract="您的管理員必須先授予您權限，然後您才能建立區段。"

>[!CONTEXTUALHELP]
>id="acw_push_overview_edit"
>title="需要權限"
>abstract="您的管理員必須先授予您權限，然後您才能建立區段。"


>[!CONTEXTUALHELP]
>id="acw_campaign_read_only"
>title="此行銷活動為唯讀資料"
>abstract="您沒有編輯此行銷活動的權限。如果需要，請聯絡管理員為您授予存取權限。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_read_only"
>title="此傳遞為唯讀資料"
>abstract="您沒有編輯此傳遞的權限。如果需要，請聯絡管理員為您授予存取權限。"

>[!CONTEXTUALHELP]
>id="acw_subscription_services_read_only"
>title="此服務為唯讀資料"
>abstract="您沒有編輯此服務的權限。如果需要，請聯絡管理員為您授予存取權限。"

<!-- Workflows-->

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_workflow"
>title="工作流程清單"
>abstract="您的行銷活動可使用的工作流程清單。使用「建立工作流程」按鈕在您的行銷活動中新增工作流程。"

>[!CONTEXTUALHELP]
>id="acw_orchestration_saveaudience_outbound"
>title="為儲存對象傳出轉變"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_orchestration_saveaudience_activity"
>title="儲存對象"
>abstract="使用此活動來儲存工作流程對象。"


>[!CONTEXTUALHELP]
>id="acw_wf_read_only"
>title="此工作流程為唯讀"
>abstract="您沒有編輯此工作流程的權限。如果需要，請聯絡管理員授予您存取的權限。"

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="此工作流程為唯讀資料"
>abstract="由於畫布不受支援或不相容，您無法編輯此工作流程。"

<!-- delivery template settings-->

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_tracking_validity"
>title="有效期限"
>abstract="此選項會定義在 URL 上啟動追蹤的持續時間。"

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_duration"
>title="傳遞期間"
>abstract="「傳遞期間」欄位可讓您輸入全域傳遞重試的限制。這表示 Adobe Campaign 會傳送從開始日期開始的訊息，然後，對於僅傳回錯誤的訊息，會執行一般、可設定的重試，直到達到效度限制為止。"

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_resources_validity"
>title="資源效度限制"
>abstract="「效度限制」欄位是用於上傳的資源，主要用於鏡像頁面和影像。這些資源在有限的時間內有效：一旦達到限制，資源將不再可用。"

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_approval"
>title="核准模式"
>abstract="傳遞的每個步驟可能都需要經過核准，以確保對各個流程進行全面監視。"

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_retries"
>title="最多重試次數"
>abstract="如果訊息由於臨時錯誤而失敗，則會重試到傳遞期間結束為止。"

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_recipient_importance"
>title="收件者的重要性"
>abstract="收件者的重要性是一種公式，用於確定在超出產能類型規則時要保留哪些收件者。"

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_weight"
>title="傳遞權重"
>abstract="傳遞權重可讓您確認壓力管理架構內最優先的傳遞。權重最高的訊息具有優先順序。"

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_typology"
>title="類型"
>abstract="分類可讓您控制、篩選及監視傳遞的傳送。 "

>[!CONTEXTUALHELP]
>id="acw_reporting_email_exportation"
>title="匯出"
>abstract="您只能匯出選取的頁面。"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sending"
>title="全域報告傳送"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_tracking"
>title="全域報表追蹤"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_campaign_delivery_list"
>title="Campaign 中的傳遞清單"
>abstract="Campaign 中的傳遞清單"

>[!CONTEXTUALHELP]
>id="acw_campaign_workflow_list"
>title="活動中的工作流程清單"
>abstract="活動中的工作流程清單"

<!-- delivery settings-->

>[!CONTEXTUALHELP]
>id="acw_email_settings_audience"
>title="傳遞設定對象"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="傳遞設定核准"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_email_settings_testsettings"
>title="傳遞設定測試設定"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_email_settings_webanalytics"
>title="傳遞設定網站分析"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_delivery_template_for_campaign"
>title="Campaign 中的傳遞範本"
>abstract="待定"

>[!CONTEXTUALHELP]
>id="acw_workflow_template_for_campaign"
>title="Campaign 中的工作流程範本"
>abstract="待定"
