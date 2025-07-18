---
audience: end-user
title: 設定傳送設定
description: 瞭解如何在Campaign網頁版中設定傳遞設定
feature: Email, Push, SMS, Direct Mail, Cross Channel Orchestration
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
source-git-commit: 5835d45ea2a383eed7d280fdd263548ea2e8530d
workflow-type: tm+mt
source-wordcount: '3159'
ht-degree: 43%

---


# 設定傳遞設定 {#del-settings}

傳遞設定是在傳遞範本中定義的&#x200B;**技術傳遞引數**。 每個傳遞都能讓這些量度超載。 這些設定可從編輯傳遞或傳遞範本時可用的&#x200B;**設定**&#x200B;按鈕取得。

>[!CAUTION]
>
>這些設定僅供您參考。其中一些取決於您的設定和權限。不可在此版本的產品中修改它們。

## 類型設定 {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="類型"
>abstract="您可以利用類型將所有傳遞的業務實務標準化。類型是類型規則的集合，可讓您控制、篩選傳遞的傳送並排定其優先順序。在準備階段，與類型規則中的標準相符的設定檔會排除在傳遞對象之外。"

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_typology"
>title="傳遞的類型設定"
>abstract="您可以利用類型規則將所有傳遞的業務實務標準化。類型是類型規則的集合，可讓您控制、篩選傳遞的傳送並排定其優先順序。在準備階段，與類型規則中的標準相符的設定檔會排除在傳遞對象之外。"

型別是一組&#x200B;**型別規則**，在準備階段執行，以便一次輕鬆將多個篩選規則套用至傳遞。 它們可讓行銷人員標準化所有傳送的業務實務，讓他們控制、篩選傳送內容並安排傳送內容的優先順序。 [瞭解如何建立型別與型別規則](../administration/typologies.md)

![](assets/delivery-settings-typology.png){zoomable="yes"}

### 壓力參數 {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_pressure_parameters"
>title="傳遞壓力參數"
>abstract="傳遞權重可讓您確認疲勞管理架構內最優先的傳遞。權重最高的訊息具有最高優先。"

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_weight"
>title="傳遞權重"
>abstract="傳遞權重可讓您確認壓力管理架構內最優先的傳遞。權重最高的訊息具有最高優先。"

在本節中，壓力引數可讓您定義&#x200B;**臨界值**&#x200B;以設定疲勞管理規則，此規則是在指定期間內可傳送至一個設定檔的最大訊息數量。

一旦達到此臨界值時，在考慮到該期間結束之前，將不再進行傳送。此程序可以讓您在訊息超過設定的臨界值時，自動將輪廓排除在傳送之外，以避免過度請求。

臨界值可以是常數或變數。這表示在指定期間，臨界值可能會因某個輪廓而異，甚至會因為相同的輪廓而有所不同。

「**[!UICONTROL 權重類型]**」欄位提供三個選項：

* **[!UICONTROL 常數]**
* **[!UICONTROL 取決於收件者]**
* **[!UICONTROL 已定義在每個規則中]**

使用「**[!UICONTROL 傳遞權重]**」欄位可定義傳遞優先順序。每個傳遞都有權重，代表其優先順序。傳遞的預設權重為 5。壓力規則可讓您定義套用到它們的傳遞權重。權重可以設定或透過公式計算以適合收件者。例如，您可以根據收件者的興趣定義傳遞權重。

使用&#x200B;**[!UICONTROL 傳遞模式]**&#x200B;欄位來選取目標評估模式。

提供三種模式：

* **[!UICONTROL 目標預估和訊息個人化]**
* **[!UICONTROL 臨時目標的評估和核准]**
* **[!UICONTROL 目標評估]**

>[!NOTE]
>
>疲勞管理和壓力規則是在Campaign使用者端主控台中設定。 在[Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=zh-Hant){target="_blank"}中進一步瞭解。

### 容量設定 {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_capacity_settings"
>title="傳遞的容量設定"
>abstract="在傳遞訊息之前，請使用容量規則以確保您的組織可以處理傳遞、傳遞可能產生的傳入訊息，以及用於聯絡訂閱者的呼叫次數等。容量規則是在 Adobe Campaign v8 主控台中定義。在此畫面中，選取一個與頻道關聯的規則。"

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_recipient_importance"
>title="收件者的重要性"
>abstract="收件者的重要性是一種公式，用來確定在超出容量類型規則時要保留哪些設定檔。"

在此區段中，您可以選取Adobe Campaign v8主控台中定義的容量規則。 此規則已與管道相關聯。

收件者&#x200B;**欄位的**&#x200B;重要性是公式，用來決定超過容量型別規則時保留哪些設定檔。

>[!NOTE]
>
>型別規則是在Campaign使用者端主控台中設定。 在[Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html?lang=zh-Hant){target="_blank"}中進一步瞭解。

## 對象設定 {#audience}

>[!CONTEXTUALHELP]
>id="acw_email_settings_audience"
>title="傳遞的對象設定"
>abstract="在那些可用項目中選取「**目標對應**」。目標對應是在 Adobe Campaign v8 主控台中定義的。您也可以設定傳遞的排除參數。"

在此區段中，您可以選取其中可用的&#x200B;**目標對應**。目標對應是在 Adobe Campaign v8 主控台中定義的。目標對應是作業正在處理的資料型別。 它可讓您定義目標母體：收件者、合約受益者、操作者、訂閱者等。 [進一步瞭解目標對應](../audience/targeting-dimensions.md)。

在&#x200B;**[!UICONTROL 排除]**&#x200B;欄位中，您可以選取排除不想再聯絡或隔離的設定檔。 [了解更多](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html?lang=zh-Hant){target="_blank"}

## 傳遞 {#delivery}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery"
>title="傳遞的全域設定"
>abstract="傳遞參數是套用到傳遞的技術設定。您可以變更傳遞和例行模式、啟動電子郵件密件副本、使用波段傳送，也可以選擇傳送電子郵件的格式。這些選項僅限於專業使用者。"

**[!UICONTROL 傳遞]**&#x200B;引數為套用至傳遞的技術設定。

![](assets/delivery-settings-delivery.png){zoomable="yes"}

預設會提供整合的&#x200B;**[!UICONTROL 路由]**&#x200B;外部帳戶。 其中包含可讓應用程式傳送傳遞的技術引數。

您可以定義下面的&#x200B;**[!UICONTROL 傳送]**&#x200B;設定。

* **[!UICONTROL 傳遞優先順序]**：使用此選項可設定您的傳遞的優先順序層級，以變更其傳送順序：正常、高或低。

* **[!UICONTROL 訊息批次數量]**：使用此選項可定義在同一XML傳遞套件中分組的訊息數量。 如果引數設為0，訊息會自動分組。 封裝大小由計算`<delivery size>/1024`定義，每個封裝至少有8個和256個訊息。

  >[!IMPORTANT]
  >
  >當透過複製現有傳遞建立傳遞時，此引數會重設。

* **[!UICONTROL 測試SMTP傳遞]** （電子郵件通道）：此選項用於測試透過SMTP的傳送。 電子郵件會處理到連線至SMTP伺服器，但不會傳送：對於每個電子郵件收件者，Campaign會連線至SMTP提供者伺服器、執行SMTP RCPT TO命令，並在SMTP DATA命令之前關閉連線。

* **[!UICONTROL 電子郵件密件副本]** （電子郵件頻道）：此選項是用來透過密件副本在外部系統上儲存電子郵件，只要將密件副本電子郵件地址新增到您的郵件目標即可。 在[Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/emails/email-bcc.html?lang=zh-Hant){target="_blank"}中進一步瞭解。

在&#x200B;**[!UICONTROL 波段定義]**&#x200B;區段中，選取&#x200B;**[!UICONTROL 使用多個波段傳送]**&#x200B;選項，以逐步增加使用波段傳送的音量。 這可避免您的郵件被標示為垃圾郵件，或您想要限制每天的郵件數。 使用波段您可以將傳送劃分為幾個批次，而不是同時傳送大量訊息。 [了解更多](send-using-waves.md)

對於電子郵件，您也可以變更已傳送郵件的&#x200B;**[!UICONTROL 郵件格式]**，如下所述。

* **[!UICONTROL 使用收件者偏好設定]** （預設模式）：電子郵件格式是根據儲存在收件者設定檔中的資料所定義。 如果收件者希望以特定格式接收電子郵件，則此格式為傳送的格式。 如果未填入欄位，則會傳送替代的多重部分電子郵件（請參閱下文）。

* **[!UICONTROL 讓收件者郵件使用者端選擇最合適的格式]**：電子郵件包含兩種格式：文字和HTML。 接收時顯示的格式取決於收件者郵件軟體的設定（替代的多重部分）。

  >[!IMPORTANT]
  >
  >此選項包含檔案的兩個版本。 因此，它會影響傳遞率，因為電子郵件大小較大。

* **[!UICONTROL 以文字格式傳送所有郵件]**：電子郵件是以文字格式傳送。 不會傳送HTML格式，但只有當收件者按一下電子郵件時，才會用於映象頁面。

## 網站分析 {#web-analytics}

>[!CONTEXTUALHELP]
>id="acw_email_settings_webanalytics"
>title="傳遞的網站分析設定"
>abstract="選取網路分析帳戶。此帳戶是在 Campaign 用戶端主控台中設定的。您也可以定義與您所用分析工具共用的標籤。"

您可以在此區段中選取網站分析帳戶。 此帳戶是在Campaign使用者端主控台中設定。

您也可以定義與您所用分析工具共用的標籤。

>[!NOTE]
>
>Web Analytics功能是在Campaign使用者端主控台中設定。 在[Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html?lang=zh-Hant#external-account-ac){target="_blank"}中進一步瞭解。

## 重試次數 {#retries}

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_retries"
>title="最多重試次數"
>abstract="如果訊息由於臨時錯誤而失敗，則會重試到傳遞期間結束為止。"

<!--Currently not visible in UI > ??-->

因軟性或忽略錯誤而暫時未傳送的郵件可能會自動重試。 根據預設，排程在傳送的第一天進行五次重試，最小間隔為一小時分佈在一天中的24小時。

## 核准 (電子郵件頻道) {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="傳遞的核准模式"
>abstract="選取「核准模式」。如果在傳遞準備期間產生警告，您可以設定傳遞以定義它是否仍應執行。"

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_approval"
>title="傳遞的核准模式"
>abstract="根據該範本選取傳遞的核准模式。如果在傳遞準備期間產生警告，您可以設定傳遞以定義它是否仍應執行。"

如果在電子郵件傳送準備期間產生警告，您可以設定傳送以定義是否仍應執行。 依預設，使用者必須在分析階段結束時確認傳送電子郵件：這是&#x200B;**手動**&#x200B;驗證。

您可以在相關欄位選取另一個核准模式。可用的模式包括：

* **[!UICONTROL 手動]**：分析階段結束時，使用者必須確認傳遞開始傳送。
* **[!UICONTROL 半自動]**：如果分析階段未產生警告訊息，會自動開始傳送。
* **[!UICONTROL 自動]**：分析階段結束時會自動開始傳送，不論分析的結果為何。

## 有效性 {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_validity"
>title="設定有效性"
>abstract="「**傳遞期間**」欄位可讓您輸入全域傳遞重試的限制。這表示 Adobe Campaign 會傳送從開始日期開始的訊息，然後，對於僅傳回錯誤的訊息，會執行一般、可設定的重試，直到達到效度限制為止。「<br>**資源效度限制**」欄位是用於上傳的資源，主要用於鏡像頁面和影像。一旦達到限制，資源將不可再供使用。"

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_resources_validity"
>title="資源效度限制"
>abstract="「**資源效度限制**」欄位是用於上傳的資源，主要用於鏡像頁面和影像。這些資源在有限的時間內有效：一旦達到限制，資源將不再可用。"

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_duration"
>title="傳遞期間"
>abstract="「**傳遞期間**」欄位可讓您輸入全域傳遞重試的限制。這表示 Adobe Campaign 會傳送從開始日期開始的訊息，然後，對於僅傳回錯誤的訊息，會執行一般、可設定的重試，直到達到效度限制為止。"

<!--
>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Resources validity limit"
>abstract="The Validity limit field is used for uploaded resources, such as the mirror page or images. These resources are valid for a limited time: once the limit is reached, resources are no longer available."
-->

### 有效期限 {#validity-period}

「**[!UICONTROL 傳遞期間]**」欄位可讓您輸入全域傳遞重試的限制。這表示 Adobe Campaign 會傳送從開始日期開始的訊息，然後，對於僅傳回錯誤的訊息，會執行一般、可設定的重試，直到達到效度限制為止。

您也可以選擇指定日期。為此，請選取「**[!UICONTROL 明確設定有效日期]**」。在此情況下，傳遞和有效期限制日期也讓您指定時間。預設使用目前時間，但您可以直接在輸入欄位中修改。

**[!UICONTROL 資源效度限制]**&#x200B;是用於上傳的資源，主要用於映象頁面和影像。 本頁面的資源在限定時間內有效 (以節省磁碟空間)。在此限制之後，這些資源將不再可用。

![](assets/delivery-settings-validity.png){zoomable="yes"}

<!--Change screenshot to be consistent with prod > not sure which version is correct-->

在[Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html?lang=zh-Hant#validity-period){target="_blank"}中進一步瞭解傳遞有效期。

### 映象頁面管理（電子郵件通道） {#mirror}

鏡像頁面是可透過網頁瀏覽器線上存取的 HTML 頁面。其內容與電子郵件相同。根據預設，如果將連結插入電子郵件的內容中，則會產生映象頁面。

除預設模式之外，還有提供以下選項：

* **[!UICONTROL 強制產生映象頁面]**：即使電子郵件中未插入任何映象頁面的連結，也使用此模式產生映象頁面。
* **[!UICONTROL 不要產生映象頁面]**：使用此模式可避免產生映象頁面，即使電子郵件中存在連結亦然。
* **[!UICONTROL 產生僅可使用郵件識別碼存取的映象頁面]**：當電子郵件內容中不存在映象頁面連結時，請使用此選項啟用從使用者端主控台在傳遞記錄視窗中存取映象頁面的內容。

### 追蹤 {#tracking}

<!--
>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Validity period"
>abstract="This option defines the duration for which the tracking is activated on the URLs."
-->

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_tracking_validity"
>title="有效期限"
>abstract="有效期會設定在訊息 URL 上啟動追蹤的持續時間。"

**[!UICONTROL 追蹤]**&#x200B;引數已在相關區段中定義。 可能的選項包括：

* **[!UICONTROL 追蹤效度限制]**：使用此選項變更在URL上啟用追蹤的持續時間。
* **[!UICONTROL 過期URL的替代URL]**：使用此選項可輸入後援網頁的URL：追蹤過期後就會顯示。

## 校樣設定 {#test-setttings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_testsettings"
>title="定義傳遞的校樣設定"
>abstract="選取排除參數並自訂校樣的標籤。"

<!--Test to be replaced with Proof everywhere - currently not consistent within UI > changed to Proof to reflect UI here but not consistent in documentation either-->

您可以設定在此區段設定排除參數。可使用的選項包括：

* **[!UICONTROL 保留雙面]**&#x200B;可讓您授權多個傳送給符合數個目標定位條件的設定檔。
* **[!UICONTROL 保留已加入封鎖清單的地址]**&#x200B;可讓您遠離目標，任何不再作為傳遞目標的輪廓，例如在取消訂閱 (選擇退出) 之後。
* **[!UICONTROL 保留被隔離的地址]**&#x200B;可讓您遠離目標，任何具有不會回應之地址的輪廓。

您也可以自訂校樣的標籤：

* 使用證明的&#x200B;**[!UICONTROL 保留傳遞代碼]**，以便與為其相關傳遞定義的傳遞代碼相同傳遞代碼關聯到證明。
* 依預設，校訂的主題會以「PROOF #」為前置詞，其中#是校訂的編號。 您可以在「**[!UICONTROL 標籤前置詞]**」欄位變更此前置詞。

## 簡訊設定 (簡訊管道) {#sms-tab}

>[!CONTEXTUALHELP]
>id="acw_sms_delivery_settings"
>title="簡訊傳遞設定"
>abstract="簡訊傳遞參數是套用到簡訊傳遞的技術設定。您可以定義寄件者地址、服務參數、傳輸模式等。這些選項僅限於專業使用者。"

簡訊傳遞參數是套用到簡訊傳遞的技術設定。您可以定義寄件者地址、服務參數、傳輸模式等。這些選項僅限於專業使用者。

<!--

* **[!UICONTROL Sender address]**

  The field is limited to 21 characters by the SMPP specification, but some providers may allow longer values. Note also that very strict restrictions may be applied in some countries (length, content, allowed characters, …), so you may need to double-check that the content you place here is legal. Be especially careful when using personalized fields.


  This optional field allows you to override the sender address (oADC). Its content is placed in the *source_addr* field of the SUBMIT_SM PDU.

  Although the SMPP specification limits this field to 21 characters, some providers may support longer values. Be aware that certain countries impose strict regulations on sender addresses (regarding length, content, allowed characters, etc.), so always verify that your input complies with local requirements. Use extra caution when working with personalized fields.

  If this field is left empty, the value of the Source number field defined in the external account will be used instead. If both values are empty, the *source_addr* field will be left empty.

-->

* **[!UICONTROL 服務型別]**：

  此引數會依原樣傳遞至提供者。

* **[!UICONTROL 服務或程式ID]**

  >[!NOTE]
  >
  >不建議使用此欄位。 使用者端主控台中可用的選用SMPP引數可提供更具彈性的實施。
  >
  >此欄位不能與選用的SMPP引數同時使用。

  結合相符的外部帳戶設定，允許隨每個MT傳送一個可選引數。 此欄位會定義TLV的值部分。

* **[!UICONTROL 傳輸模式]**

  此欄位會定義要傳送的SMS型別：這是一般或快閃訊息，以及是否應儲存在行動裝置或SIM卡上。 此設定會在SUBMIT_SM PDU的dest_addr_subunit選擇性欄位中傳輸。

   * **Flash**&#x200B;將值設為1。 傳送立即在熒幕上顯示且未儲存的Flash SMS。
   * **Normal**&#x200B;將值設為0。 傳送標準SMS。
   * **儲存在行動裝置上**&#x200B;將值設為2。 指示裝置將簡訊儲存在內部記憶體中。
   * **儲存在終端機**&#x200B;上，將值設為3。 指示裝置將簡訊儲存在SIM卡上。

* **[!UICONTROL 優先順序，通訊型別]**

  擴展SMPP聯結器會忽略這些欄位。

* **[!UICONTROL 每則訊息的最大SMS數目]**

  此設定僅在訊息裝載選項停用時有效（如需詳細資訊，請參閱外部帳戶設定）。 如果訊息需要的SMS數量超過此值，則會觸發錯誤。

  雖然SMS通訊協定允許將訊息分割為最多255個部分，但有些行動裝置可能難以重新組合超過10個部分的訊息（此限制取決於裝置型號）。 為了保持可靠性，最好將郵件限制在5個或更少的部分。

  請注意，由於個人化訊息在Adobe Campaign中的運作方式，訊息大小可能會有所不同。 大量長訊息可能會導致傳送成本增加，因此使用合理的限制有助於控制費用。

  將此值設定為0會停用限制。

## 電子郵件傳遞適用的 SMTP 設定 {#smtp}

>[!CONTEXTUALHELP]
>id="acw_email_settings_smtp"
>title="SMTP 參數"
>abstract="您可以新增電子郵件傳遞的其他 SMTP 參數。"

您可以將其他SMTP引數新增至電子郵件傳遞。 您可以在傳送設定的SMTP標籤中執行此作業。

![](assets/smtp_tab.png){zoomable="yes"}

### 字元編碼 {#character-encoding}

**[!UICONTROL 字元編碼]**&#x200B;區段可讓您設定特定編碼。 預設編碼為UTF-8，適用於大多數字元。 但是，如果某些電子郵件提供者不支援UTF-8標準編碼，則可能無法正確顯示特殊字元。

例如，如果您想要傳送包含日文字元的電子郵件，最好使用專門支援這些字元的編碼，好讓您在日本的對象可以正確看到所有內容。

若要這麼做，請啟動&#x200B;**[!UICONTROL 強制用於訊息的編碼]**&#x200B;切換按鈕，並從支援特殊字元的清單中選取正確的編碼。

![](assets/smtp_encoding.png){zoomable="yes"}

### 退回電子郵件 {#bounce-emails}

傳遞設定的&#x200B;**[!UICONTROL SMTP]**&#x200B;標籤可讓您同時設定退回郵件的管理。

* **[!UICONTROL 錯誤對位址]**：如果您啟用&#x200B;**[!UICONTROL 使用為平台]**&#x200B;切換定義的預設錯誤位址，則會在平台的預設錯誤方塊中接收退回的電子郵件。 如果您未啟用此功能，您可以為傳送定義特定的錯誤地址。

* **[!UICONTROL 退信地址]**：您也可以定義其他未處理退信電子郵件的轉寄地址。 此位址可讓您在應用程式無法自動限定電子郵件時，調查退回的原因。

這兩個欄位可以個人化，如[本節](../personalization/gs-personalization.md)中所述。

![](assets/smtp_bounce.png){zoomable="yes"}

### 其他 SMTP 標頭 {#smtp-headers}

您可以在傳遞設定的SMTP索引標籤中，將&#x200B;**[!UICONTROL SMTP標頭]**&#x200B;新增至您的電子郵件傳遞。

在此視窗中輸入的指令碼必須參考以下格式的每行一個標題： name：value。

如有必要，會自動對值編碼。

![](assets/smtp_headers.png){zoomable="yes"}


>[!IMPORTANT]
>
>會為進階使用者保留新增指令碼，以便插入其他 SMTP 標題。此指令碼的語法必須符合以下內容類型的要求：沒有未使用的空間，沒有空行等。

## 新增變數 {#variables-delivery}

>[!CONTEXTUALHELP]
>id="acw_delivery_settings_variable"
>title="變數"
>abstract="您可以在傳遞中新增變數，以供追蹤和個人化使用。您可以透過傳遞內容和工作流程存取這些變數。"

您可以在傳遞中新增變數，以供追蹤和個人化使用。您可從傳遞內容和工作流程存取這些變數。 儲存的變數可用來設定傳送內所有訊息中保持不變的值。 您也可以在傳遞範本中設定這些變數。

若要新增變數，請瀏覽至&#x200B;**[!UICONTROL 變數]**&#x200B;標籤，如下所示。

![](assets/variables-tab.png){zoomable="yes"}

按一下&#x200B;**[!UICONTROL 新增變數]**&#x200B;按鈕以輸入變數的詳細資料。 您可以透過啟動核取方塊&#x200B;**[!UICONTROL 值是運算式]**&#x200B;的結果，直接新增其值或使用運算式。 然後按一下&#x200B;**[!UICONTROL 確認]**&#x200B;以儲存變更。

![](assets/variables-add.png){zoomable="yes"}

深入瞭解[使用變數進行個人化](../personalization/personalize.md#variables-personalization)以及[使用變數進行動態內容](../personalization/conditions.md#variables-conditional)。