---
audience: end-user
title: 傳送校樣
description: 瞭解如何定義和傳送校樣
exl-id: b2677579-c95d-443d-b207-466af364c208
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 15%

---

# 傳送校樣 {#send-test-deliveries}

>[!CONTEXTUALHELP]
>id="acw_email_preview_mode"
>title="預覽模式"
>abstract="將測試母體納入主要目標，以預覽和測試訊息。"

定義訊息內容後，您可以傳送校樣到測試設定檔，以預覽和測試訊息。 如果您已插入個人化內容，您可以使用測試設定檔資料檢查此內容在訊息中的顯示方式。

若要偵測訊息內容或個人化設定中可能出現的錯誤，請先傳送校樣至測試設定檔，再傳送給目標對象。 每次進行變更時都應傳送校樣，以驗證最新內容。 傳送校樣是驗證行銷活動和識別潛在問題的重要步驟。 校樣收件者可以檢查各種元素，例如連結、選擇退出連結、影像或映象頁面，並偵測轉譯、內容、個人化設定和傳遞設定中的任何錯誤。

## 使用測試設定檔模擬內容 {#simulate-content-test-deliveries}

>[!CONTEXTUALHELP]
>id="acw_email_preview_option_test_target"
>title="測試母體"
>abstract="選取測試母體模式。"

在傳送校樣之前，請務必定義傳送的目標對象。 [了解更多](../audience/add-audience.md)

若要開始測試訊息內容：

1. 編輯傳送的內容。
1. 按一下 **[!UICONTROL 模擬內容]** 按鈕。
1. 按一下 **[!UICONTROL 傳送證明]** 按鈕以傳送校樣。

   ![](assets/simulate-test-button-email.png){zoomable=&quot;yes&quot;}

1. 選取您的校訂收件者。

   根據訊息通道，校樣可以傳送給下列型別的收件者：

   * 對於簡訊與電子郵件，您可以使用 [測試設定檔](#test-profiles)，即資料庫中的其他特定收件者。 您也可以使用 [從主要目標替代](#substitution-profiles) 模式，將校樣傳送至電子郵件測試地址或電話號碼，並使用現有設定檔的個人化資料。 這可讓您以收件者的方式體驗訊息，讓您精確呈現設定檔將收到的內容。

   * 對於推送訊息，您可以使用 [訂閱者](#subscribers)，即新增至資料庫的虛擬訂閱者。 它們是在下列位置建立的： [!DNL Campaign] 主控台。 進一步瞭解 [Campaign v8 （使用者端主控台）檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}

   每種模式的詳細設定如下。

## 使用測試設定檔 {#test-profiles}

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_mode"
>title="校訂的目標"
>abstract="如果想要在發送到主要目標之前測試您的傳遞，可以上傳第二個檔案做為「校訂的目標」。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_upload"
>title="上傳設定檔"
>abstract="如果想要透過和已經用於主要目標不同的集合測試您的傳遞，則可以上傳包含其他設定檔的第二個檔案。"

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_sample"
>title="範本檔案"
>abstract="檔案格式必須與原始檔案相同。<br/>支援的檔案格式：txt、csv。檔案大小上限：15MB。使用第一行作為欄標題。"

>[!CONTEXTUALHELP]
>id="acw_sms_preview_option_app_target"
>title="將測試設定檔納入主要對象"
>abstract="啟用此選項也可將最終訊息傳送給校訂收件者。"

測試設定檔是資料庫中的其他收件者。 它們是從 **[!UICONTROL 客戶管理]** > **[!UICONTROL 設定檔]** 功能表。 [了解更多](../audience/test-profiles.md#create-test-profiles)

將校樣傳送至測試設定檔的步驟已詳述如下。

1. 從傳送的內容中，按一下 **[!UICONTROL 模擬內容]** 按鈕，以及 **[!UICONTROL 傳送證明]** 按鈕。

1. 從 **[!UICONTROL 模式]** 下拉式清單，選擇 **[!UICONTROL 測試設定檔]** 將目標定位為將接收證明或SMS傳送的虛構收件者。

   ![](assets/simulate-profile-mode.png){zoomable=&quot;yes&quot;}

1. 如果您已選取設定檔至 [預覽訊息](preview-content.md) 在內容模擬畫面中，會預先選取這些設定檔作為校樣收件者。 您可以使用「 」清除選擇和/或新增其他收件者 **[!UICONTROL 新增測試設定檔]** 按鈕。

1. 瀏覽測試設定檔或設定檔清單時，您可以使用篩選器來縮小搜尋範圍。 例如，您可以定義規則以尋找所有具有 **[!UICONTROL 潛在客戶]** 狀態。 瞭解如何使用新增規則 [查詢模型工具](../query/query-modeler-overview.md).

   ![](assets/simulate-test-profile-filter.png){zoomable=&quot;yes&quot;}

1. 若要也傳送最終訊息給證明的收件者，請選取 **[!UICONTROL 在主要目標中包含測試族群]** 選項。

   ![](assets/simulate-include-test.png){zoomable=&quot;yes&quot;}

1. 選取測試設定檔後，您可以 [傳送證明](#send-test).

## 替代設定檔資料 {#substitution-profiles}

使用設定檔替代，將校樣傳送至特定的電子郵件地址或電話號碼，同時顯示來自 [!DNL Adobe Campaign] 資料庫。 只有在已定義傳送的對象時，才能選取此模式。

若要從主要目標取代設定檔資料，請遵循下列步驟：

1. 從傳送的內容中，按一下 **[!UICONTROL 模擬內容]** 按鈕，以及 **[!UICONTROL 傳送證明]** 按鈕。

1. 從 **[!UICONTROL 模式]** 下拉式清單，選擇 **[!UICONTROL 從主要目標替代]** 顯示現有設定檔中的資料時，將校樣傳送至特定電子郵件地址或電話號碼。

   >[!CAUTION]
   >
   >如果您尚未選取 [對象](../audience/about-recipients.md) 對於您的傳遞， **[!UICONTROL 從主要目標替代]** 選項將會呈現灰色，且您將無法選取替代設定檔。

1. 按一下 **[!UICONTROL 新增地址]** 按鈕並指定將接收校樣的電子郵件地址或電話號碼。

   ![](assets/simulate-add-substitution-address.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >您可以輸入任何電子郵件地址或電話號碼。 這可讓您傳送校樣給任何收件者，即使他們不是的使用者 [!DNL Adobe Campaign].

1. 從您為傳送定義的目標中選取設定檔，以用作替代。 您也可以讓 [!DNL Adobe Campaign] 從目標中選取隨機設定檔。 來自所選設定檔的設定檔資料將顯示在校樣中。

1. 確認收件者並重複作業，視需要新增電子郵件地址或電話號碼。

   ![](assets/simulate-profile-substitute.png){zoomable=&quot;yes&quot;}

1. 若要也傳送最終訊息給證明的收件者，請選取 **[!UICONTROL 在主要目標中包含測試族群]** 選項。

1. 選取替代設定檔後，您可以 [傳送證明](#send-test).

## 傳送校樣給應用程式訂閱者 {#subscribers}

使用推播通知進行設計時，校樣只能傳送給應用程式訂閱者。 請依照下列步驟進行選取。

1. 從推播傳送的內容中，按一下 **[!UICONTROL 模擬內容]** 按鈕，以及 **[!UICONTROL 傳送證明]** 按鈕。

   ![](assets/simulate-test-button-push.png){zoomable=&quot;yes&quot;}

1. 如果您已選取訂閱者 [預覽傳遞](preview-content.md) 在內容模擬畫面中，會預先選取這些設定檔為測試訂閱者。

   您可以使用專用按鈕清除您的選擇和/或新增其他訂閱者。

   ![](assets/simulate-test-subscribers.png){zoomable=&quot;yes&quot;}

1. 若要也傳送最終推播通知給測試訂閱者，請選取 **[!UICONTROL 在主要目標中包含測試族群]** 選項。

1. 選取訂閱者後，您可以 [傳送證明](#send-test).

## 傳送證明 {#send-test}

若要將校樣傳送給所選收件者，請遵循下列步驟。

1. 按一下 **[!UICONTROL 傳送證明]** 按鈕。

1. 確認傳送。

   ![](assets/simulate-send-test.png){zoomable=&quot;yes&quot;}

1. 傳送所需數量的校樣，直到您完成傳送內容為止。

完成後，您可以準備並傳送傳遞至主要目標。 請在以下專屬章節中瞭解如何操作：

* [傳送您的電子郵件](../monitor/prepare-send.md)
* [傳送推播通知](../push/send-push.md#send-push)
* [傳送簡訊傳遞](../sms/send-sms.md#send-sms)

## 存取已傳送的校樣 {#access-test-deliveries}

傳送校樣後，您就可以從存取其記錄 **[!UICONTROL 模擬內容]** 畫面。

這些記錄可讓您存取針對所選傳遞傳送的所有校樣，並視覺化與其傳送相關的特定統計資料。 [了解如何監控傳遞記錄](../monitor/delivery-logs.md)

![](assets/simulate-test-log.png){zoomable=&quot;yes&quot;}

您也可以從存取已傳送的校樣 [傳遞清單](../msg/gs-messages.md)，就像任何傳送一樣。

![](assets/simulate-deliveries-list.png){zoomable=&quot;yes&quot;}
