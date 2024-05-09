---
audience: end-user
title: 開始使用 AI 助理
description: 開始使用AI助理
badge: label="Beta"
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
hide: true
hidefromtoc: true
source-git-commit: f96c807c2ee094ad4775b6bf56f5f02822da8d28
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 39%

---

# 開始使用 AI 助理 {#generative-gs}

>[!BEGINSHADEBOX]

**目錄**

* 開始使用 AI 助理
* [使用 AI 助理產生電子郵件](generative-content.md)
* [使用 AI 助理產生簡訊](generative-sms.md)
* [使用 AI 助理產生推播](generative-push.md)

>[!ENDSHADEBOX]

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="AI 助理"
>abstract="精心設計和個人化傳遞後，您可以使用 AI 助理來強化內容。此功能可讓您透過描述您想產生的內容來進行微調，進而簡化個人化和改善內容的流程。"


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="在 Campaign 中使用 AI 助理定義內容"
>abstract="若要將所選內容做為內容生成的輸入，請啟動&#x200B;**使用目前的內容進行增強**&#x200B;切換。您也可以上傳您的品牌資產以將其做為來源。如果您不使用所選內容，則必須上傳並選取品牌資產。"


>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Adobe 生成式 AI 詞彙"
>abstract="若要取得此功能的存取權限，您必需同意 Adobe Experience Cloud 生成式 AI 使用者準則。您為此功能提供的任何提示、上下文或補充資訊或其他輸入都必須與特定上下文相關聯，其中可以包括您的品牌素材、網站內容、資料、此類資料的架構、範本或其他可信任文件，並且不得包含任何個人資訊 (個人資訊包括任何可連結到特定個人的資訊)。您應該檢查此功能之任何輸出的準確性，並確保它適合您的使用案例"
>additional-url="https://www.adobe.com/tw/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe 生成式 AI 使用者準則"

隨著行銷業的競爭日益激烈，品牌們開始尋求有效率的方法，以有效率且快速的方式產生具影響力的內容。 Campaign中的AI Assistant是Adobe的AI支援內容產生功能，徹底改變行銷人員跨電子郵件、簡訊、推播等通道建立專業且品牌一致內容的方式。 透過進階GenAI模型和對品牌指導方針的深入瞭解，AI Assistant會根據行銷目標自動產生個人化、吸引人且有效的內容，其內容針對品牌概述的樣式、版面、色調等最佳化。

AI Assistant可以讓您在電子郵件、簡訊和推播等通路上，以直覺的方式建立和執行行銷活動，既簡單又輕鬆，同時還能節省時間、提高效率和取得更好的結果。

>[!NOTE]
>
>此功能在其Beta版中提供，且可能會有所變更，恕不另行通知。

## 護欄和限制 {#generative-guardrails}

在Campaign中使用AI助理產生電子郵件的一般准則如下：

* 產生的內容品質強烈受到您定義的行銷目標/提示所影響。 使用定義明確的提示讓GenAI模型正確解譯。 
* 上傳品牌資產，以便對品牌內容取得準確資訊。 否則，內容會以公開可用的資訊為基礎。 上傳的內容可以有下列格式：PDF、JPEG、PNG或ZIP檔案（具有支援的檔案格式）。
* 已上傳品牌資產的大小上限為50MB。 大型檔案或大量影像可以運作，但處理時間會增加。
* 最好使用Adobe Campaign編寫的電子郵件範本 [內建電子郵件範本](../email/create-email-templates.md)，此元件為品牌特定範本或自訂範本，可建立您的電子郵件內容。 建議使用最多8至10個影像的電子郵件範本。
* 選擇變體時，請務必使用向上縮圖、向下縮圖或標幟圖示來報告任何有問題的輸出。
* 您使用AI助理須遵守Adobe Experience Cloud Generative AI使用指南。 [了解更多](https://www.adobe.com/tw/legal/licenses-terms/adobe-gen-ai-user-guidelines.html)

下列限制適用於Campaign中的AI助理：

* 支援的語言只有英文。
* 僅適用於電子郵件、推播和簡訊頻道。
* GenAI內容可能並不一定都準確：請分享您的意見回饋，以便我們的工程師可以調整模型。
* 您可以上傳多個品牌資產，但只能針對特定世代使用一個品牌資產。

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="電子郵件產生" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>使用AI助理產生電子郵件</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="簡訊產生" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-sms.md"><strong>使用AI助理產生簡訊</strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="推播產生" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-push.md"><strong>使用AI助理產生推播通知</strong></a>
</div>
<p></td>
</tr></table>
