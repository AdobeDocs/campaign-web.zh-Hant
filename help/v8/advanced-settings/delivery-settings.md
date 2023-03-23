---
audience: end-user
title: 電子郵件傳送設定
description: 進一步了解Campaign網頁UI中的電子郵件傳送設定
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
source-git-commit: c92e6c1455266fe3430720117d61114ba027b187
workflow-type: tm+mt
source-wordcount: '1471'
ht-degree: 29%

---

# 電子郵件傳送設定 {#email-del-settings}

![Alpha版](../assets/do-not-localize/badge.png)

這些設定包括 **技術傳遞參數** 在電子郵件範本中定義。 可從 **配置傳送設定** 圖示。

## 電子郵件傳送設定 {#email-delivery-settings}

>[!CAUTION]
>
> 這些設定僅供您參考。 其中部分取決於您的設定和權限。 不得在此版本的產品中修改它們。

## 類型 {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="類型"
>abstract="分類可讓您控制、篩選及監視傳遞的傳送。 "

類型是一組&#x200B;**類型規則**，在訊息分析階段執行。它們可讓您確定您的電子郵件一律包含特定元素（例如，取消訂閱連結或主旨行）或篩選規則，以排除群組不受您預定目標（如取消訂閱者、競爭者或不忠誠客戶）的影響。

將類型與訊息或訊息範本產生關聯時，會執行包含在類型中的類型規則，以在訊息準備期間檢查訊息是否有效。

![](assets/delivery-settings-1.png)


### 壓力參數 {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="傳遞權重"
>abstract="傳遞權重可讓您確認壓力管理架構內最優先的傳遞。權重最高的訊息具有優先順序。"

在本節中，壓力參數可讓您定義 **臨界值**. 這是指定期間內可傳送至一個設定檔的訊息數上限。 一旦達到此臨界值時，在考慮到該期間結束之前，將不再進行傳送。此程序可以讓您在訊息超過設定的臨界值時，自動將設定檔排除在傳送之外，以避免過度請求。

臨界值可以是常數或變數。這表示在指定期間，臨界值可能會因某個設定檔而異，甚至會因為相同的設定檔而有所不同。

在 **權重類型** 欄位，有三個可用選項：

* **常數**
* **取決於收件者**
* **已定義在每個規則中**

使用 **傳送重量** 欄位來定義傳送優先順序。 每個傳送都有一個權重，代表其優先順序等級。 依預設，傳送的權重會設為5。 壓力規則可讓您定義套用至傳送的重量。 您可以透過公式來設定或計算加權，以適合收件者。 例如，您可以根據收件者興趣定義傳送的權重。


使用 **傳送模式** 欄位來選取目標評估模式。 提供三種模式：

* **目標預估和訊息個人化**
* **臨時目標的評估和核准**
* **目標評估**

疲勞管理隨附 **促銷活動最佳化** 附加元件。 進一步了解壓力規則以及如何在 [Campaign v8檔案](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html?lang=zh-Hant){target="_blank"}.

### 容量設定 {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="收件者的重要性"
>abstract="收件者的重要性是一種公式，用於確定在超出容量類型規則時要保留哪些收件者。"

在本節中，您可以選取Adobe Campaign v8主控台中定義的容量規則。 此規則與電子郵件通道相關聯。

此 **收件者的重要性** 欄位是一種公式，用於判斷超過容量類型規則時要保留哪些收件者。

進一步了解一致性和容量規則，以及如何在 [Campaign v8檔案](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html){target="_blank"}.


## 對象 {#audience}

在本節中，您可以選取 **目標對應** 其中包括。 目標對應是在Adobe Campaign v8主控台中定義。

進一步了解中的目標對應 [Campaign v8檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html){target="_blank"}.

## 傳遞 {#delivery}

傳遞參數是適用於您傳遞的技術設定。

* **路由**:預設會提供整合式電子郵件路由外部帳戶。 其包含可讓應用程式傳送電子郵件的技術參數。

* **測試SMTP傳送**:此選項可用於測試透過SMTP的傳送。 會處理傳送，直到連線至SMTP伺服器為止，但不會傳送：對於傳送的每個收件者，Campaign會連線至SMTP提供者伺服器、執行SMTP RCPT TO命令，並在SMTP DATA命令之前關閉連線。

* **電子郵件密件副本**:此選項只需新增BCC電子郵件地址至訊息目標，即可透過BCC在外部系統上儲存電子郵件。 進一步了解電子郵件密件副本，位於 [Campaign v8檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.



### 重試次數 {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="最多重試次數"
>abstract="如果訊息由於臨時錯誤而失敗，則會重試到傳遞期間結束為止。"

<!--Temporarily undelivered messages due to a Soft or Ignored error are subject to an automatic retry. By default, five retries are scheduled for the first day of the delivery with a minimum interval of one hour spread out over the 24 hours of the day. -->

進一步了解重試管理，位於 [Campaign v8檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.

## 核准 {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="核准模式"
>abstract="傳遞的每個步驟可能都需要經過核准，以確保對各個流程進行全面監視。"

如果在傳送準備期間產生警告，您可以設定傳送以定義是否應仍執行該傳送。 依預設，使用者必須在分析階段結束時確認訊息的傳送：這是 **手動** 驗證。

您可以在適當欄位中選取其他核准模式。 可用模式包括：

* **手動**:在分析階段結束時，使用者必須確認傳送以開始傳送。

* **半自動**:如果分析階段未產生警告訊息，則會自動開始傳送。

* **自動**:無論結果如何，傳送都會在分析階段結束時自動開始。


## 有效性 {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_duration"
>title="傳遞期間"
>abstract="傳遞期間欄位可讓您輸入全域傳遞重試的限制。這表示 Adobe Campaign 會從開始日期開始傳送訊息，然後，對於僅傳回錯誤的訊息，將執行定期、可設定的重試，直到達到有效期限制。"

>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="資源有效期限制"
>abstract="有效期限制欄位用於上傳的資源，主要適用於鏡像頁面和影像。此頁面上的資源在有限的時間內有效。"


此 **傳送持續時間** 欄位可讓您輸入全域傳送重試的限制。 這表示 Adobe Campaign 會從開始日期開始傳送訊息，然後，對於僅傳回錯誤的訊息，將執行定期、可設定的重試，直到達到有效期限制。

您也可以選擇指定日期。 要執行此操作，請選取 **明確設定有效日期**. 在此情況下，傳送和有效性限制日期也可讓您指定時間。 預設會使用目前時間，但您可以直接在輸入欄位中修改。

**資源有效性限制** 用於上傳的資源，主要用於鏡像頁面和影像。 本頁上的資源在限定時間內有效（以節省磁碟空間）。

![](assets/delivery-settings-2.png)


深入了解傳遞有效期，位於 [Campaign v8檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html#validity-period){target="_blank"}.

### 鏡像頁面管理 {#mirror}

鏡像頁面是可透過網頁瀏覽器線上存取的HTML頁面。 其內容與電子郵件相同。 依預設，如果將連結插入郵件內容中，則會產生鏡像頁面。

除了預設模式外，還提供下列選項：

* **[!UICONTROL 強制產生鏡像頁面]**:即使傳送中未插入鏡像頁面的連結，也會建立鏡像頁面。
* **[!UICONTROL 不生成鏡像頁]**:不會產生任何鏡像頁面，即使傳送中存在連結亦然。
* **[!UICONTROL 生成僅使用消息標識符可訪問的鏡像頁]**:此選項可讓您在傳送記錄視窗中存取鏡像頁面的內容，並附上個人化資訊。 若要這麼做，請在傳送結束後，按一下 **[!UICONTROL 傳送]** 頁簽，並選取您要檢視其鏡像頁面的收件者行。 按一下 **[!UICONTROL 顯示此消息的鏡像頁……]** 連結。


### 追蹤 {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="有效期限"
>abstract="此選項會定義在 URL 上啟動追蹤的期間。"

追蹤參數會在相關區段中定義。 可能的選項包括：

**追蹤有效性限制**:使用此選項可變更在URL上啟動追蹤的持續時間。

**過期URL的替代URL**:使用此選項可輸入後退網頁的URL:追蹤過期後，就會顯示此訊息。

## 測試設定 {#test-setttings}

您可以在本區段中設定排除參數。 可用選項包括：

* **保持雙倍** 可讓您授權多個傳送給滿足數個鎖定目標的收件者。

* **保留已拒絕的地址** 可讓您在取消訂閱（選擇退出）後，將任何不再由傳送定位的設定檔從目標中保留。

* **保留隔離地址** 可讓您保留任何具有未回應之位址的設定檔，以避免鎖定目標。

您也可以自訂測試電子郵件的名稱。

使用 **保留校樣的傳送代碼** 與測試電子郵件建立關聯的傳送代碼，與為其相關的傳送定義的傳送代碼相同。

依預設，測試電子郵件的主旨會加上前置詞「PROOF #」，其中#代表測試電子郵件的編號。 您可以在 **標籤前置詞** 欄位。