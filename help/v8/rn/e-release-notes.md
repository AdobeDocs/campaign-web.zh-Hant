---
title: Campaign v8 Web 使用者介面早期發行說明
description: 探索下一個 Campaign Web 使用者介面版本的新功能
hide: true
hidefromtoc: true
exl-id: a4c6ecb7-d657-46de-aa55-90c4cb45164b
source-git-commit: d4f9f3562f7dc2550bf9fea01f27456fdfdad43e
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 46%

---

# 早期發行說明 {#e-release}

Adobe Campaign Web 使用者介面持續提供新功能、現有功能的增強功能並修正錯誤。所有變更都會在每個月月末整合於[發行說明](release-notes.md)中。

**在發行日期之前，以下早期發行說明如有更改，恕不另行通知**。連結、畫面和更新文件會於發行日期在[發行說明](release-notes.md)中發佈。

## 7月發行說明 {#24-7-release}

**發行日期**： 2024年7月30至31日

從7月發行版本開始，將推出下列功能和改進專案。

### 種子清單 {#24-7-2}

種子清單 (又稱&#x200B;**陷阱群組**) 是種子地址清單。它用於在您的傳遞中包含特定地址，然後定位與定義的目標標準不相符的設定檔。這樣，不在傳遞對象範圍內的收件者就可以像其他目標收件者一樣接收傳遞內容。您可以在傳送校訂時使用種子地址，或保護您的郵寄清單。

### 豐富推送通知範本{#24-7.3}

您現在可以傳送豐富推送通知。 豐富推送通知是行動通知的增強型形式，其不僅限於簡單的文字訊息，而是結合多媒體元素，例如影像、互動按鈕或其他豐富媒體內容。 此版本中，豐富推送通知的一組範本現在可供您的iOS和Android應用程式使用。

>[!AVAILABILITY]
>
>此功能需要更新Campaign v8.6.3或v8.7.2。[在Campaign使用者端主控台發行說明中瞭解更多](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/releases/release-notes)


### 功能改進 {#improvements-24-7}

**資料夾管理** — 您現在可以管理資料夾的許可權和限制。

### 有限可用性的新功能 {#acs-24-4}

>[!AVAILABILITY]
>
>以下功能為有限可用性 (LA) 版本。僅限適用於&#x200B;**從 Adobe Campaign Standard 移轉到 Adobe Campaign v8** 的客戶，且無法部署在任何其他環境中。
>
>請參閱以下文件頁面：「[Campaign Standard 轉換到 Campaign v8](../rn/acs-migration.md)」和「[適用於 Campaign Standard 使用者的功能](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=zh-Hant)」。

#### 內容片段 {#LA-24-7}

您現在可以建立和使用內容片段。 內容片段是可重複使用的元件，可在一或多個訊息中參照。 修改片段時，使用該片段的每個內容都會更新。 此功能允許預先建置多個自訂內容區塊，可供行銷使用者在改良的設計流程中快速組合訊息內容。

提供兩種型別的片段：

* **運算式片段**&#x200B;是預先定義的運算式，可從運算式編輯器中的專用專案取得。
* **視覺化片段**&#x200B;是預先定義的視覺化區塊，您可以在多個電子郵件傳遞或內容範本中重複使用。 [了解更多](../email/fragments.md)

  >[!AVAILABILITY]
  >
  >**視覺片段**&#x200B;為有限可用性(LA)。 此功能僅限將&#x200B;**從Adobe Campaign Standard移轉至Adobe Campaign v8**&#x200B;的客戶使用，且無法部署於任何其他環境。
