---
audience: end-user
title: 電子郵件傳遞設定
description: 進一步了解 Campaign Web UI 中的電子郵件傳遞設定
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '1471'
ht-degree: 95%

---


# 電子郵件傳遞設定 {#email-del-settings}

這些設定是在電子郵件範本中定義的&#x200B;**技術傳遞參數**。它們可從「**設定傳遞設定**」圖示取得，編輯電子郵件傳遞時會出現此圖示。

## 電子郵件傳遞設定 {#email-delivery-settings}

>[!CAUTION]
>
> 這些設定僅供您參考。其中一些取決於您的設定和權限。不可在此版本的產品中修改它們。

## 類型 {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="類型"
>abstract="分類可讓您控制、篩選及監視傳遞的傳送。 "

類型是一組&#x200B;**類型規則**，在訊息分析階段執行。它們可讓您確定您的電子郵件一律包含特定元素（例如，取消訂閱連結或主旨行）或篩選規則，以排除群組不受您預定目標（如取消訂閱者、競爭者或不忠誠客戶）的影響。

將類型與訊息或訊息範本產生關聯時，在訊息準備期間將執行包含在類型中的類型規則以檢查訊息是否有效。

![](assets/delivery-settings-1.png)


### 壓力參數 {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="傳遞權重"
>abstract="傳遞權重可讓您確認壓力管理架構內最優先的傳遞。權重最高的訊息具有優先順序。"

在此區段中，壓力參數可讓您定義&#x200B;**臨界值**。這是在一段時間內可以傳送到一個設定檔的訊息數上限。一旦達到此臨界值時，在考慮到該期間結束之前，將不再進行傳送。此程序可以讓您在訊息超過設定的臨界值時，自動將設定檔排除在傳送之外，以避免過度請求。

臨界值可以是常數或變數。這表示在指定期間，臨界值可能會因某個設定檔而異，甚至會因為相同的設定檔而有所不同。

「**權重類型**」欄位提供三個選項：

* **常數**
* **取決於收件者**
* **已定義在每個規則中**

使用「**傳遞權重**」欄位可定義傳遞優先順序。每個傳遞都有權重，代表其優先順序。傳遞的預設權重為 5。壓力規則可讓您定義套用到它們的傳遞權重。權重可以設定或透過公式計算以適合收件者。例如，您可以根據收件者的興趣定義傳遞權重。


使用「**傳遞模式**」欄位可選取目標評估模式。提供三種模式：

* **目標預估和訊息個人化**
* **臨時目標的評估和核准**
* **目標評估**

**行銷活動最佳化** 附加元件隨附疲勞管理。如需進一步了解壓力規則以及如何設定疲勞管理，請參閱 [Campaign v8 文件](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=zh-Hant){target="_blank"}。

### 產能設定 {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="收件者的重要性"
>abstract="收件者的重要性是一種公式，用於確定在超出產能類型規則時要保留哪些收件者。"

在此區段中，您可以選取在 Adobe Campaign v8 主控台中定義的產能規則。此規則與電子郵件管道相關聯。

「**收件者的重要性**」欄位是一種公式，用於確定在超出產能類型規則時要保留哪些收件者。

如需進一步了解一致性與產能規則以及如何設定它們，請參閱 [Campaign v8 文件](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html){target="_blank"}。


## 對象 {#audience}

在此區段中，您可以選取其中可用的&#x200B;**目標對應**。目標對應是在 Adobe Campaign v8 主控台中定義的。

如需進一步了解目標對應，請參閱 [Campaign v8 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html){target="_blank"}。

## 傳遞 {#delivery}

傳遞參數是套用到傳遞的技術設定。

* **路由**：預設提供整合的電子郵件路由外部帳戶。其包含可讓應用程式傳送電子郵件的技術參數。

* **測試 SMTP 傳遞**：此選項用於測試透過 SMTP 傳送。處理傳遞直到連線到 SMTP 伺服器，但不傳送：對於傳遞的每個收件者，Campaign 會連線到 SMTP 提供者伺服器，執行 SMTP RCPT TO 命令，並在 SMTP DATA 命令之前關閉連線。

* **電子郵件 BCC**：此選項用於透過 BCC 將電子郵件儲存在外部系統上，只需將 BCC 電子郵件地址新增到您的訊息目標即可。如需進一步了解電子郵件 BCC，請參閱 [Campaign v8 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}。



### 重試次數 {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="最多重試次數"
>abstract="如果訊息由於臨時錯誤而失敗，則會重試到傳遞期間結束為止。"

<!--Temporarily undelivered messages due to a Soft or Ignored error are subject to an automatic retry. By default, five retries are scheduled for the first day of the delivery with a minimum interval of one hour spread out over the 24 hours of the day. -->

如需進一步了解重試管理，請參閱 [Campaign v8 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}。

## 核准 {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="核准模式"
>abstract="傳遞的每個步驟可能都需要經過核准，以確保對各個流程進行全面監視。"

如果在傳遞準備期間產生警告，您可以設定傳遞以定義它是否仍應執行。依預設，使用者必須在分析階段結束時確認傳送訊息：這是&#x200B;**手動**&#x200B;驗證。

您可以在相關欄位選取另一個核准模式。可用的模式包括：

* **手動**：分析階段結束時，使用者必須確認傳遞開始傳送。

* **半自動**：如果分析階段未產生警告訊息，會自動開始傳送。

* **自動**：分析階段結束時會自動開始傳送，不論分析的結果為何。


## 有效期 {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_duration"
>title="傳遞期間"
>abstract="「傳遞期間」欄位可讓您輸入全域傳遞重試的限制。這表示 Adobe Campaign 會從開始日期開始傳送訊息，然後，僅對於傳回錯誤的訊息，執行定期、可設定的重試，直到達到有效期限制。"

>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="資源有效期限制"
>abstract="「有效期限制」欄位用於上傳的資源，例如鏡像頁面或影像。這些資源在有限的時間內有效：一旦達到限制，資源將不再可用。"


「**傳遞期間**」欄位可讓您輸入全域傳遞重試的限制。這表示 Adobe Campaign 會從開始日期開始傳送訊息，然後，僅對於傳回錯誤的訊息，執行定期、可設定的重試，直到達到有效期限制。

您也可以選擇指定日期。為此，請選取「**明確設定有效日期**」。在此情況下，傳遞和有效期限制日期也讓您指定時間。預設使用目前時間，但您可以直接在輸入欄位中修改。

**資源有效期限制**&#x200B;用於上傳的資源，主要適用於鏡像頁面和影像。本頁面的資源在限定時間內有效 (以節省磁碟空間)。在此限制之後，這些資源將不再可用。

![](assets/delivery-settings-2.png)


如需進一步了解傳遞有效期限，請參閱 [Campaign v8 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html#validity-period){target="_blank"}。

### 鏡像頁面管理 {#mirror}

鏡像頁面是可透過網頁瀏覽器線上存取的 HTML 頁面。其內容與電子郵件相同。依預設，如果將連結插入郵件內容中，則會產生鏡像頁面。

除預設模式之外，還有提供以下選項：


* **[!UICONTROL 強制產生鏡像頁面]**：使用此模式產生鏡像頁面，即使無鏡像頁面連結插入到傳遞中。
* **[!UICONTROL 不要產生鏡像頁面]**：使用此模式可以避免產生鏡像頁面，即使傳遞有連結存在。
* **[!UICONTROL 產生僅可使用訊息識別碼存取的映象頁面]**：當電子郵件內容中不存在映象頁面連結時，使用此選項可啟用從使用者端主控台在傳送記錄視窗中存取映象頁面內容。


### 追蹤 {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="有效期限"
>abstract="此選項會定義在 URL 上啟動追蹤的期間。"

追蹤參數是在相關區段中定義。可能的選項包括：

**追蹤有效期限制**：使用此選項可變更在 URL 上啟動追蹤的期間。

**過期 URL 的替代 URL**：使用此選項輸入後備網頁的 URL：追蹤過期後顯示。

## 測試設定 {#test-setttings}

您可以設定在此區段設定排除參數。可使用的選項包括：

* **維持雙面**&#x200B;可讓您授權對滿足多個目標定位條件的收件者進行多個傳遞。

* **保留已加入封鎖清單的地址**&#x200B;可讓您遠離目標，任何不再作為傳遞目標的設定檔，例如在取消訂閱 (選擇退出) 之後。

* **保留被隔離的地址**&#x200B;可讓您遠離目標，任何具有不會回應之地址的設定檔。

您也可以自訂測試電子郵件的名稱。

使用「**保留傳遞程式碼用於校訂**」將測試電子郵件與傳遞程式碼相關聯，此傳遞程式碼與其相關之傳遞的傳遞程式碼相同。

依預設，測試電子郵件的主旨會以「PROOF #」為前置詞，其中#是測試電子郵件的編號。 您可以在「**標籤前置詞**」欄位變更此前置詞。