---
audience: end-user
title: 進階設定
description: Campaign v8網頁檔案
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
source-git-commit: 3c7aa37bb74349e88176f1fc75a26bc52e34c628
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 進階設定 {#advanced-settings}

>[!NOTE]
>
>本檔案正在建置中，且經常更新。 此內容的最終版本將於2023年1月推出。

這些設定是電子郵件範本中定義的技術傳送參數。 如果您想要針對特定傳送修改其中任何內容，請小心處理。

## 電子郵件傳送設定 {#email-delivery-settings}

<!--
October 2022 

Note that this page is for now a placeholder to host Contextualhelp blocks

Do not delete these blocks 

Documentation on this part is targeted for december 2022
-->

範本中的所有技術傳送參數。

>[!NOTE]
>
> 僅更改參數，此處不建立。 根據權限。

>[!NOTE]
>
> 實踐者不應修改此內容，請小心。 僅檢查並變更類型規則。

## 分類 {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="分類"
>abstract="類型可讓您控制、篩選及監控傳送的傳送。"

類型是一組類型規則，在訊息分析階段執行。它們可讓您確定您的電子郵件一律包含特定元素（例如，取消訂閱連結或主旨行）或篩選規則，以排除群組不受您預定目標（如取消訂閱者、競爭者或不忠誠客戶）的影響。

將分類與訊息或訊息範本產生關聯時，將執行包含在類型中的類型規則，以檢查消息是否有效。

### 壓力參數 {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="傳遞權重"
>abstract="傳遞權重可讓您識別壓力管理框架內的最優先傳送。 權重最高的報文具有優先順序。"

在本節中，壓力參數可讓您定義臨界值。 這是指定期間內可傳送至一個設定檔的訊息數上限。 一旦達到此臨界值時，在考慮到該期間結束之前，將不再進行傳送。此程序可以讓您在訊息超過設定的臨界值時，自動將設定檔排除在傳送之外，以避免過度請求。

臨界值可以是常數或變數。這表示在指定期間，臨界值可能會因某個設定檔而異，甚至會因為相同的設定檔而有所不同。

在 **權重類型** 欄位，有三個可用選項：（根據選項缺少公式……）

此 **傳送重量** 欄位：每個傳送都有一個權重，代表其優先順序等級。 依預設，傳送的權重會設為5。 壓力規則可讓您定義要套用至的傳送的權重。權重可以透過公式設定或計算，以符合收件者。 例如，您可以根據收件者興趣定義傳送的權重。

此 **傳送模式** 欄位……??

### 容量設定 {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="收件者的重要性"
>abstract="收件者的重要性是一個公式，用於判斷超過容量類型規則時要保留哪些收件者。"

在本節中，您可以選取Adobe Campaign v8主控台中定義的容量規則。 此規則與電子郵件通道相關聯。

此 **收件者的重要性** 欄位是一種公式，用於判斷超過容量類型規則時要保留哪些收件者。

## 對象 {#audience}

在本節中，您可以選取 **目標對應** 在Adobe Campaign v8主控台中定義。 若您使用的收件者表格不是Adobe Campaign提供的表格，則必須建立目標對應。

## 傳遞 {#delivery}

**路由** 選擇：選擇外部帳戶…….

**測試SMTP傳送**:使用此選項可測試透過SMTP的傳送。 會處理傳送，直到連線至SMTP伺服器為止，但不會傳送：對於傳送的每個收件者，Campaign會連線至SMTP提供者伺服器、執行SMTP RCPT TO命令，並在SMTP DATA命令之前關閉連線。

**電子郵件密件副本**:使用此選項，只需將BCC電子郵件地址新增至訊息目標，即可透過BCC在外部系統上儲存電子郵件。

### 重試次數 {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="最大重試次數"
>abstract="如果訊息因暫時錯誤而失敗，則在傳送期間將執行重試。"

由於「軟」或「已忽略」錯誤而暫時未傳送的郵件可能會自動重試。 依預設，會為傳送的第一天排程五次重試，最小間隔為一小時，分散於一天的24小時內。 在此之後，並在「有效性」索引標籤中定義的傳送截止日期之前，每天會寫程式一次重試。

## 核准 {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="核准模式"
>abstract="傳送的每個步驟都需經過核准，以確保對各種程式進行完整監控。"

**手動**:在分析階段結束時，使用者必須確認傳送以開始傳送。

**半自動**:如果分析階段未產生警告訊息，則會自動開始傳送。

**自動**:無論結果如何，發送都會在分析階段結束時自動開始。


## 有效性 {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_duration"
>title="傳遞期間"
>abstract="「傳送持續時間」欄位可讓您輸入全域傳送重試的限制。 這表示Adobe Campaign會傳送從開始日期開始的訊息，然後，對於僅傳回錯誤的訊息，會執行一般、可設定的重試，直到達到有效性限制為止。"

>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="資源效度限制"
>abstract="「有效性限制」欄位是用於上傳的資源，主要用於鏡像頁面和影像。 此頁面上的資源在限定時間內有效。"


此 **傳送持續時間** 欄位可讓您輸入全域傳送重試的限制。 這表示Adobe Campaign會傳送從開始日期開始的訊息，然後，對於僅傳回錯誤的訊息，會執行一般、可設定的重試，直到達到有效性限制為止。

您也可以選擇指定日期。 要執行此操作，請選取 **明確設定有效日期**. 在此情況下，傳送和有效性限制日期也可讓您指定時間。 預設會使用目前時間，但您可以直接在輸入欄位中修改。

**資源有效性限制** 用於上傳的資源，主要用於鏡像頁面和影像。 本頁上的資源在限定時間內有效（以節省磁碟空間）。

### 鏡像頁面管理 {#mirror}

**鏡像頁面管理** 包含四個選項：


### 追蹤 {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="有效期"
>abstract="此選項會定義要在URL上啟動追蹤的持續時間。"

**追蹤有效性限制**:此選項會定義要在URL上啟動追蹤的持續時間。

**過期URL的替代URL**:TBC


## 測試設定 {#test-setttings}

**保持雙倍** 可讓您授權多個傳送給滿足數個鎖定目標的收件者。

**保留已加入封鎖清單的地址**

**保留隔離地址** 可讓您保留任何具有未回應之位址的設定檔，以避免鎖定目標。

**保留校樣的傳送代碼** 可讓您提供與其相關之傳送所定義之傳送代碼相同的校樣。

依預設，校樣的主旨會加上前置詞「校樣#」，其中#代表校樣的編號。 您可以在 **標籤前置詞** 欄位。