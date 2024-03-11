---
audience: end-user
title: 開始使用內容助理
description: 開始使用內容助理
badge: label="Alpha"
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
hide: true
hidefromtoc: true
source-git-commit: 1bce844800ad82559bdefebddc96dcec58177f09
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 23%

---

# 開始使用內容助理 {#generative-gs}


>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Adobe 生成式 AI 詞彙"
>abstract="對此功能的存取權取決於您對Adobe Experience Cloud Generative AI使用者指南的同意，以及下列各項：您為此功能提供的任何提示、內容、補充資訊或其他輸入內容(a)都必須與特定內容連結，其中可能包括您的品牌推廣材料、網站內容、資料、此類資料的結構描述、範本或其他受信任檔案"

<!--
", and (b) must not contain any personal information (personal information includes anything that can be linked back to a specific invidual). You should review any output from this feature for accuracy and ensure that it is appropriate for your use case.
>additional-url="https://www.adobe.com/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe Generative AI User Guidelines"
-->

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="內容助理"
>abstract="精心設計和個人化傳遞後，您可以使用內容助理來強化內容。此功能可讓您透過描述您想產生的內容來進行微調，進而簡化個人化和改善內容的流程。"


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="定義內容生成的上下文"
>abstract="若要將所選內容做為內容生成的輸入，請啟動&#x200B;**使用目前的內容進行增強**&#x200B;切換。您也可以上傳您的品牌資產以將其做為來源。如果您不使用所選內容，則必須上傳並選取品牌資產。"

內容助理由創作AI提供技術支援，是改善電子郵件內容的寶貴工具。 它簡化個人化和內容增強，將您的電子郵件傳遞最佳化，以便與您的對象產生更好的共鳴。

此功能可自動產生完整的電子郵件內容，以節省時間並確保一致的品質。 使用Generative AI，您可以輕鬆建立吸引人的電子郵件，提高溝通的效率和效益。


您可在電子郵件中使用「促銷活動內容助理」，以： [產生影像](generative-image.md)， [產生文字內容](generative-content.md)， [產生完整的HTML內容](generative-email.md).

>[!NOTE]
>
>此功能在其Alpha版本中提供，且可能會有所變更，恕不另行通知。 它將在10月初啟用。

## 護欄和限制 {#generative-guardrails}

以下列出使用「內容助理」產生電子郵件的一般准則：

* 產生的內容品質強烈受到您定義的行銷目標/提示所影響。 使用定義明確的提示讓GenAI模型正確解譯。 
* 上傳品牌資產，以便對品牌內容取得準確資訊。 否則，內容會以公開可用的資訊為基礎。 上傳的內容可以有下列格式：PDF、JPEG、PNG或ZIP檔案（具有支援的檔案格式）。
* 建議上傳品牌資產的大小小於10MB。 大型檔案或大量影像可以運作，但處理時間會增加。
* 使用Adobe Campaign編寫的電子郵件範本，或是 [內建電子郵件範本](../email/create-email-templates.md) 以建立您的電子郵件內容。 建議使用最多8至10個影像的電子郵件範本。


下列限制適用於「Campaign內容助理」：

* 支援的語言只有英文
* 僅適用於電子郵件頻道
* GenAI內容可能並不一定都準確：請分享您的意見回饋，以便我們的工程師可以調整模型
* 您可以上傳多個品牌資產，但只能針對特定世代使用一個品牌資產



<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="文字產生" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong>使用內容助理產生文字</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-image.md">
<img alt="影像產生" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-image.md"><strong>使用內容助理產生影像</strong>
</div>
<p>
</td>
<td>
<a href="generative-email.md">
<img alt="電子郵件產生" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-email.md"><strong>使用內容助理產生電子郵件</strong></a>
</div>
<p></td>
</tr></table>
