---
title: 在Adobe Campaign中使用GenStudio for Performance Marketing
description: 瞭解如何在Adobe Campaign中使用GenStudio for Performance Marketing
feature: Email Design
topic: Content Management, Artificial Intelligence
role: User
level: Beginner, Intermediate
exl-id: c22a44a8-e4e2-453a-9ca2-b80f7c0edc19
source-git-commit: 61e6dcf13fc6a405f5e25328bf336e863701b2fe
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 7%

---

# 使用 GenStudio for Performance Marketing {#genstudio}

>[!CONTEXTUALHELP]
>id="ac_genstudio_button"
>title="使用以 GenStudio 建置的範本"
>abstract="由於與 Adobe GenStudio for Performance Marketing 緊密整合，您可以輕鬆匯入透過 Adobe AI 技術增強的 GenStudio 範本。"

## 開始使用GenStudio {#gs-genstudio}

[Adobe GenStudio for Performance Marketing](https://experienceleague.adobe.com/zh-hant/docs/genstudio-for-performance-marketing/user-guide/home){target="_blank"}是創作AI優先的應用程式，可讓行銷團隊建立自己的廣告和電子郵件，以推動具影響力、個人化的行銷活動，符合您的品牌標準並遵守您的企業政策。 透過運用Adobe AI技術，提供一套完整的工具，可簡化內容建立及管理的複雜性，讓創意人員可專注在創新上。

>[!AVAILABILITY]
>
>此功能僅適用於電子郵件頻道。

若要提升行銷效率並維持品牌一致性，您可以將&#x200B;[!DNL **GenStudio for Performance Marketing**]&#x200B;體驗與&#x200B;[!DNL **Adobe Campaign**]&#x200B;緊密整合。 這可讓您運用[!DNL GenStudio]的AI支援內容建立以及[!DNL Adobe Campaign]的進階協調功能。

>[!INFO]
>
>若要更進一步，請檢視此[總覽](https://business.adobe.com/tw/products/genstudio-for-performance-marketing.html#watch-overview){target="_blank"}以及[的](https://business.adobe.com/tw/products/genstudio-for-performance-marketing.html#demo){target="_blank"}示範[!DNL Adobe GenStudio for Performance Marketing]。

## 在Adobe Campaign中使用GenStudio功能 {#use-genstudio}

[!DNL GenStudio for Performance Marketing]與[!DNL Adobe Campaign]整合可讓您公司的行銷人員更有效地合作，以簡化程式。

例如，使用[!DNL Adobe Campaign]開發和自動化電子郵件行銷活動的技術行銷人員，可以與使用[!DNL GenStudio]建立內容的效能行銷人員共同作業。

透過這項整合，兩者可以共同作業，輕鬆地將[!DNL GenStudio]中的品牌上內容整合到[!DNL Adobe Campaign]中，傳遞吸引人的電子郵件，以鎖定特定客戶細分並提升銷售量。

### 將HTML範本從Adobe Campaign匯出至GenStudio {#export-from-campaign-to-genstudio}

首先，您可以將包含品牌指引的[!DNL Adobe Campaign] HTML範本匯出至[!DNL GenStudio for Performance Marketing]。 請遵循下列步驟。

1. 在[!DNL Adobe Campaign]中，存取您電子郵件的內容。 [了解做法](../email/create-email.md#create-content)

1. 在電子郵件Designer中，從&#x200B;**[!UICONTROL 更多]**&#x200B;按鈕中選取&#x200B;**[!UICONTROL 匯出HTML]**。

   ![](assets/genstudio-export-template.png){zoomable="yes"}

1. 將此HTML匯出的範本上傳至[!DNL GenStudio for Performance Marketing]。<!--Make sure you detect the fields that the generative AI uses to insert content in order to create an actionable template.-->

   >[!NOTE]
   >
   >在[!DNL GenStudio]HTML使用手冊[專屬區段中，瞭解如何將Adobe GenStudio for Performance Marketing範本上傳至](https://experienceleague.adobe.com/zh-hant/docs/genstudio-for-performance-marketing/user-guide/content/templates/use-templates#templates-from-ajo-and-marketo){target="_blank"}。<!--GenStudio doc to be updated with Campaign-->

1. 在GenStudio中，使用此範本建立具有AI提示的多個電子郵件變體並儲存。

   >[!NOTE]
   >
   >瞭解如何在GenStudio專屬的[區段](https://experienceleague.adobe.com/zh-hant/docs/genstudio-for-performance-marketing/user-guide/create/create-email-experience){target="_blank"}中建立電子郵件體驗。

### 在Adobe Campaign中善用GenStudio體驗 {#leverage-genstudio-experiences}

若要運用您剛才建立的[!DNL GenStudio]電子郵件變數（透過將其匯入[!DNL Adobe Campaign]中），請遵循下列步驟。

1. 在[!DNL Adobe Campaign]中，[建立電子郵件傳遞](../email/create-email.md)。

1. 在電子郵件傳遞控制面板中，按一下&#x200B;**[!UICONTROL 編輯內容]**&#x200B;按鈕。 [了解更多](../email/create-email.md#create-content)

1. 在電子郵件Designer首頁上，選取&#x200B;**[!UICONTROL 匯入HTML]**，然後按一下&#x200B;**[!UICONTROL Adobe GenStudio for Performance Marketing]**&#x200B;按鈕。

   ![](assets/genstudio-pem-import-email.png){zoomable="yes"}

1. 瀏覽GenStudio體驗以開始建立您的內容。 您可以根據數個條件篩選體驗，例如產品、角色、品牌或甚至顏色。

   <!--![](assets/genstudio-filter-experiences.png){zoomable="yes"}-->

1. 選取體驗並按一下&#x200B;**[!UICONTROL 使用]**。

   ![](assets/genstudio-use-experience.png){zoomable="yes"}

1. 選取您要匯入GenStudio體驗的資料夾。

   ![](assets/genstudio-choose-destination.png){zoomable="yes"}

1. 選取的內容會顯示在電子郵件Designer中。

   ![](assets/genstudio-email-content.png){zoomable="yes"}

   >[!NOTE]
   >
   >從[範本 [!DNL Adobe Campaign] 建立的GenStudio體驗](#export-from-ajo-to-genstudio)會直接匯入電子郵件Designer。 未使用[!DNL Adobe Campaign]範本建立的GenStudio體驗已匯入至[相容性模式](../email/existing-content.md)。

   使用[電子郵件內容編輯工具](../email/create-email-content.md)和[個人化欄位](../personalization/personalize.md)，依需要編輯您的電子郵件。 儲存您的內容。

<!--Detail a use case with A/B testing to import other GenStudio variations and track how your tratments are performing.-->


<!--
## How-to video {#video}

Discover the process of exporting an email template from Adobe Campaign to GenStudio for Performance Marketing, crafting brand-compliant emails using the template in GenStudio, and importing them seamlessly back into Adobe Campaign.

>[!VIDEO](https://video.tv.adobe.com/v/3456060/?captions=chi_hant&quality=12)
TO REPLACE WITH CAMPAIGN VIDEO WHEN/IF RELEASED
-->