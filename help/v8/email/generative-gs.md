---
audience: end-user
title: 開始使用AI助理
description: 開始使用AI助理
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: 5f7fe214c1c89b1ee25cea6d512bd1a55b5522ec
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 6%

---

# 使用AI助理 {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="AI 助理"
>abstract="精心打造並個人化您的傳遞內容後，請使用AI Assistant增強您的內容。 此功能可讓您描述要產生的內容，以微調內容，進而簡化個人化和內容改善。"

>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="在 Campaign 中使用 AI 助理定義內容"
>abstract="若要使用選取的內容作為內容產生的輸入，請啟動&#x200B;**以目前內容增強**&#x200B;切換按鈕。 您也可以上傳您的品牌資產以將其做為來源。如果您未使用選取的內容，則必須上傳及選取品牌資產。"

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Adobe 生成式 AI 條款"
>abstract="能否存取此功能取決於您對Adobe Experience Cloud Generative AI使用者指南的同意。 請檢閱此功能的任何輸出是否準確，並確定其適合您的使用案例。"
>additional-url="https://www.adobe.com/tw/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe 生成式 AI 使用者準則"

>[!INFO]
>
>透過[我們的即時功能預覽](https://experienceleague.adobe.com/en/apps/journey-optimizer/ai-assistant-content-accelerator)，親身體驗親身體驗各種功能，讓您親身體驗各項功能，全面瞭解各項功能。

隨著行銷產業變得更具競爭力，品牌們開始尋求有效率的方式，以迅速產生具影響力的內容。 Adobe Campaign Web中的AI助理採用Microsoft Azure OpenAI和Adobe Firefly技術，是Adobe的AI內容產生功能，可轉變行銷人員如何跨電子郵件、簡訊和推播通知等管道建立專業且品牌一致的內容。 透過進階GenAI模型和對品牌指導方針的深入瞭解，AI Assistant會根據行銷目標自動產生個人化、吸引人且有效的內容，針對品牌概述的樣式、版面、色調等最佳化內容。

AI Assistant可簡化跨管道（例如電子郵件、簡訊和推播通知）行銷活動的建立和執行作業，進而節省時間、改善效率並取得更好的結果。

>[!IMPORTANT]
>
>* 使用此功能之前，請先檢閱相關的[護欄和限制](#generative-guardrails)。
>
>* 您必須先同意[使用者合約](https://www.adobe.com/tw/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)，才能在Adobe Campaign Web中使用AI小幫手。 如需詳細資訊，請聯絡您的 Adobe 代表。

## 存取AI助理 {#generative-access}

電子郵件、推播通知和簡訊的AI助理現在已全面推出(GA)，可供所有使用者使用。 授予使用者存取權的必要許可權和步驟詳述如下。

+++ 瞭解如何指派內容產生相關許可權

1. **建立產品設定檔** — 在[Admin Console](https://stage.adminconsole.adobe.com/)中，建立具有以下特定模式的產品設定檔：
   `Campaign - <instance-name> - AIAssistant`

1. **新增使用者** — 將必要的使用者新增至該產品設定檔，\
   或\
   **建立使用者群組**&#x200B;並將該使用者群組新增至產品設定檔，然後將使用者新增至該產品設定檔。

在[本節](../get-started/permissions.md)中瞭解如何定義Campaign中的許可權。

+++

## 護欄和限制 {#generative-guardrails}

在Adobe Campaign Web中使用AI助理產生電子郵件的一般准則如下：

* 產生內容的品質很大程度上取決於您定義的行銷目標或提示。 使用定義明確的提示讓GenAI模型正確解譯。
* 上傳品牌資產以確保準確的On-Brand內容。 否則，內容會以公開可得的資訊為基礎。 上傳的內容格式如下：PDF、JPEG、PNG或ZIP檔案（具有支援的檔案格式）。
* 已上傳品牌資產的大小上限為50MB。 大型檔案或大量影像可能會增加處理時間。
* 使用[內建電子郵件範本](../email/create-email-templates.md)、品牌特定範本或自訂範本，以使用AI助理建立您的電子郵件內容。 建議使用最多8至10個影像的電子郵件範本。
* 選擇變體時，使用向上縮圖、向下縮圖或標幟圖示，報告任何有問題的輸出。
* 您使用AI助理須遵守Adobe Experience Cloud Generative AI使用者指南。 [了解更多](https://www.adobe.com/tw/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)。
* 作為Adobe承諾在媒體建立中使用創作AI工具時提高透明度的其中一環，Adobe在下載或匯出內容或專案(包含Firefly產生的資產)時套用Content Credentials。 [了解更多](https://helpx.adobe.com/firefly/using/content-credentials.html)。

下列限制適用於Adobe Campaign Web中的AI助理：

* Adobe Campaign Web中的AI助理目前僅支援英文版。 非英文輸入可能會產生不一致或錯誤的結果。 非英文回覆所引起的問題目前無法解決或改善。
* 僅適用於電子郵件、推播和簡訊頻道。
* GenAI內容不一定都是準確的。 分享您的意見回饋，讓工程師可以調整模型。
* 您可以上傳多個品牌資產，但只能針對特定世代使用一個品牌資產。

## AI Assistant內容產生功能 {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="[使用AI助理產生電子郵件]" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
使用AI助理產生<a href="generative-content.md"><strong>電子郵件</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="[使用AI助理產生簡訊]" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div>使用AI助理產生<a href="generative-sms.md"><strong>簡訊</strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="[使用AI助理產生推播通知]" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-push.md"><strong>使用AI助理產生推播通知</strong></a>
</div>
<p></td>
</tr></table>