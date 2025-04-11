---
audience: end-user
title: 使用波段傳送
description: 進一步瞭解Campaign網頁中的傳遞設定
feature: Email
exl-id: d4cd5fe5-f9ac-44ac-a961-ae45131aeb3e
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 13%

---

# 使用波段傳送 {#send-using-waves}

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_definition"
>title="將傳遞內容分成幾批次"
>abstract="定義波段以將傳遞內容分成幾批次，而不是同時傳送大量訊息。您可以設定多個相同大小的波段，或為要傳送的不同波段設定行事曆。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_size"
>title="定義每個波段的大小"
>abstract="您必須輸入要新增之所有波段的大小。輸入數值 (每個波段的訊息數量) 或百分比 (0-100%)。"

若要平衡負載，您可以將電子郵件傳送劃分為幾個批次。 設定批次數量及其相對於整個傳送的比例，以及兩個批次之間的間隔。

>[!NOTE]
>
>您只能定義兩個連續波段之間的大小和延遲。 無法調整每個波次的收件者選取條件。

若要使用波段傳送傳遞，請遵循下列步驟。

1. 開啟[傳遞設定](delivery-settings.md#retries)。

1. 瀏覽至&#x200B;**[!UICONTROL 傳遞]**&#x200B;區段。

1. 選取&#x200B;**[!UICONTROL 使用多個波段傳送]**&#x200B;選項。

1. 若要設定波段，您可以：

   * [排定大小相同的多個波段](#waves-same-size)
   * [根據行事曆排定波段](#waves-calendar)

1. 照常準備並傳送您的傳遞。 [了解更多](../msg/gs-deliveries.md)

   >[!CAUTION]
   >
   >請確定最後批次不超過[有效性](delivery-settings.md#validity)標籤中定義的傳遞期限，否則可能無法傳送部分訊息。 特定型別控制規則&#x200B;**[!UICONTROL 波段排程檢查]**&#x200B;可確保最後一個波段是在傳遞有效期限之前計畫。 在[Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html?lang=zh-Hant)中進一步瞭解控制規則。
   >
   >在設定最後一個波段時，您也必須允許足夠的重試時間。 [了解更多](delivery-settings.md#retries)

1. 若要監視您的傳送，請移至[傳遞記錄](../monitor/delivery-logs.md)。 您可以看到已在已處理批次中傳送的傳遞（**[!UICONTROL 已傳送]**&#x200B;狀態）以及將在剩餘批次中傳送的傳遞（**[!UICONTROL 擱置中]**&#x200B;狀態）。

## 排定大小相同的多個波段 {#waves-same-size}

如果選取此選項，則所有波段的大小都相同（最後一個波段除外），而且每個波段之間的延遲始終相同。

![大小相同的波段範例](assets/waves-same-size.png){zoomable="yes"}

* 指定您要分割傳遞的所有波段的大小。 您可以輸入百分比或數值。 只有最後一個波段的大小可以不同，因為它必須包含剩餘的訊息數量。

  例如，如果您在&#x200B;**[!UICONTROL 波段大小]**&#x200B;欄位中輸入&#x200B;**[!UICONTROL 30%]**，前三個波段代表傳遞中包含的所有訊息的30%，第四個波段代表剩餘的10%。

* 在&#x200B;**[!UICONTROL 間隔]**&#x200B;區段中，指定兩個連續波段開始之間的延遲。 例如，如果您輸入&#x200B;**[!UICONTROL 2天]**，第一個波段會立即開始，第二個波段會在兩天內開始，第三個波段會在四天內開始，依此類推。

使用數個相同大小的批次的常見使用案例是涉及呼叫中心。 管理電話忠誠度行銷活動時，貴組織處理聯絡訂閱者之通話次數的能力有限。

使用波段時，您可以將每天的訊息數量限製為20，這是客服中心的每日處理能力。

若要這麼做，請選取&#x200B;**[!UICONTROL 排程多個相同大小的波段]**&#x200B;選項。 輸入&#x200B;**[!UICONTROL 20]**&#x200B;作為波段大小，並在&#x200B;**[!UICONTROL 間隔]**&#x200B;欄位中輸入&#x200B;**[!UICONTROL 1天]**。

![呼叫中心處理的波段範例](assets/waves-call-center.png){zoomable="yes"}

## 根據行事曆排定波段 {#waves-calendar}

如果您選取此選項，請定義您傳送之每個波次的開始日/時間，以及每個波次的大小。

* 在&#x200B;**[!UICONTROL 開始]**&#x200B;欄位中，指定兩個連續波段開始之間的延遲。

* 在&#x200B;**[!UICONTROL 大小]**&#x200B;欄中，輸入固定數字或百分比。

視需要新增多個波段。 根據您的要求重新排序。

>[!NOTE]
>
>如果您使用百分比，則所有波段的總和不應超過100%。

在以下範例中，第一個波段代表傳送中包含之訊息總數的25%，而且會立即開始。 接下來的兩個批次會完成傳遞，並設定為每六小時開始一次。

![行事曆排程的波段範例](assets/waves-calendar.png){zoomable="yes"}

根據行事曆使用多個波段的常見使用案例是在向上移動過程中。

使用新平台傳送電子郵件時，網際網路服務提供者(ISP)會懷疑無法辨識的IP位址。 如果突然傳送大量電子郵件，ISP通常會將其標籤為垃圾郵件。

為避免標籤為垃圾訊息，請逐步增加使用波段傳送的數量。 這可以確保啟動階段的順利發展，並降低無效位址的整體比率。

若要這麼做，請使用&#x200B;**[!UICONTROL 根據行事曆]**&#x200B;選項排程波段。 例如，將第一個波段設為10%，將第二個波段設為15%，將第三個波段設為20%，以此類推。

![遞增流程的波次範例](assets/waves-ramp-up.png){zoomable="yes"}