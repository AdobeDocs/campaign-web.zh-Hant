---
audience: end-user
title: 開始使用 AI 助理
description: 開始使用AI助理
badge: label="Beta"
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
hide: true
hidefromtoc: true
source-git-commit: af67094638cfc3c5c64385203340918f0f8f2482
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 40%

---

# 開始使用 AI 助理 {#generative-gs}

>[!BEGINSHADEBOX]

**目錄**

* **[開始使用AI助理](generative-gs.md)**
* [使用AI助理產生電子郵件](generative-content.md)
* [使用AI助理產生簡訊](generative-sms.md)
* [使用AI助理產生推播通知](generative-push.md)

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

AI助理是改善電子郵件內容的寶貴工具。 它簡化個人化和內容增強，將您的電子郵件傳遞最佳化，以便與您的對象產生更好的共鳴。

此功能可自動產生完整的電子郵件內容，以節省時間並確保一致的品質。 使用Generative AI，您可以輕鬆建立吸引人的電子郵件，提高溝通的效率和效益。

>[!NOTE]
>
>此功能在其Alpha版本中提供，且可能會有所變更，恕不另行通知。 它將在10月初啟用。

## 護欄和限制 {#generative-guardrails}

在Campaign中使用AI助理產生電子郵件的一般准則如下：

* 產生的內容品質強烈受到您定義的行銷目標/提示所影響。 使用定義明確的提示讓GenAI模型正確解譯。 
* 上傳品牌資產，以便對品牌內容取得準確資訊。 否則，內容會以公開可用的資訊為基礎。 上傳的內容可以有下列格式：PDF、JPEG、PNG或ZIP檔案（具有支援的檔案格式）。
* 建議上傳品牌資產的大小小於50MB。 大型檔案或大量影像可以運作，但處理時間會增加。
* 最好使用Adobe Campaign編寫的電子郵件範本 [內建電子郵件範本](../email/create-email-templates.md)，此元件為品牌特定範本或自訂範本，可建立您的電子郵件內容。 建議使用最多8至10個影像的電子郵件範本。


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
