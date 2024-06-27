---
audience: end-user
title: 傳遞警報
description: 瞭解如何使用傳送警報。
exl-id: 120afaa0-7017-4644-b6db-229b4a5c8a91
source-git-commit: bb61fdb34fecb4131d4069965cda8a3a5099b6bc
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 19%

---

# 開始使用傳遞警報 {#gs-delivery-alerting}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="傳遞警報"
>abstract="Campaign 中現已提供傳遞警報功能。此功能是警報管理系統，可讓使用者群組自動接收包含其傳送執行資訊的電子郵件通知。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=zh-Hant" text="請參閱版本注意事項"

「傳送警報」是警報管理系統，可讓使用者群組自動接收包含其傳送執行資訊的電子郵件通知。收件者可監控Adobe Campaign所處理的進行中傳遞，並在發生問題時採取適當的動作。

您可以根據透過Adobe Campaign Web使用者介面定義的特定警報條件來自訂通知。

有關如何管理傳送失敗的詳細資訊，請參閱 [Adobe Campaign v8 （主控台）檔案](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/delivery-failures#send){target="_blank"}

## 電子郵件通知內容 {#content}

電子郵件通知包括下列小節：

* **摘要**：顯示符合您定義條件的傳送數目，每個條件都有標籤和顏色。
* **詳細資料**：列出控制面板的所有已定義傳送條件，以及每個條件的對應傳送。

![](assets/alerting-email.png)

## 設定傳送警報 {#set-up}

為協助您設定這些警示，Campaign Web使用者介面可讓您建立並管理：

* **傳送警報儀表板**：指定收件者、設定要納入控制面板的警報條件，以及存取已傳送警報的歷史記錄。 [瞭解如何使用儀表板](../msg/delivery-alerting-dashboards.md)
* **傳遞警報條件**：Campaign Web使用者介面提供預先定義的警示准則（輸送量低的傳送、準備失敗的傳送……），您可將其新增至您的儀表板。 您也可以根據自己的需求建立條件。 [瞭解如何使用條件](../msg/delivery-alerting-criteria.md)

假設您只想通知具有管理許可權的使用者傳送失敗，並通知行銷使用者傳送軟跳出錯誤率高的情況。 若要完成此操作，請為每個收件者群組建立兩個獨立的控制面板，其中包含適當的條件。

>[!NOTE]
>
>若要存取及設定控制面板和警報條件，您必須擁有 **管理許可權** 或屬於 **傳遞主管** 安全性群組。 標準使用者無法存取Adobe Campaign介面中的儀表板，但會收到警報通知。 [進一步瞭解存取和許可權](../get-started/permissions.md)
