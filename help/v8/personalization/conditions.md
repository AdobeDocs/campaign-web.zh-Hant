---
title: 建立條件式內容
description: 瞭解如何在Adobe Campaign Web UI中定義條件以個人化您的內容
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Alpha" type="Positive"
exl-id: b650a859-e27d-4a36-a725-a1f5bb31e014
source-git-commit: 5598a82bf745659b8c1db8cb51b1a82cfd184093
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 1%

---

# 建立條件式內容{#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="建立條件式內容"
>abstract="建立條件式內容，以根據收件者的設定檔定義動態個人化，在滿足某些條件時自動取代文字區塊和影像。 此功能可將您的行銷活動提升到新的高度，並為您的受眾提供極具針對性的個人化體驗。"


條件式內容是一項強大的功能，可讓您根據收件者的設定檔建立動態個人化，在滿足某些條件時自動取代文字區塊和影像。 此功能可將您的行銷活動提升到新的高度，並為您的受眾提供極具針對性的個人化體驗。

例如，透過設定條件式內容欄位，您可以根據收件者的設定檔建立進階動態個人化。 當滿足特定條件時，會在訊息內容中取代文字區塊、連結、主旨行和/或影像。 例如，您可以根據Adobe Campaign資料庫中「性別」欄位的值顯示「先生」或「夫人」，或根據收件者偏好的語言包含其他連結。

## 個人化語法{#perso-syntax}



## 使用個人化編輯器中的條件{#condition-perso-editor}

若要定義交貨的條件式內容，請執行下列步驟：

1. 開啟傳遞並編輯內容。
1. 按一下 **[!UICONTROL 開啟個人化對話方塊]** 圖示（例如SMS），位於「訊息」欄位右側。

   ![](assets/open-perso-editor-sms.png)

1. 在個人化編輯器中，瀏覽至 **[!UICONTROL 輔助函式]**.
1. 按一下旁邊的「+」圖示 **若** 函式。 下列行會新增至中央畫面：
   `<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`
1. Replace `<FIELD>` 依個人化欄位。 例如，收件者的公司： `recipient.company`.
1. Replace `<VALUE>` 以要滿足的值取代。 例如，`ADOBE` 。




## 範例：條件式SMS主旨行{#condition-subject-line}

若要為SMS訊息建立條件式主旨行，請遵循下列步驟：

1. 開啟傳遞並編輯內容。
1. 按一下主旨列右側的「開啟個人化對話方塊」圖示。
1. 在個人化編輯器中，瀏覽至


```sql
<% if 
(recipient.email == 'recipient@domain.com' ) 
{ % >
<table>
    <tr>
        <td>variant A</td>
    </tr>
</table>
< % } 
else 
{ % >
<table>
    <tr>
        <td>variant B< td>
    </tr>
</table>
< % } 
%>
```
