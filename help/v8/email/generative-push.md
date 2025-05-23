---
audience: end-user
title: 使用AI助理的推播通知
description: 開始使用AI助理
exl-id: a361f75d-63c2-4fdc-993c-f8414b18e13e
source-git-commit: 5f7fe214c1c89b1ee25cea6d512bd1a55b5522ec
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 2%

---

# 使用AI助理產生推播通知 {#generative-push}

>[!IMPORTANT]
>
>開始使用此功能之前，請先閱讀相關的[護欄和限制](generative-gs.md#generative-guardrails)。
></br>
>
>您必須先同意[使用者合約](https://www.adobe.com/tw/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)，才能在Adobe Campaign Web中使用AI小幫手。 如需詳細資訊，請聯絡您的 Adobe 代表。

AI Assistant可建議與您的對象產生共鳴的不同內容，以協助最佳化傳送的影響。

在下列範例中，AI Assistant用來製作吸引人的訊息，以打造更吸引人的客戶體驗。

1. 建立及設定推播通知傳遞之後，請按一下[編輯內容]。**&#x200B;**

   如需設定推播傳遞的詳細資訊，請參閱[此頁面](../push/create-push.md)。

1. 存取&#x200B;**[!UICONTROL 顯示AI助理]**&#x200B;功能表。

   ![顯示[顯示AI小幫手]功能表的熒幕擷圖](assets/push-genai-1.png){zoomable="yes"}

1. 啟用AI助理的&#x200B;**[!UICONTROL 使用原始內容]**&#x200B;選項，以根據選取的內容個人化新內容。

1. 描述您要在&#x200B;**[!UICONTROL 提示]**&#x200B;欄位中產生的內容，以微調內容。

   如果製作提示時需要協助，請存取&#x200B;**[!UICONTROL 提示程式庫]**，其中提供各種不同的提示概念，以改進傳送內容。

   ![顯示提示程式庫介面的熒幕擷圖](assets/push-genai-2.png){zoomable="yes"}

1. 選擇要產生的欄位： **[!UICONTROL 標題]**、**[!UICONTROL 訊息]**&#x200B;和/或&#x200B;**[!UICONTROL 影像]**。

1. 使用&#x200B;**[!UICONTROL 文字設定]**&#x200B;選項量身打造您的提示：

   * **[!UICONTROL 通訊策略]**：選擇最適合您產生文字的通訊樣式。
   * **[!UICONTROL 音調]**：調整您的電子郵件音調，與您的對象產生共鳴。 無論您是要提供豐富資訊、好玩或有說服力的聲音，AI Assistant都會據以調整訊息。

   ![熒幕擷圖顯示文字設定選項](assets/push-genai-3.png){zoomable="yes"}

1. 選擇您的&#x200B;**[!UICONTROL 影像設定]**：

   * **[!UICONTROL 內容型別]**：將視覺元素的本質分類，區分不同的視覺呈現形式，例如像片、圖形或藝術品。
   * **[!UICONTROL 視覺強度]**：調整影像的強度，控制影像的影響。 較低的設定(2)可建立更柔和、更克制的外觀，而較高的設定(10)則可讓影像更生動、視覺效果更強大。
   * **[!UICONTROL 光線]**：調整影像中的光線，以調整其大氣的形狀，並反白顯示特定的元素。
   * **[!UICONTROL 構成]**：在影像框架中排列元素。

   ![顯示影像設定選項的熒幕擷圖](assets/push-genai-4.png){zoomable="yes"}

1. 從&#x200B;**[!UICONTROL 品牌資產]**&#x200B;功能表，按一下&#x200B;**[!UICONTROL 上傳品牌資產]**，新增任何包含為AI助理提供額外內容的品牌資產，或選取先前上傳的品牌資產。

   先前上傳的檔案可在&#x200B;**[!UICONTROL 已上傳的品牌資產]**&#x200B;下拉式清單中使用。 切換您要納入產生程式的資產。

1. 提示就緒後，請按一下[產生]。**&#x200B;**

1. 瀏覽產生的&#x200B;**[!UICONTROL 變數]**，然後按一下&#x200B;**[!UICONTROL 預覽]**&#x200B;以檢視所選變數的全熒幕版本。

1. 導覽至&#x200B;**[!UICONTROL 預覽]**&#x200B;視窗中的&#x200B;**[!UICONTROL 調整]**&#x200B;選項，以存取其他自訂功能：

   * **[!UICONTROL 使用作為參考內容]**：使用選擇的變體作為參考內容來產生其他結果。
   * **[!UICONTROL 重述]**：以不同的方式重述您的訊息，讓您的寫作保持新鮮，並吸引不同受眾。
   * **[!UICONTROL 使用較簡單的語言]**：簡化您的語言，確保更廣大的受眾能夠清楚無誤地使用。

   您也可以變更文字的&#x200B;**[!UICONTROL 音調]**&#x200B;和&#x200B;**[!UICONTROL 通訊策略]**。

   ![熒幕擷圖顯示精簡選項](assets/push-genai-5.png){zoomable="yes"}

1. 找到適當的內容後，按一下&#x200B;**[!UICONTROL 選取]**。

1. 插入個人化欄位，以根據設定檔資料自訂您的電子郵件內容。 然後，按一下&#x200B;**[!UICONTROL 模擬內容]**&#x200B;按鈕以控制轉譯，並使用測試設定檔檢查個人化設定。 [了解更多](../preview-test/preview-content.md)

   ![顯示模擬內容按鈕的熒幕擷圖](assets/push-genai-6.png){zoomable="yes"}

定義內容、對象和排程時，請準備推送傳送。 [了解更多](../monitor/prepare-send.md)