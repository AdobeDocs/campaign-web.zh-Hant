---
audience: end-user
title: 開始使用 Adobe Campaign Web
description: 開始使用 Adobe Campaign Web
exl-id: 885d7851-4e5d-4b03-ba6f-71f90ede83e8
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: ht
source-wordcount: '566'
ht-degree: 100%

---

# 開始使用 Adobe Campaign Web {#get-started}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_learnmore"
>title="開始使用"
>abstract="新的 Adobe Campaign Web 介面提供了整合、直覺和一致性的使用者體驗。"

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_learnmore"
>title="開始使用"
>abstract="新的 Adobe Campaign Web 介面提供了整合、直覺和一致性的使用者體驗。"

>[!CONTEXTUALHELP]
>id="acw_homepage_learnmore"
>title="開始使用"
>abstract="新的 Adobe Campaign Web 介面提供了整合、直覺和一致性的使用者體驗。"

Adobe Campaign 提供跨管道客戶體驗設計的平台，也提供進行視覺化行銷活動協調、Real-time Interaction Management 以及 Cross-channel Execution 的環境。

Adobe Campaign v8 是專為電子郵件、推播、簡訊和直接郵件等各種行銷管道打造的新一代行銷活動工具。其提供強大的 ETL 和資料管理功能，協助製作和策畫完美的行銷活動。其協調流程引擎能落實豐富的多點接觸行銷方案，並以批次主導的歷程為重點。此工具還包括可擴充的即時傳送訊息伺服器，讓行銷團隊能夠根據來自任何 IT 系統的全面性承載傳送預先定義的訊息，進行如密碼重設、訂單確認、電子收據等通訊。

使用 Campaign 可以：

* 透過單一可存取的客戶視圖，**推動**&#x200B;個人化和參與度。
* 將電子郵件、行動裝置、線上和離線管道&#x200B;**整合**&#x200B;至客戶歷程中。
* 將有意義之即時訊息和優惠方案的傳遞&#x200B;**自動化**。

## 探索 Campaign Web 使用者介面 {#web}

最初只能透過擁有豐富功能的[用戶端主控台](#ac-client)使用的 Campaign，現在提供新的 Web 使用者介面 (UI)，易用性和可及性更高，而且採用全新設計，能大幅提升使用者體驗。這個現代的使用者介面簡化行銷活動的設計和傳遞過程，並與其他 Adobe 解決方案 (包括 Adobe Experience Platform) 介面保持一致性。

![顯示 Adobe Campaign Web 使用者介面首頁畫面的螢幕擷圖](assets/home.png){zoomable="yes"}

這個新的 Web 使用者介面主要是為了滿足&#x200B;**商務從業人員**&#x200B;的需求。在此初始版本中無法進行一般的管理工作，但在後續版本中會解決這個問題。請注意，用戶端主控台中可使用的功能或選項，目前並非每項皆可在新的使用者介面中存取。新的使用案例、選項和功能將在未來的版本中引入。

做為管理員或專家使用者，如果您需要存取未在 Campaign Web 使用者介面中提供的 Campaign v8 功能，請連線至[用戶端主控台](#ac-client)。

在[此頁面](connect-to-campaign.md)中了解如何連線至 Adobe Campaign Web。

➡️ [在影片中探索 Campaign Web](#video)

## 關於 Campaign 用戶端主控台 {#ac-client}

此用戶端主控台是專為管理員和進階使用者所設計，用於執行其任務。Campaign 用戶端主控台是安裝在您的系統上並以瀏覽器為基礎的應用程式。其使用 Web 服務 API 連接至您的 Campaign 應用程式伺服器。

Campaign 資料儲存在應用程式伺服器中。從用戶端主控台以及 Campaign Web 使用者介面皆可存取資料。例如，若您使用用戶端主控台建立傳遞範本，則該範本也可以在 Campaign Web 使用者介面中使用。同樣地，若您在 Campaign Web 使用者介面中建立電子郵件傳遞，也可以從用戶端主控台存取此傳遞。

某些物件只能在用戶端主控台中建立和管理。您可以在 Campaign Web 使用者介面中看到並使用這些物件，但不能在這個環境中建立或修改物件。所有的 Campaign 物件和元件都能透過探索工具使用，並且從左側導覽存取。

如需關於如何透過其用戶端主控台使用 Campaign v8 的詳細資訊，請參閱 [Campaign v8 (用戶端主控台) 文件](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaign-home.html?lang=zh-Hant){target="_blank"}。

<!--
## How-to video {#video}

Learn how to access and navigate the Campaign Web user interface and how to customize the inventory lists. Discover the AI-powered Knowledge Assistant.

>[!VIDEO](https://video.tv.adobe.com/v/3453433?quality=12&captions=chi_hant)
-->

<!--
## Get started for marketers and administrators

>[!BEGINTABS]

>[!TAB Get started for Marketers]

**Discover the interface**

The new Adobe Campaign Web interface offers a modern and intuitive user experience to simplify marketing campaign design and delivery. Learn more in this section. [Learn more](user-interface.md)

**Use plans, programs, campaigns**

Adobe Campaign allows you to easily orchestrate your targeted marketing initiatives, using the built-in campaign management capability. With the ability to define a schedule, you can plan the duration and timing of your campaigns to align with strategic objectives and maximize audience engagement. [Learn more](../campaigns/gs-campaigns.md)

**Create and manage profiles and audiences**

A profile is a record stored in the database, serving as a key component to create audiences for deliveries and add personalization data to your content. Learn how to access, manage, and explore profiles using the Campaign Web User Interface in [this page](../audience/gs-audiences-recipients.md).

Audiences are sets of profiles who share similar behaviors and/or characteristics. This collection of people can either be generated, selected, or loaded. Once created, audiences can be leveraged as the target population of your deliveries. Learn how to build and manage audiences, how to select audiences for a delivery, and define control groups. Learn how to build and manage audiences, how to select audiences for a delivery, and define control groups in [this section](../audience/delivery-recipients.md).

**Configure workflows**

With workflows, you can orchestrate the full range of processes and tasks, improve the speed and scale of every aspect of your marketing campaigns, from creating segments and preparing messages to delivery. Plus, you can get your channels in sync with a single, easy-to-use interface for campaign orchestration.

Understand how workflows work and how to create a targeting workflow in this how-to video:

>[!VIDEO](https://video.tv.adobe.com/v/3448375?quality=12&captions=chi_hant)

Adobe Campaign Web user interface features a query modeler that simplifies the process of filtering the database based on various criteria. Learn how to use it in [this section](../query/query-modeler-overview.md)

**Work with deliveries**

You can create standalone deliveries from the **Deliveries** left menu, or create deliveries in the context of a workflow, included or not in a campaign. Learn how to create a delivery in [this page](../msg/gs-deliveries.md).

For an accelerated and improved design process, you can create delivery templates to easily reuse custom content and settings across your campaigns. This functionality enables you to standardize the creative look and feel, in order to be quicker in executing and launching campaigns. [Learn more](../msg/delivery-template.md)

Delivery settings are technical delivery parameters that are defined in the delivery template. They can be overloaded for each delivery. These settings are available from the **Settings** button available when editing a delivery or a delivery template.

Adobe Campaign Web dynamic content capabilities allow you to customize your content based on the information you have gathered about your recipients. By utilizing dynamic content, you ensure that your marketing efforts are more relevant, avoiding marketing unwanted or unnecessary products or services. Learn more about dynamic content in [this section](../content/fragments.md).

Once your delivery content has been defined, you can use profiles and test profiles to preview and test it before sending the message. This is a crucial step to ensure that it is accurate but also free of errors both in content and personalization settings.

* **Send email** - Learn how to create an email delivery from scratch, define the audience, design the content, simulate preview, and send a proof.
    Learn how to create your first targeted email. In this use case, you schedule the sending of an email to Silver and Gold loyalty members on a specific date.

    The Email Designer enables you to create captivating, individually tailored emails through an intuitive drag-and-drop interface.

    Learn how to preview email message content and personalization, send test deliveries (proofs) to specific recipients or subscribers for testing and validation, and check the email rendering in popular desktop, mobile, and web-based clients.

* **Send SMS** - SMS deliveries provide a practical and efficient way to send text messages to your customers' mobile devices. With this feature, you can create, personalize, and preview text-based messages for effective communication.

* **Send push notifications** - Push notifications are essential for reaching out to your mobile app users, even when they're not actively using your app. They serve various purposes like providing updates, driving specific actions, and notifying about deals.

    Adobe Campaign v8 can send rich push notifications. Parameters and settings depend on the mobile operating system:
    * Android Rich push documentation
    * iOS Rich push documentation

* **Send direct mail** - Direct mail is an offline channel that allows you to produce files to mass deliver personalized letters to your customers such as postcards, flyers, or catalogs. When creating a direct mail delivery, Adobe Campaign automatically generates an extraction file containing all the targeted profiles and selected data, such as postal addresses and profile attributes.<br/>

* **Create landing pages** - Adobe Campaign allows you to create, design, and share landing pages. Landing pages enable you to direct your users to online forms where they can update their data, opt-in/out from receiving your communications, or subscribe to a specific service such as a newsletter.

* **Use reporting** -  Adobe Campaign suite of reporting tools provides valuable insights into the effectiveness of your marketing efforts, allowing you to optimize your campaigns for maximum impact.

    Dynamic Reporting provides fully customizable and real-time reports to measure the impact of your marketing activities. It adds access to profile data, enabling demographic analysis by profile dimensions such as gender, city, and age in addition to functional email campaign data like opens and clicks.

>[!TAB Get started for Admins]

**Work with the client console** 

* **Install client console** - Learn how to download and install the Adobe Campaign Client Console, create and manage your connections to multiple environments, and verify access to the Adobe Campaign Client console with this tutorial video.

    Learn how to download, install, and manage the Adobe Campaign Client Console with this documentation.

* **Discover console client interface** - Learn about the Adobe Campaign v8 user interface and how to navigate the main features with this tutorial video.

    You can access Adobe Campaign via its client console or its Web user interface. You can also use APIs to manage data and perform tasks in your Campaign platform.

**Understand Campaign general architecture**

Learn about the typical Adobe Campaign solution deployment.

Adobe Campaign is a cross-channel marketing solution that automates email, mobile, social, and offline campaigns. Adobe Campaign provides a central place to access your customer data and profiles. Use Adobe Campaign to orchestrate consistent experiences for your customers, design, execute, and personalize your marketing across channels, while improving customer experiences on every device and touchpoint.

**Administrate environment**

* **Connect to your environment(s)** - Once the client console is installed, follow the steps in this documentation to create the connection to the application server.

* **Define permissions** - Adobe Campaign lets you define and manage the rights assigned to users. These permissions are defined by combining operator group permissions, named rights, and permissions on folders.

* **Use Campaign control panel** - The Adobe Campaign Control Panel allows Adobe Campaign administrators to monitor key assets and perform administrative tasks, such as managing the SFTP storage by instance, managing GPG keys, or subdomains and certificates.

    Control Panel allows you to set up new connections to your instances by adding IP address ranges to the allow list.
    Subdomain configuration allows you to configure a sub-section of your domain (technically a "DNS zone") for use with Adobe Campaign.
    In the Control Panel, you can interact with all SFTP servers that are connected to Campaign instances that you have access to.

* **Use the audit trail** - In Adobe Campaign Web User Interface, the Audit trail feature provides users with full visibility into all modifications made to important entities within your instance, typically those that significantly impact a smooth operation of the instance.

**Set up user interface**

* **Customize campaign UI** - Guidelines for managing user interface settings like lists, units, or data display.

* **Add custom fields** - Custom fields are additional attributes added to the out-of-the-box schemas through the Adobe Campaign console. These custom fields are displayed in various screens, for example, the details of a profile or a test profile.

**Set up the branding**

Every company has brand guidelines that define both visual elements and technical details. Adobe Campaign helps you manage these guidelines centrally, so you can present a consistent brand image to your customers in everything you do, from logos in emails to the URLs and domains used in your campaigns.

**Understand data model creation**

Adobe Campaign comes with a pre-defined data model. This section gives some details on the built-in tables of the Adobe Campaign data model and their interaction. Adobe Campaign relies on a Cloud database containing tables that are linked together.

A schema is an XML document associated with a database table. It defines data structure and describes the SQL definition of the table.
When you create or extend a schema, you need to create or modify the associated input forms to make those changes visible to end-users.
An input form lets you edit an instance associated with a data schema from the Adobe Campaign client console. The form is identified by its name and namespace.

**Understand data management**

Use Adobe Campaign workflows to improve the speed and scale of every aspect of your marketing campaigns, from creating segments and preparing messages to delivery.

Campaign helps you add contacts to the Cloud database. You can load a file, schedule and automate multiple contact updates, collect data on the Web, or enter profile information directly into the recipient table.

You can easily export your different reports to PDF or CSV format, which enables you to share, manipulate, or print them.
Quarantine is the way to manage the invalid addresses in deliveries.

**About delivery management**

Campaign Optimization is the Adobe Campaign module which lets you control, filter, and monitor the sending of deliveries. To avoid conflicts between campaigns, Adobe Campaign can test various combinations by applying specific constraint rules. This guarantees that the messages sent meet the needs and expectations of customers and company communication policies.

All marketing campaigns are based on a template, which stores main characteristics and capabilities. Campaign comes with a built-in template to create campaigns. This template has all functionalities enabled: Documents, Seed addresses, Approvals, Delivery outlines, etc.

Learn how to set up and manage subscriptions and target subscribers.

**Work with templates**

* **Campaigns** - Campaign templates contain pre-configured settings which can be reused for creating new campaigns. A set of built-in templates is available to help you get started.

* **Delivery** - For an accelerated and improved design process, you can create delivery templates to easily reuse custom content and settings across your campaigns. This functionality enables you to standardize the creative look and feel, in order to be quicker in executing and launching campaigns.

* **Workflows** - Workflow templates contain pre-configured settings and activities which can be reused for creating new workflows. Using a workflow template is a best practice if you need to regularly import files with the same structure.

* **Content blocks** - Learn how to create dynamic content blocks and how to use them to personalize the content of your email delivery.

* **Landing pages** - Once you design your landing page content, you can save it for future reuse.

* **Content fragments** - A content fragment is a reusable component that can be referenced in one or more messages. When modifying a fragment, every content using it is updated.

* **Triggers** - Each event can trigger a personalized message. For this to happen, you need to create a message template to match each event type. Templates contain the necessary information for personalizing the transactional message.

**Use subscription services**

Use Adobe Campaign Web to manage and create your services such as newsletters, and to check the subscriptions or unsubscriptions to these services.

**Configure delivery sending**

External accounts are used by technical processes such as technical workflows or campaign workflows. For example, when setting up a file transfer in a workflow or a data exchange with any other application (Adobe Target, Experience Manager, or other tools), you need to select an external account.

**Manage Adobe Campaign integrations**

You can connect your Campaign environment with Adobe Experience Cloud solutions and apps to combine capabilities.<br/>
Adobe Campaign comes with several connectors that allow you to communicate with external applications, connect to database engines, and share and synchronize data. These connections are configured by Adobe.

Here are the possible integrations:

**Use transactional messages**

Transactional messaging (Message Center) is a Campaign module designed for managing trigger messages. These notifications are generated from events triggered from information systems, and can include: invoices, order confirmations, shipping confirmations, password changes, product unavailability notifications, account statements, website account creations, and more.

**Use reporting**

Adobe Campaign provides a set of reporting tools.

>[!ENDTABS]

-->