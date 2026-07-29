---
audience: end-user
title: 檢閱優惠方案環境設定
description: 瞭解如何在Campaign Web中檢視、設定和部署優惠方案環境
feature: Offers
product_v2: id: dfc56824-e8b9-499e-85d4-21aedb507314
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 7be45366e3ae14e6fa7e4569a37c64e6d72f534c
workflow-type: tm+mt
source-wordcount: 319
ht-degree: 2%

---

# 檢閱優惠方案環境設定 {#offer-environment}

**優惠方案環境**&#x200B;是您用來組織優惠方案目錄和相關優惠方案空間的容器。 有兩種型別的環境：

* **設計**&#x200B;環境，在此環境中可建立、設定和核准優惠方案，
* 唯讀&#x200B;**即時**&#x200B;環境，已核准和已部署的優惠方案可供傳遞選擇。

每個&#x200B;**設計**&#x200B;環境都連結到&#x200B;**即時**&#x200B;環境。 當優惠方案完成並核准後，就會自動部署至&#x200B;**即時**&#x200B;環境並可供傳送。

![顯示環境的熒幕擷圖。](assets/offers-env.png){zoomable="yes"}

根據預設，Campaign提供兩個&#x200B;**設計**&#x200B;和&#x200B;**即時**&#x200B;環境，預先設定以鎖定內建的收件者表格（已識別的優惠）。

若要鎖定其他表格（例如造訪您網站進行傳入互動的匿名設定檔），您需要建立其他環境（每個目標維度一個環境）。 請參閱[Campaign v8檔案](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/offers/interaction-settings/interaction-env#create-an-offer-environment){target="_blank"}。

## 存取選件環境 {#offer-environment-settings}

選件環境會儲存為資料夾。 若要存取及檢閱環境設定（資格、重量管理、安全性），請遵循下列步驟：

>[!CAUTION]
>
>這些設定可以修改，但您應非常小心，因為變更可能會破壞現有的實作。

1. 從左側導覽功能表，開啟&#x200B;**[!UICONTROL Explorer]**，並在&#x200B;**設計環境**&#x200B;節點下找到選件環境資料夾。

1. 按一下……按鈕，然後選取&#x200B;**[!UICONTROL 資料夾設定]**&#x200B;以顯示環境設定。

   ![熒幕擷圖顯示環境的[資料夾設定]選項](assets/offers-env-1.png){zoomable="yes"}

1. 檢閱不同的區段。 優惠方案環境群組優惠方案特定選項的資料夾設定。

   ![熒幕擷圖顯示環境的屬性設定](assets/offers-env-2.png){zoomable="yes"}

   大部分的設定都反映使用者端主控台中可用的選件環境設定。 如需詳細資訊，請參閱 [Campaign v8 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-env.html){target="_blank"}。

<!--
## Create a new offer environment {#create}

If you need to manage a separate offer catalog — for example, for a different targeting dimension — you can create a new **Design** environment directly from the Web UI.

1. From the left navigation menu, open the **[!UICONTROL Explorer]** and locate the **Offers - design** folder.

1. Create a new folder from this location, then open its properties and fill in the environment-specific settings described below.

The **[!UICONTROL Linked live environment]** field is set automatically when the environment is created — see [Type of environment](#type).

## Access the offer environment settings {#access}

Offer environments are stored as folders. To access an environment and modify its properties, follow these steps. 

1. From the left navigation menu, open the **[!UICONTROL Explorer]** and locate the offer environment folder under the **Design environment** node.

1. Click on the ... button, and select **[!UICONTROL Folder settings]** to display the environment settings.

  ![Screenshot showing the Folder settings option of an environment](assets/offers-env-1.png){zoomable="yes"}

The folder settings of an offer environment group offer-specific options into several sections. 

-->
<!-- 
Most settings mirror the offer environment configuration available in the Adobe Campaign client console.
-->
<!-- 

## Properties {#properties}

This section is common to all folders. It allows you to define the **Label** of the folder and modify the technical folder properties.  

![Screenshot showing the Properties settings of an environment](assets/offers-env-2.png){zoomable="yes"}

-->
<!--

* **[!UICONTROL Label]** — Display name of the environment.


Expand **[!UICONTROL Additional options]** to access the technical properties of the folder:

* **[!UICONTROL Internal name]** — Unique identifier of the folder. Used to reference the environment from schemas, workflows, and API calls. The internal name is set at creation and should not be changed afterwards.

* **[!UICONTROL Full name]** — Read-only path of the folder in the Explorer tree (for example, `/Offers - design/Environment - Recipient/`).

* **[!UICONTROL Template]** — Read-only name of the folder template the environment is based on (for example, **[!DNL nmsOfferEnv]** for an offer environment).

* **[!UICONTROL Created by]** / **[!UICONTROL Modified by]** — Audit fields populated automatically with the operator that created and last modified the folder.

This section gathers the offer-specific settings of the folder.

-->
<!--

## Environment {#env-section}

  ![Screenshot showing the Environment settings of an environment](assets/offers-env-3.png){zoomable="yes"}

### Type of environment {#type}

* **[!UICONTROL Type of environment]** — Switches the folder between **[!UICONTROL Design]** and **[!UICONTROL Live]**. The type is set when the environment is created. Changing it later is not recommended.

 **[!UICONTROL Linked live environment]** — Displays the read-only **[!UICONTROL Live]** environment that receives the deployed offers. Set automatically when the environment is created.

### Execution instances {#execution-instances}

* **[!UICONTROL Display execution instances]** — Opens the list of execution instances mapped to the environment. This section is only displayed when the multi-instance execution option is activated. Refer to the [Campaign v8 documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-architecture.html#distributed-architecture){target="_blank"}.

### Targets of this environment {#targets}

  ![Screenshot showing the other Environment settings of an environment](assets/offers-env-4.png){zoomable="yes"}

* **[!UICONTROL Environment dedicated to incoming anonymous interactions]** — Activates anonymous interaction features on the environment. This relies on a target mapping for the visitor targeting dimension, which you can now create directly from the Web UI — see [Manage target mappings](../administration/target-mappings.md). Refer to the [Campaign v8 documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-env.html#create-an-offer-environment){target="_blank"} for the full anonymous interaction setup.

-->
<!--
and [Anonymous interactions](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/anonymous-interactions.html){target="_blank"}.
-->
<!--

* **[!UICONTROL Targeting dimension]** — Schema and table of the contacts targeted by the offers contained in this environment (for example, **[!DNL Recipients (nms:recipient)]**). The targeting dimension is reused by every offer and offer space of the environment.

### Storage of generated propositions {#storage}

* **[!UICONTROL Storage dimension]** — Schema and table where the propositions generated through this environment are stored (for example, **[!DNL Recipient offer propositions (nms:propositionRcp)]**).

* **[!UICONTROL Call data schema]** — Schema used to capture the data of each call to the Offer engine (for example, **[!DNL Interactions (nms:interaction)]**). For details on this schema, refer to the [Campaign v8 data model documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/dev/datamodel.html){target="_blank"}.

### Implicit identification (if the function is enabled in the space) {#implicit-identification}

* **[!UICONTROL Target mapping]** — Used to configure the **changeover process**, which lets the Offer engine switch between an identified and an anonymous environment depending on whether the contact can be identified during an inbound interaction. Leave this field empty when implicit identification is not used. Learn how to create and manage target mappings directly from the Web UI in [Manage target mappings](../administration/target-mappings.md). For the offer-specific changeover process configuration, refer to [Campaign v8 documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/anonymous-interactions.html){target="_blank"}.

-->
<!--
## Eligibility {#eligibility}

  ![Screenshot showing the other Environment settings of an environment](assets/offers-env-5.png){zoomable="yes"}

* **[!UICONTROL Presentation typology]** — Typology rule of type **[!UICONTROL Offer presentation]** referenced by the environment. Presentation typologies exclude offers based on the proposition history of a recipient. You can edit these rules directly from the Web UI's **[!UICONTROL Business rules]** screen — see [Work with business rules (typologies)](../administration/typologies.md). Refer to the [Campaign v8 documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-offer.html#offer-presentation){target="_blank"} for the full rule reference.

* **[!UICONTROL Filters on the target]** — Filter rules that apply to every offer in the environment. Use **[!UICONTROL Add rules]** to open the rule builder and restrict the audience targeted by all offers contained in this environment.

## Offer weight {#offer-weight}

* **[!UICONTROL Display offer weight]** — Click the **Display offer weight** button to open the read-only list of offer weights included in the environment folder. Weights themselves are configured at the offer space and the offer levels — refer to [Create and publish an offer](create-offer.md#eligibility).

## Security settings and Restrictions {#security}

These two sections are generic Campaign folder controls. They are not specific to offer management.

* **[!UICONTROL Security settings]** — The **[!UICONTROL Group or operator]** table defines the operators and operator groups allowed to read, write, or delete the environment and its contents. For Interaction-specific operator roles (Offer manager, Delivery manager), refer to [Operators of the Interaction module](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-operators.html){target="_blank"}.

* **[!UICONTROL System folder]** — When enabled, marks the folder as a system folder.

* **[!UICONTROL Restrictions]** — Lets you turn the folder into a view by enabling **[!UICONTROL This folder is a view]** and clicking **[!UICONTROL Edit restrictions]** to define a filter on the records displayed in the folder.
-->
接著，[建立優惠方案空間](offer-space.md)以定義優惠方案的公開位置和方式。
