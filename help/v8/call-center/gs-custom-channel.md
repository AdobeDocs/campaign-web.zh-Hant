---
audience: end-user
title: 開始使用自訂外部管道
description: 瞭解如何使用Adobe Campaign Web建立並傳送自訂外部通道傳遞
source-git-commit: 7438ce1805cde00cf5b76f05d72bd19d2ef2343a
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 1%

---

# 開始使用自訂外部管道 {#gs-custom-channel}

您可以直接從Adobe Campaign Web UI，根據與第三方整合的自訂外部管道來協調和執行傳遞。 自訂外部頻道的建立是在使用者端主控台中執行。

您可以在工作流程中設定自訂通道外部傳送，或作為獨立傳送，定義您的對象，並使用所有必要的聯絡和個人化資料產生可自訂的匯出檔案。

>[!NOTE]
>
>Web UI中的報告不適用於自訂管道外部傳遞。 您必須瀏覽至「使用者端主控台」才能存取報表。

以下步驟詳細說明獨立（一次性）傳送的程式。 大多數步驟類似於呼叫中心傳遞。 如需詳細資訊，請參閱此[頁面](../call-center/create-call-center.md)。

若要建立並傳送新的獨立自訂外部傳送，請遵循下列主要步驟：

1. 建立自訂外部通道，[瞭解詳情](#create-channel)
1. 建立傳遞，[瞭解詳情](#create-delivery)
1. 定義對象，[瞭解詳情](#select-audience)
1. 編輯內容，[瞭解詳情](#edit-content)
1. 預覽並傳送傳遞，[瞭解詳情](#preview-send)

## 建立自訂外部管道{#create-channel}

首先，您需要設定自訂外部通道。 以下是要在使用者端主控台中執行的主要步驟：

1. 設定結構以新增通道至可用通道清單。
1. 建立新的路由外部帳戶。
1. 建立與新頻道關聯的新傳遞範本。

如需詳細資訊，請參閱[使用者端主控台檔案](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/custom-channel.html)

## 建立傳遞{#create-delivery}

請依照下列步驟建立傳遞並設定其屬性：

1. 選取&#x200B;**[!UICONTROL 傳遞]**&#x200B;功能表並按一下&#x200B;**[!UICONTROL 建立傳遞]**&#x200B;按鈕。

1. 選擇所需的自訂外部管道，選取關聯的範本，然後按一下&#x200B;**[!UICONTROL 建立傳遞]**&#x200B;以進行確認。

   ![熒幕擷圖顯示自訂傳遞的建立](assets/cus-create.png){zoomable="yes"}


1. 在&#x200B;**[!UICONTROL 屬性]**&#x200B;下，輸入傳遞的&#x200B;**[!UICONTROL 標籤]**。

   ![熒幕擷圖顯示自訂傳遞的內容組態](assets/cus-properties.png){zoomable="yes"}

如需傳遞建立的詳細資訊，請參閱客服中心[檔案](../call-center/create-call-center.md#create-delivery)。

## 定義客群{#select-audience}

現在，您需要定義擷取檔案的目標對象。

1. 在傳遞頁面的&#x200B;**[!UICONTROL 對象]**&#x200B;區段中，按一下&#x200B;**[!UICONTROL 選取對象]**。

1. 選擇現有對象或建立您自己的對象。

   ![熒幕擷圖顯示自訂傳遞的對象選擇](assets/cc-audience2.png){zoomable="yes"}

如需對象定義的詳細資訊，請參閱客服中心[檔案](../call-center/create-call-center.md#select-audience)。

## 編輯內容{#edit-content}

現在，讓我們編輯自訂頻道傳送產生的擷取檔案內容。

1. 從傳遞頁面，按一下&#x200B;**[!UICONTROL 編輯內容]**&#x200B;按鈕。

1. 指定&#x200B;**[!UICONTROL 檔案名稱]**、選取&#x200B;**[!UICONTROL 檔案格式]**，並視需要為解壓縮檔案新增欄數。

   ![顯示擷取檔案之屬性組態選項的熒幕擷圖。](assets/cc-content-attributes.png)

如需內容版本的詳細資訊，請參閱客服中心[檔案](../call-center/create-call-center.md#edit-content)。

## 預覽並傳送傳遞{#preview-send}

當傳送內容準備就緒時，您可以使用測試設定檔來預覽並傳送校樣。 然後，您可以傳送傳遞以產生解壓縮檔案。

1. 從傳遞內容頁面，按一下&#x200B;**[!UICONTROL 模擬內容]**&#x200B;按鈕並選取測試設定檔。

   ![在傳遞內容頁面中顯示模擬內容選項的熒幕擷圖](assets/cus-simulate.png){zoomable="yes"}

1. 從傳遞頁面，按一下&#x200B;**[!UICONTROL 檢閱與傳送]**，然後按一下&#x200B;**[!UICONTROL 準備]**。 然後，確認。

   ![顯示準備選項和記錄檔功能表的熒幕擷圖](assets/cus-prepare.png){zoomable="yes"}

1. 按一下&#x200B;**[!UICONTROL 傳送]**&#x200B;以繼續進行最後的傳送程式，然後確認。

如需預覽和傳送的詳細資訊，請參閱客服中心[檔案](../call-center/create-call-center.md#preview-send)。
