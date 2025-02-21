---
audience: end-user
title: 開始使用 AI 助理
description: 開始使用AI助理
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: 3729a6159affbbb30d2cdab91d1e42dbf9df9c86
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 26%

---

# 使用 AI 助理 {#generative-gs}


>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="AI 助理"
>abstract="精心設計和個人化傳遞後，您可以使用 AI 助理來強化內容。此功能讓您可以藉由描述想要產生的內容來進行微調，進而簡化個人化和改善內容的流程。"


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="在 Campaign 中使用 AI 助理定義內容"
>abstract="若要將所選內容做為內容產生的輸入，請啟動&#x200B;**使用目前的內容進行增強**&#x200B;切換。您也可以上傳您的品牌資產以將其做為來源。如果您不使用所選內容，則必須上傳並選取品牌資產。"

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Adobe 生成式 AI 條款"
>abstract="要存取此功能，您必須同意 Adobe Experience Cloud 生成式 AI 使用者準則。請檢查此功能之任何輸出的準確性，並確保它適合您的使用案例。"
>additional-url="https://www.adobe.com/tw/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe 生成式 AI 使用者準則"

>[!INFO]
>
>透過[我們的即時功能預覽](https://experienceleague.adobe.com/en/apps/journey-optimizer/ai-assistant-content-accelerator)，親身體驗親身體驗各種功能，讓您親身體驗各項功能，全面瞭解各項功能。


隨著行銷業的競爭日益激烈，品牌們開始尋求有效率的方法，以有效率且快速的方式產生具影響力的內容。 Adobe Campaign Web中的AI助理採用Microsoft Azure OpenAI和Adobe Firefly技術，是Adobe的AI內容產生功能，徹底改變行銷人員透過電子郵件、簡訊、推播等通道建立專業且品牌一致的內容方式。 透過進階GenAI模型和對品牌指導方針的深入瞭解，AI Assistant會根據行銷目標自動產生個人化、吸引人且有效的內容，其內容針對品牌概述的樣式、版面、色調等最佳化。

AI 助理讓您利用直覺、簡單且無繁複手續的方式在多個頻道之間，包括電子郵件、SMS 和 Push 等建立和執行行銷活動，還能節省時間、提高效率並帶來更好的結果。

>[!IMPORTANT]
>
>* 開始使用此功能之前，請先閱讀相關的[護欄和限制](#generative-guardrails)。
>
>* 您必須先同意[使用者合約](https://www.adobe.com/tw/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)，才能在Adobe Campaign網頁中使用AI小幫手。 如需詳細資訊，請聯絡您的 Adobe 代表。

## 存取AI助理 {#generative-access}

適用於電子郵件、推播通知和簡訊的AI助理現在為「一般可用性(GA)」，可供所有使用者使用。 授予使用者存取權的必要許可權和步驟詳述如下。

+++  瞭解如何指派內容產生相關許可權

1. **建立產品設定檔** — 在[Admin Console](https://stage.adminconsole.adobe.com/)中，建立具有以下特定模式的產品設定檔：
   `Campaign - <instance-name> - AIAssistant`

1. **新增使用者** — 將必要的使用者新增至該產品設定檔，
或
   **建立使用者群組**&#x200B;並將該使用者群組新增至產品設定檔，並將使用者新增至該產品設定檔。

在[本節](../get-started/permissions.md)中瞭解如何定義Campaign中的許可權。

+++

## 護欄和限制 {#generative-guardrails}

在Adobe Campaign Web中使用AI助理產生電子郵件的一般准則如下：

* 產生的內容品質強烈受到您定義的行銷目標/提示所影響。 使用定義明確的提示讓GenAI模型正確解譯。 
* 上傳品牌資產，以便對品牌內容取得準確資訊。 否則，內容會以公開可用的資訊為基礎。 上傳的內容格式如下：PDF、JPEG、PNG或ZIP檔案（具有支援的檔案格式）。
* 已上傳品牌資產的大小上限為50MB。 大型檔案或大量影像可以運作，但處理時間會增加。
* 使用[內建電子郵件範本](../email/create-email-templates.md)、品牌特定範本或自訂範本，以使用AI助理建立您的電子郵件內容。 建議使用最多8至10個影像的電子郵件範本。
* 選擇變體時，請務必使用向上縮圖、向下縮圖或標幟圖示來報告任何有問題的輸出。
* 您使用AI助理須遵守Adobe Experience Cloud Generative AI使用指南。 [了解更多](https://www.adobe.com/tw/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)
* 作為Adobe提升在媒體建立中使用創作AI工具之透明度的承諾的一部分，Adobe將在內容或專案包含Content Credentials產生的資產下載或匯出時套用Firefly。 [了解更多](https://helpx.adobe.com/firefly/using/content-credentials.html)

下列限制適用於Adobe Campaign Web中的AI助理：

* Adobe Campaign Web中的AI助理目前僅支援英文版。 非英文輸入可能會產生不一致或錯誤的結果。 非英文回覆所引起的問題目前無法解決或改善。
* 僅適用於電子郵件、推播和簡訊頻道。
* GenAI內容可能並不一定都準確：請分享您的意見回饋，以便我們的工程師可以調整模型。
* 您可以上傳多個品牌資產，但只能針對特定世代使用一個品牌資產。

## AI Assistant內容產生功能 {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="電子郵件產生" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
使用AI助理產生<a href="generative-content.md"><strong>電子郵件</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="簡訊產生" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div>使用AI助理產生<a href="generative-sms.md"><strong>簡訊</strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="推播產生" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
使用AI助理產生<a href="generative-push.md"><strong>推播通知</strong></a>
</div>
<p></td>
</tr></table>
