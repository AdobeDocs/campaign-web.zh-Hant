---
audience: end-user
title: 使用商業規則（型別）
description: 瞭解如何使用型別和型別規則來控制、篩選及監控傳送的傳送。
exl-id: 54fdd03a-e49d-4f22-b6d4-6055c8922e58
source-git-commit: 1f3f3afb9b21ab37aeea73057d832cea172c00bf
workflow-type: tm+mt
source-wordcount: '1449'
ht-degree: 22%

---

# 使用商業規則（型別） {#typologies}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="業務規則"
>abstract="您現在可以在Adobe Campaign網頁使用者介面中建立型別與型別規則。 型別可讓您控制、篩選傳遞內容，並設定其優先順序。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=zh-hant" text="請參閱版本注意事項"


>[!CONTEXTUALHELP]
>id="acw_business_rules"
>title="類型和類型規則"
>abstract="您可以利用類型將所有傳遞的業務實務標準化。類型是類型規則的集合，可讓您控制、篩選傳遞的傳送並排定其優先順序。在準備階段，與類型規則中的標準相符的輪廓會排除在傳遞對象之外。"

## 關於型別

您可以利用類型將所有傳遞的業務實務標準化。**型別**&#x200B;是&#x200B;**型別規則**&#x200B;的集合，可讓您控制、篩選傳遞內容，並排定其優先順序。 在準備階段，與類型規則中的標準相符的輪廓會排除在傳遞對象之外。

型別可確保您的傳送一律包含特定元素（例如取消訂閱連結或主旨列）或篩選規則，以從您的預期目標（例如取消訂閱者、競爭者或不忠誠客戶）中排除群組。

可透過&#x200B;**[!UICONTROL 管理]** > **[!UICONTROL 商業規則]**&#x200B;功能表存取型別。 您可以從此畫面存取所有現有的型別與型別規則，或根據您的需求建立新型別與型別規則。

![](assets/business-rules-list.png)

>[!NOTE]
>
>**[!UICONTROL 型別規則]**&#x200B;清單會顯示目前在Web使用者介面或使用者端主控台中建立的所有現有規則。 不過，在Web使用者介面中只能建立&#x200B;**控制**&#x200B;和&#x200B;**篩選**&#x200B;規則。 若要建立其他型別的型別規則，例如壓力或容量規則，請使用Campaign v8使用者端主控台。 [瞭解如何在使用者端主控台中建立型別規則](https://experienceleague.adobe.com/en/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"}

將型別套用至訊息的主要步驟如下：

1. [建立型別](#typology)。
1. [建立型別規則](#typology-rules)。
1. [在型別](#add-rules)中參考型別規則。
1. [套用型別至訊息](#message)。

## 建立類型 {#typology}

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_properties"
>title="類型屬性"
>abstract="定義類型的屬性並展開「**[!UICONTROL 附加選項]**」區段，以存取進階設定。使用「**[!UICONTROL IP 親和原則]**」欄位，使 IP 親和原則與類型相關聯。透過定義每個親和原則可使用哪些特定的 IP 位址，便可以更好地控制傳出 SMTP 流量。"

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_ip_affinity"
>title="IP 親和原則"
>abstract="管理與 IP 位址的相似性可讓您根據傳遞動作的類型，將不同的 IP 位址與每種類型的流量相關聯，從而更好地控制傳出 SMTP 流量。"

若要建立型別，請遵循下列步驟：

1. 導覽至&#x200B;**[!UICONTROL 商業規則]**&#x200B;功能表，然後選取&#x200B;**[!UICONTROL 型別]**&#x200B;標籤。

1. 按一下&#x200B;**[!UICONTROL 建立型別]**&#x200B;按鈕，然後輸入型別的&#x200B;**[!UICONTROL 標籤]**。

1. 展開&#x200B;**[!UICONTROL 其他選項]**&#x200B;區段以定義進階設定，例如型別的內部名稱、儲存資料夾和說明。

   ![](assets/business-rules-typology.png)

   >[!NOTE]
   >
   >**[!UICONTROL IP相關性]**&#x200B;欄位可讓您將IP相關性與型別建立關聯。 這可讓您定義哪些特定IP位址可用於每個相似性，藉此更好地控制傳出SMTP流量。  例如，您可以對每個國家或子網域使用一個相似性。 接著，您可以為每個國家/地區建立一個型別，並將每個相似性連結至對應的型別。

1. 按一下&#x200B;**[!UICONTROL 「建立]**」以確認型別建立。

型別會開啟詳細資訊。 在此畫面中，您可以直接參考現有的型別規則。 您也可以建立新的型別規則，並於稍後在型別中參考這些規則：
* [瞭解如何建立型別規則](#add-rules)
* [瞭解如何在型別中參考規則](#add-rules)

## 建立類型規則 {#typology-rule}

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_properties"
>title="類型規則屬性"
>abstract="定義類型規則的屬性。**控制**&#x200B;規則在傳送前驗證訊息品質和有效性，而&#x200B;**篩選**&#x200B;規則會根據特定標準排除目標對象的區段。<br/><br/>當屬於相同類型的數個規則在同一個訊息處理階段執行時，您也可以變更此規則的執行順序，以管理執行類型規則的順序。"

若要建立型別規則，請導覽至&#x200B;**[!UICONTROL 商業規則]**&#x200B;功能表，然後選取&#x200B;**[!UICONTROL 型別規則]**&#x200B;標籤。

按一下&#x200B;**[!UICONTROL 建立型別規則]**&#x200B;按鈕，然後遵循以下詳細步驟。

### 定義型別規則的屬性 {#properties}

定義型別規則的屬性：

1. 輸入規則的&#x200B;**[!UICONTROL 標籤]**。

   ![](assets/business-rules-control-rule.png)

1. 選取型別規則的&#x200B;**[!UICONTROL 型別]**：

   * **控制項**：確保訊息品質和預先傳送的有效性（例如字元顯示、簡訊長度、位址格式、URL縮短）。 它們使用指令碼介面來建立，以定義內容檢查和修改的複雜邏輯。

   * **篩選**&#x200B;規則根據特定標準 (例如年齡、地點、國家、電話號碼) 排除目標對象區段。這些規則會連結至目標維度。

   >[!NOTE]
   >
   >目前，只能從Web使用者介面建立&#x200B;**控制**&#x200B;和&#x200B;**篩選**&#x200B;型別規則。 若要建立其他型別的規則，請使用使用者端主控台。 [瞭解如何在使用者端主控台中建立型別規則](https://experienceleague.adobe.com/en/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"}

1. 選取要與規則關聯的&#x200B;**[!UICONTROL 管道]**。

1. 如果您不希望規則在建立後立即啟用，請將&#x200B;**[!UICONTROL 啟用]**&#x200B;選項切換為關閉。

1. 定義規則&#x200B;**[!UICONTROL 執行順序]**。

   依預設，型別規則順序設為50。 您可以調整此值，來管理在同一訊息處理階段執行相同型別的數個規則時，型別規則的執行順序。 例如，執行順序為20的篩選規則會在執行順序為30的篩選規則之前執行。

1. 展開&#x200B;**[!UICONTROL 其他選項]**&#x200B;區段以存取進階設定，例如規則的內部名稱、資料夾儲存和說明。

1. 對於控制規則，其他選項中還提供兩個其他規則。 它們可讓您指定何時應套用規則及其警示等級：

   * **[!UICONTROL 階段]**：此欄位可讓您指定在傳遞生命週期的哪個時間點套用規則。 選取要在&#x200B;**[!UICONTROL 階段]**&#x200B;下拉式清單中套用的值。 展開下方的區段，以取得可能值的詳細資訊。

   +++控制規則階段：

   **[!UICONTROL 在鎖定目標開始時]**：若要防止發生錯誤時執行個人化步驟，您可以在此處套用控制規則。

   **[!UICONTROL 鎖定目標之後]**：如果您需要知道目標的磁碟區以套用控制規則，請選取此階段。 例如，檢查校樣大小控制規則適用於每個目標定位階段之後：如果校樣收件者過多，此規則會防止訊息個人化。

   **[!UICONTROL 在個人化開始時]**：如果控制項涉及核准訊息個人化，則必須選取此階段。 訊息個人化會在分析階段中執行。

   **[!UICONTROL 在分析結束時]**：當檢查需要完成訊息個人化時，請選取此階段。

+++

   * **[!UICONTROL 層級]**：此選項可讓您指定規則的警示層級。 展開以下區段以取得詳細資訊。

   +++控制規則層次：

   **[!UICONTROL 錯誤]**：停止訊息準備。

   **[!UICONTROL 警告]**：在準備記錄檔中顯示警告。

   **[!UICONTROL 資訊]**：在準備記錄檔中顯示資訊。

   <!--**[!UICONTROL Status]**:-->

   **[!UICONTROL 詳細資訊]**：顯示伺服器記錄檔中的資訊。

+++

### 建置規則內容 {#build}

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_filtering"
>title="篩選"
>abstract="**篩選**&#x200B;規則根據特定標準 (例如年齡、地點、國家、電話號碼) 排除目標對象區段。選取類型規則的目標維度，然後按一下「**[!UICONTROL 新增規則]**」按鈕以存取查詢建模工具並建置規則。"

>[!CONTEXTUALHELP]
>id="acw_business_rules_typology_rules_code"
>title="程式碼"
>abstract="**控制**&#x200B;規則在傳送前驗證訊息品質和有效性 (例如字元顯示、SMS 長度、地址格式、URL 縮短)。它們是使用 JavaScript 程式碼建立的。"

定義型別規則的屬性後，您就可以建置規則的內容。

* 針對&#x200B;**控制項規則**，按一下&#x200B;**編輯程式碼**&#x200B;按鈕，然後使用JavaScript輸入規則的邏輯。 在以下範例中，我們將建立一個規則，如果目標為空，則會在紀錄中顯示警告。

  ![](assets/business-rules-code.png)

* 針對&#x200B;**篩選規則**，請選取目標維度，然後按一下&#x200B;**[!UICONTROL 新增規則]**&#x200B;按鈕，以使用[查詢模型工具](../query/query-modeler-overview.md)定義篩選條件。

  ![](assets/business-rules-query.png)

當您的規則準備就緒時，按一下&#x200B;**[!UICONTROL 建立]**&#x200B;按鈕以建立型別規則。 您現在可以在型別中參考規則，以將其套用至訊息。

## 在型別中參考型別規則 {#add-rules}

若要在型別中參照一或多個規則，請遵循下列步驟：

1. 導覽至&#x200B;**[!UICONTROL 型別]**&#x200B;標籤，並開啟您要參考規則的型別。

1. 選取&#x200B;**[!UICONTROL 型別規則]**&#x200B;索引標籤，然後按一下&#x200B;**[!UICONTROL 新增型別規則]**&#x200B;按鈕。

   ![](assets/business-rules-reference.png)

1. 選取一或多個要與型別產生關聯的型別規則，並加以確認。

   ![](assets/business-rules-typology-save.png)

1. 按一下「**[!UICONTROL 儲存]**」。

您現在可以將型別套用至訊息。 完成後，將執行所有選取的型別規則以執行定義的檢查。

## 套用型別至訊息 {#message}

若要將型別套用至訊息或訊息範本，您必須在訊息設定中選取型別。 [瞭解如何設定傳遞設定](../advanced-settings/delivery-settings.md#typology)

![](assets/business-rules-apply.png)

完成後，將執行型別中包含的型別規則，以在訊息準備期間檢查傳遞是否有效。 然後，符合型別規則中之條件的設定檔會從傳送對象中排除。
