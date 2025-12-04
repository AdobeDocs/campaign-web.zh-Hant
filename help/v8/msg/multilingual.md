---
audience: end-user
title: 設定多語言傳遞
description: 瞭解如何設定多語言傳送
source-git-commit: 50a798abea166e89d58e8e46eb55590333071ef0
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 7%

---

# 設定多語言傳遞 {#multilingual-delivery}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_multilingual"
>title="新增語言"
>abstract="在此索引標籤中，您將找到要用來傳遞內容的語言清單。您可以按一下「新增語言」按鈕，或透過此索引標籤複製其他語言來新增更多語言。"

>[!CONTEXTUALHELP]
>id="acw_multilingual_file_upload"
>title="匯入語言變體"
>abstract="使用此對話方塊可透過匯入CSV檔案來新增語言變體。 檔案會自動填入所選語言的所有可用欄位。 您可以拖放檔案，或在確認之前從電腦中選擇檔案。"

在Campaign Web UI中，您可以將傳送設定為多語言，這可讓您根據設定檔的偏好語言傳送訊息。 未定義偏好設定時，訊息會以預設語言傳送。

在多語言傳遞中，語言管理會根據變體。 每個變體代表一種語言。 在建立傳遞期間，您可以新增多種語言變體，以符合訊息中所需語言的數量。 您也可以在新增這些變體後，隨時變更預設語言。

多語言功能目前可用於電子郵件、推播通知、異動訊息和簡訊。

>[!AVAILABILITY]
>
>多語言推播通知、交易式訊息和簡訊僅供一組組織使用（可用性限制），並將在未來版本中全域推出。 您的伺服器必須升級至8.8.2或更新版本。

若要設定多語言傳送，請遵循下列主要步驟：

1. 新增語言變體，[瞭解詳情](#add-variant)
1. 定義每個變體的內容，[瞭解詳情](#define-content)
1. 管理語言變體，[瞭解詳情](#manage-variant)

## 新增語言變體{#add-variant}

若要建立語言變體，請依照下列步驟進行：

1. 在傳遞儀表板中，按一下鉛筆圖示以存取傳遞內容版本畫面，然後按一下&#x200B;**[!UICONTROL 新增語言]**。

   >[!IMPORTANT]
   >
   >**[!UICONTROL 新增語言]**&#x200B;按鈕只有在目標維度包含&#x200B;**語言**&#x200B;結構描述時才可用。 若要進一步瞭解結構描述和目標維度，請參閱[詳細檔案](../audience/targeting-dimensions.md)。

   ![](assets/edit-content_2.png){zoomable="yes"}

1. 從&#x200B;**新增語言**&#x200B;下拉式清單中，選取要新增的語言，然後確認。

   您新增的第一個語言會自動設定為預設語言，而現有內容會成為預設版本。 新增其他語言時，其內容最初會從預設語言複製。

   ![](assets/edit-content_3.png){zoomable="yes"}

   >[!NOTE]
   >
   >透過此清單可用的語言取決於&#x200B;**語言**&#x200B;屬性所定義的值（例如：system、user、dbenum等值）。 在此[區段](../administration/enumerations.md)中進一步瞭解列舉管理。

1. 重複此作業以新增其他語言。 左側的&#x200B;**[!UICONTROL 語言]**&#x200B;面板會顯示您已選擇的語言清單、語言數目和預設語言。

   例如，如果您已選擇英文、法文和瑞典文，您可以看到下列3種語言：

   ![](assets/edit-content_9.png){zoomable="yes"}

   若要瞭解如何管理語言變體，請參閱此[區段](#manage-variant)。

## 定義每個變體的內容{#define-content}

語言設定完成後，請針對每種語言定義傳送內容。

1. 在傳遞內容版本畫面中，從左側的&#x200B;**[!UICONTROL 語言]**&#x200B;面板選取語言。

   ![](assets/edit-content_11.png){zoomable="yes"}

1. 為此語言定義訊息的內容。 在此[節](../msg/create-deliveries.md)中瞭解更多。

1. 針對每種語言重複此作業。

<!--
>[!BEGINTABS]

>[!TAB Email delivery]

1. From the delivery content edition screen, choose a language and click the **[!UICONTROL Edit email body]** button. You can also hover over the email preview and select **[!UICONTROL Open email designer]**.

    ![](assets/edit-content_11.png){zoomable="yes"}

1. Define the content of your email for this language. [Read more](../email/get-started-email-designer.md#start-authoring)

1. Repeat this operation for each language.

>[!TAB SMS delivery]

1. From the delivery content edition screen, choose a language.

1. Edit the content of the SMS message for this language. [Read more](../sms/create-sms.md)

    ![](assets/edit-content_11-sms.png){zoomable="yes"}

1. Repeat this operation for each language.

>[!ENDTABS]

-->

若要預覽傳遞，請按一下&#x200B;**[!UICONTROL 模擬內容]**&#x200B;按鈕，然後選擇設定檔。 確保為每個設定檔顯示正確的內容。

![](assets/edit-content_5.png){zoomable="yes"}

## 管理語言變體{#manage-variant}

在左側面板中，會顯示所有語言變體資訊。 若要刪除所有語言，請按一下展開按鈕，然後按一下&#x200B;**[!UICONTROL 刪除所有變體]**。

![](assets/edit-content_13.png){zoomable="yes"}

在語言變體清單中，您可以執行下列動作：

* **編輯**：在保留關聯內容的同時變更語言。
* **設定為預設值**：將語言設定為預設語言。 當設定檔未定義語言時，訊息會以預設語言傳送。
* **複製**：複製針對此語言定義的內容，並選擇不同的變體。
* **刪除**：刪除變體及其相關內容。

![](assets/edit-content_13-sms.png){zoomable="yes"}

