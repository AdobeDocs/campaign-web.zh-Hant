---
audience: end-user
title: 在Campaign中使用AI助理的簡訊
description: 開始使用Campaign中的AI助理
badge: label="Beta"
hide: true
hidefromtoc: true
exl-id: db0459e5-8759-42d9-8945-8c9667450527
source-git-commit: fe687647b0a3d4969373ced400c49b364e878acd
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 9%

---

# 使用 AI 助理產生簡訊 {#generative-sms}

>[!BEGINSHADEBOX]

**內容表**

* [開始使用 AI 助理](generative-gs.md)
* [使用 AI 助理產生電子郵件](generative-content.md)
* 使用 AI 助理產生簡訊
* [使用 AI 助理產生推播](generative-push.md)

>[!ENDSHADEBOX]

當您製作和個人化SMS訊息以符合對象需求後，請利用Campaign中由創新的AI技術支援的AI助理，將您的通訊提升到新的境界。

這個方便使用的工具提供智慧型建議，可精簡您的內容，確保您的訊息能有效地引起共鳴，並最大化參與度。

>[!NOTE]
>
>開始使用此功能之前，請先閱讀相關的[護欄和限制](generative-gs.md#generative-guardrails)。

1. 建立及設定簡訊傳遞之後，請按一下&#x200B;**[!UICONTROL 編輯內容]**。

   如需如何設定SMS傳送的詳細資訊，請參閱[此頁面](../sms/create-sms.md)。

1. 填寫傳遞的&#x200B;**[!UICONTROL 基本詳細資料]**。 完成後，按一下&#x200B;**[!UICONTROL 編輯內容]**。

1. 視需要個人化您的SMS訊息。 [了解更多](../sms/content-sms.md)

1. 存取&#x200B;**[!UICONTROL 顯示AI助理]**&#x200B;功能表。

   ![](assets/sms-genai-1.png){zoomable="yes"}

1. 啟用AI助理的&#x200B;**[!UICONTROL 使用原始內容]**&#x200B;選項，以根據您的傳遞、傳遞名稱和選取的對象來個人化新內容。

   >[!IMPORTANT]
   >
   > 您的提示必須一律繫結至您目前的內容。

1. 說明您要在&#x200B;**[!UICONTROL 提示]**&#x200B;欄位中產生的內容，以微調內容。

   如果您正在尋求製作提示的協助，請存取&#x200B;**[!UICONTROL 提示程式庫]**，它提供各種提示概念，以改進傳送內容。

   ![](assets/sms-genai-2.png){zoomable="yes"}

1. 選取&#x200B;**[!UICONTROL 上傳品牌資產]**&#x200B;以新增任何包含可為AI助理提供額外內容的品牌資產。

1. 使用不同的選項量身打造您的提示：

   * **[!UICONTROL 通訊策略]**：針對產生的文字選取所要的通訊方式。
   * **[!UICONTROL 語言]**：選擇變體內容的語言。
   * **[!UICONTROL 音調]**：確定文字適合您的對象和目的。
   * **[!UICONTROL 長度]**：使用範圍滑桿選取內容的長度。

   ![](assets/sms-genai-3.png){zoomable="yes"}

1. 提示就緒後，請按一下[產生]。****

1. 瀏覽產生的&#x200B;**[!UICONTROL 變數]**，然後按一下&#x200B;**[!UICONTROL 預覽]**&#x200B;以檢視所選變數的全熒幕版本。

1. 瀏覽至&#x200B;**[!UICONTROL 預覽]**&#x200B;視窗中的&#x200B;**[!UICONTROL 調整]**&#x200B;選項，以存取其他自訂功能並微調您的偏好設定變化：

   * **[!UICONTROL 使用作為參考內容]**：選擇的變體將作為參考內容以產生其他結果。

   * **[!UICONTROL 使用較簡單的語言]**： AI助理可以協助您撰寫清晰、簡明的訊息，讓每個人都能理解。

   * **[!UICONTROL 重述]**： AI助理會重述您的訊息，讓不同對象能夠繼續使用內容。

   ![](assets/sms-genai-4.png){zoomable="yes"}

1. 找到適當的內容後，按一下&#x200B;**[!UICONTROL 選取]**。

1. 插入個人化欄位，以根據設定檔資料自訂您的簡訊內容。 [進一步了解內容個人化](../personalization/personalize.md)

   ![](assets/sms-genai-5.png){zoomable="yes"}

1. 定義訊息內容後，按一下&#x200B;**[!UICONTROL 模擬內容]**&#x200B;按鈕以控制呈現，並使用測試設定檔檢查個人化設定。 [了解更多](../preview-test/preview-content.md)

   ![](assets/sms-genai-6.png){zoomable="yes"}

當您定義內容、對象和排程時，就能準備好SMS傳送。 [了解更多](../monitor/prepare-send.md)
