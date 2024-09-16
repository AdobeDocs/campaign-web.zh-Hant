---
title: 從Campaign Standard轉換後，開始使用Adobe Campaign v8
description: 瞭解開始使用新的Campaign v8應用程式所需的步驟
role: User, Admin, Developer
level: Beginner
source-git-commit: a1c16a9ba5e5ca844eaf82ed3b587f4f7a0b0873
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# 從 Campaign Standard 至 v8 {#ac-acs}

歡迎使用Adobe Campaign v8！

作為從Campaign Standard轉換到Campaign v8的使用者，本參考指南是專為您設計的。 它可幫助您熟悉新的Campaign環境，並逐步引導您完成開始使用角色所需的步驟。

1. 首先瞭解[Adobe Campaign v8](#new)的新增功能。

1. 接下來，根據您的角色](#experiences)，瞭解Adobe Campaign Standard與Adobe Campaign v8之間的[體驗差異。

## 新增功能 {#new}

在本頁中檢視Adobe Campaign網路使用者介面的最新增強功能。 如需重要功能和發行更新功能的完整清單，請參閱[本節](../../v8/rn/whats-new.md)。

### Campaign v8的增強功能 {#ac-enhancements}

以下列出Adobe Campaign v8隨附的主要增強功能。

* **網頁使用者介面**

  Adobe Campaign v8同時提供使用者端主控台和網頁使用者介面，滿足不同的使用者偏好和需求。 使用者端主控台提供強大的案頭應用程式體驗，而Web使用者介面則設計為直覺式且易於存取，因此對於熟悉Adobe Campaign Standard的行銷人員來說，是理想的選擇。

  網頁使用者介面與Adobe Campaign Standard有許多相似之處，但有些術語可能有所不同。

  您可以[在此](../../v8/campaign-web-home.md)進一步瞭解Adobe Campaign網頁使用者介面。

  ![](assets/home.png){zoomable="yes"}

  所有新功能和改進專案都列在[發行說明](../../v8/rn/release-notes.md)中。 Adobe Campaign Web 使用者介面版本會在持續傳遞模型上運作，透過該模型可採用更具擴充性、分階段的方式來部署功能。因此，這些發行說明每月會更新多次。請定期進行檢查。


* **效能**

  Adobe Campaign v8運用進階雲端規模的資料庫技術，大幅改善效能和效率。 此重新設計的架構提供數項主要優點：

   * *縮放*：系統現在支援大幅提高處理能力，批次處理處理吞吐量高達每小時&#x200B;**20百萬次作業**。 有了此新架構，甚至更高的設定檔也能以可預測的效能管理。
   * *速度*：系統已針對任何行銷活動進行改善：異動訊息的分段、傳遞準備或輸送量，目前為每小時&#x200B;**1百萬條**。

  完全受管理的雲端服務為使用者提供：

   * 即時資料探索：即時存取和分析資料，以獲得快速見解及更明智的決策。

   * 快速建立受眾：在數分鐘內輕鬆建立目標受眾，以實現更有效的行銷活動細分。

  整體而言，Adobe Campaign v8強大的架構以提升速度和效率，為管理廣泛而複雜的行銷活動提供了強大的基礎。

### Adobe Campaign v8的新功能 {#ac-new-features}

作為Campaign Standard使用者轉換到Adobe Campaign v8，您現在可以使用以下功能：

* **豐富推送**

  Adobe Campaign v8提供傳送豐富推送通知的功能，可吸引使用者的注意並鼓勵他們採取行動。 這些通知可包含各種元素，例如文字、影像、按鈕、倒數計時器、聲音等。

  ![](../../v8/push/assets/rich_push.png){zoomable="yes"}

  為了協助建立這些豐富的通知，Adobe Campaign v8提供各種範本，讓您能夠設計和自訂複雜通知的內容，例如輪播或計時器。

  您可以根據客戶的系統量身打造通知：

   * 針對[Android](../../v8/push/rich-push.md)範本

   * 針對[iOs](../../v8/push/rich-push.md)範本

  推播通知是吸引行動應用程式使用者的重要工具，即使他們未主動使用您的應用程式，您也可以與他們聯絡。

* **Adobe Experience Manager as a Cloud Service**

  Adobe Campaign v8與Adobe Experience Manager as a Cloud Service緊密整合，加強您為客戶提供個人化和豐富內容體驗的能力。 這項原生整合可簡化內容管理，並運用Adobe Experience Manager強大的功能來最佳化行銷工作。

  以下是透過這項整合啟用的主要功能：

   * *資產管理*：在Adobe Campaign v8中，電子郵件設計工具會提供選取器來存取和管理資產。 此功能可簡化將Adobe Experience Manager中的元素整合至您的傳送作業，讓內容管理更有效率。 [進一步瞭解資產管理](../../v8/integrations/aem-assets.md)

     ![](../../v8/integrations/assets/assets_6.png){zoomable="yes"}

   * *電子郵件範本匯入*： Adobe Campaign v8可讓您瀏覽並直接從Adobe Experience Manager將電子郵件範本匯入Campaign。 [進一步瞭解電子郵件範本匯入](../../v8/integrations/aem-content.md)

     ![](../../v8/integrations/assets/aem_6.png){zoomable="yes"}

  Adobe Experience Manager as a Cloud Service提供雲端原生的敏捷性，可讓您加速實現價值的時間，並適應不斷變化的業務需求。 此整合不僅可增強您的內容管理功能，也可讓您透過所有接觸點，將更個人化且吸引人的體驗提供給您的客戶。

* **AI Assistant — 內容加速器**

  Campaign AI Assistant可以讓您在電子郵件、簡訊和推播等管道直觀地建立和執行行銷活動，既簡單又輕鬆，同時還能節省時間、提高效率並帶來更好的結果。

  ![](../../v8/email/assets/full-email-1.png){zoomable="yes"}

  AI Assistant徹底改變您跨管道建立專業且品牌一致內容的方式。 透過進階GenAI模型並深入瞭解您的品牌方針，AI Assistant會根據行銷目標自動產生個人化、吸引人且有效的內容，其內容針對品牌概述的樣式、版面、色調等內容進行最佳化。

  AI Assistant可讓您以直覺的方式建立和執行行銷活動，既簡單又輕鬆，同時節省時間、提高效率並帶來更好的結果。

  ![](../../v8/email/assets/full-email-2.png){zoomable="yes"}

  它提供電子郵件範本的變體，並產生和重新產生影像。 在[本節](../../v8/email/generative-content.md)中進一步瞭解AI Assistant — 內容加速器。 Adobe Campaign v8有AI助理可用於[電子郵件](../../v8/email/generative-content.md)、[簡訊](../../v8/email/generative-sms.md)和[推播](../../v8/email/generative-push.md)。

* **升級的SMS基礎結構 — SMS v2.0**

  SMS的簡易性和易用性使其成為非常寶貴的通訊通道，此外還有其穩健性和在數十億台終端機上無與倫比的相容性。

  Adobe Campaign v8隨附新的基礎架構，可改善SMS的傳送。 [進一步瞭解新的簡訊設定](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/sms/sms){target="_blank"}。

* **已升級的推送基礎結構**

  Adobe Campaign v8隆重推出最新推播通知服務，以現代尖端技術為基礎打造的強大架構提供支援。 此服務旨在解鎖全新等級的擴充能力，確保您的通知能夠以順暢的效率觸及更廣泛的對象。 透過我們增強的基礎架構和最佳化程式，您可以期待更大規模且更可靠的服務，讓您以前所未有的方式與行動應用程式使用者互動和交流。

  [進一步瞭解升級的推送基礎結構](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/push/push-data-collection){target="_blank"}。


## Managed Services {#ac-managed-services}

Adobe Campaign v8 可作為 Managed Cloud Services，提供主動預防性監督、即時警報及服務管理。Adobe Managed Cloud Service 為行銷人員提供了更靈活、安全性更高、可擴充性也更大的跨頻道行銷管理解決方案，而且總體擁有成本低廉。 新產品結合了服務與主動性監督和及時警報。

## v8中新增的Campaign Standard功能 {#ac-v8-added}

為了讓您順利轉換到 Campaign v8，Campaign v8 中新增了關鍵的 Campaign Standard 功能。[本文件](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html){target="_blank"}對此進行了詳細說明。

* **動態報告**：動態報告提供完全可自訂的即時報告來測量行銷活動的影響。此功能新增對個人檔案資料的存取，除了開啟和點選這類功能性電子郵件行銷活動資料外，還可以按性別、城市和年齡等個人資料維度進行人口統計分析。[了解更多](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html){target="_blank"}。

* **集中品牌化**：每家公司都有各自的品牌視覺化與技術準則。有了 Adobe Campaign，您可以定義一組規格，從標誌到技術層面 (例如電子郵件寄件者、URL 或網域)，為客戶呈現一致的品牌。[了解更多](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html)

* **Rest API**  - 作為 Campaign Standard 移轉使用者，您可以使用 Rest API 為 Adobe Campaign 建立整合，並透過將 Adobe Campaign 與您使用的一組技術結合來建立自己的生態系統。[了解更多](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html?lang=zh-hant){target="_blank"}。

* **登陸頁面** - Campaign v8 登陸頁面進行了一些改進，以確保功能與 Campaign Standard 相同。請參閱[發行說明](../../v8/rn/release-notes.md#new-24-4)和登陸頁面[文件](../../v8/landing-pages/get-started-lp.md)以了解更多資訊。

* **視覺片段**  - 視覺片段是可重複使用的視覺元件，可在一個或多個電子郵件傳遞或在內容範本中進行參考。修改片段時，使用該片段的所有內容都會隨之更新。此功能可讓您預先建立多個自訂內容區塊，以便行銷使用者在改進的設計流程中使用這些內容區塊來快速組裝訊息內容。[了解更多](../../v8//content/use-visual-fragments.md)

## Campaign Standard和Campaign v8之間的主要差異 {#experiences}

Adobe Campaign v8和Adobe Campaign Standard中的大多數概念都類似。 不過，兩者有一些差異，如下所述。

### 術語變更 {#terminology-changes}

以下是Campaign Standard和Campaign v8之間的一些術語差異。

* 自訂資源為&#x200B;**綱要**
* 訊息稱為&#x200B;**傳遞內容**
* 產品使用者為&#x200B;**操作者**。
* 角色設定有&#x200B;**命名權限**
* 安全性群組為&#x200B;**操作者群組**。
* 組織實體透過&#x200B;**資料夾權限**&#x200B;進行管理

此外，身為現有的Campaign使用者，請注意有些概念已重新命名，以符合最新的術語標準。 這些變更僅適用於 Campaign Web 使用者介面，不會反映在用戶端主控台。它們總結如下。

* 收件者現在為&#x200B;**設定檔**。[了解更多](../../v8/audience/gs-audiences-recipients.md)。
* 種子地址現在為&#x200B;**測試設定檔**。[了解更多](../../v8/preview-test/test-deliveries.md)。
* 傳遞分析現在是&#x200B;**傳遞準備**。當您需要啟動訊息準備時，按一下「**準備**」按鈕。[了解更多](../../v8/monitor/prepare-send.md)。
* 電子郵件預覽現在可透過「**模擬內容**」按鈕取得。[了解更多](../../v8/preview-test/preview-test.md)
* 清單現在是&#x200B;**客群**。[了解更多](../../v8/audience/gs-audiences-recipients.md)。

## 新的使用者體驗

存取您角色的相關參考指南，以探索Adobe Campaign v8的新使用者體驗。

<table>
<tr>
  <td>
    <a href="marketers.md">
      <img alt="行銷活動管理員"src="./assets/digital_marketing.jpeg"/>
    </a>
    <div>
  </td>
  <td>
  <a href="admin-developers.md">
    <img alt="管理員或開發人員" src="./assets/admin.jpeg"/>
    </a>
    <div>
  </td>
  </tr>
  <tr>
    <td>
    <a href="marketers.md">
    <strong>行銷人員</strong>
    </a>
    </td>
    <td>
      <a href="admin-developers.md">
      <strong>系統管理員或開發人員</strong>
      </a>
    </td>
  </tr>
    <td>
    <em>行銷活動經理，媒體行銷專員</em>
    </td>
    <td>
      <em>系統管理員，技術行銷專員</em>
    </td>
  <tr>
    <td>
    <b>主要工作/職責包括：</b>
    </td>
      <td>
    <b>主要工作/職責包括：</b>
    </td>
  </tr>
  <tr>
    <td>
      <li>建立行銷活動
      <li>設計工作流程
      <li>測試及執行行銷活動
      <li>部署多頻道行銷活動
      <li>最佳化行銷活動
      <li>最佳化自動化行銷活動
    </td>
    <td>
        <li>存取管理
        <li>系統組態
        <li>系統自訂
    </td>
</tr>
</table>
</div>

<!--
## Deprecated items

Adobe constantly evaluates product capabilities to identify older features that should be replaced with more modern alternatives to improve overall customer value, always under careful consideration of backward compatibility.

Please refer to [this documentation for information on deprecated items](https://experienceleague.adobe.com/en/docs/campaign-standard/using/release-notes/deprecated-features).-->

