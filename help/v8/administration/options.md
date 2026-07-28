---
title: 設定 [!DNL Campaign] 選項
description: 瞭解如何設定Campaign選項及建立自己的自訂選項。
exl-id: 44f90e34-e72e-4506-90d5-06ab68242d34
TQID: https://experienceleague.adobe.com/a3MU21qEI7ggDv-gUT4--glIkWdU05mz14v3U9Q2wnM
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2:
  - id: c5474392-5419-4296-9e41-f6f4ce4f6e9b
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 0638cc11f533521f7c8f3df3a80361b040a05b0c
workflow-type: tm+mt
source-wordcount: 592
ht-degree: 4%

---

# 設定 [!DNL Campaign] 選項 {#options}

>[!CONTEXTUALHELP]
>id="acw_options_list"
>title="選項"
>abstract="選項"

>[!CONTEXTUALHELP]
>id="acw_options_create"
>title="建立選項"
>abstract="建立選項"

Adobe Campaign網頁版包含技術選項，可讓您更明確地設定應用程式。 這些選項中有些是內建的，有些則可視需要手動新增。

>[!IMPORTANT]
>內建選項已預先設定，僅供進階使用者修改。 如果您有任何問題或請求，請聯絡您的Adobe代表。

## 存取Campaign選項 {#access}

可從&#x200B;**[!UICONTROL 管理]** / **[!UICONTROL 選項]**&#x200B;功能表取得選項。 使用篩選窗格縮小清單的範圍，並快速找出您需要的選項。

![](assets/options-list.png)\
[選項清單顯示在[管理] / [選項]功能表中]

>[!NOTE]
>雖然選項功能表位置在Adobe Campaign主控台和Web使用者介面之間有所不同，但清單仍相同，而且就像映象一樣運作。 如需可用選項的詳細資訊，請參閱[Campaign v7檔案](https://experienceleague.adobe.com/en/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options){target="_blank"}中的選項清單。

從選項清單中，您可以：

* **複製或刪除選項**：按一下省略符號按鈕，然後選取所要的動作。
* **修改選項**：按一下選項名稱以開啟其屬性。 進行變更並儲存。
* **建立自訂選項**：按一下&#x200B;**[!UICONTROL 建立選項]**&#x200B;按鈕。

## 建立選項 {#create}

Adobe Campaign Web使用者介面可讓您建立符合您需求的自訂選項。 在處理 **[!UICONTROL JavaScript 程式碼]**&#x200B;工作流程活動時，利用自訂選項來儲存中間資料特別實用。

若要建立選項：

1. 存取選項清單並按一下&#x200B;**[!UICONTROL 建立選項]**。
1. 輸入選項的名稱，選取其型別，然後設定所要的值。
1. 按一下&#x200B;**[!UICONTROL 建立]**&#x200B;以建立選項。

![建立選項介面，顯示名稱、型別和值的欄位](assets/options-create.png)

選項可作為資料的臨時儲存空間，提供下列優點：

* 輸入值：選項支援特定的資料型別，例如日期、整數、字串等。
* 彈性：選項可讓使用者有效率地儲存及擷取資料，而不需要管理資料庫表格。

在下列範例中，名為`sampleOption`的自訂選項是以初始值「a」建立的。 工作流程中的&#x200B;**[!UICONTROL JavaScript程式碼]**&#x200B;活動會修改此選項的值，並將其儲存在變數中。 更新的值會顯示在工作流程記錄檔中，並反映在&#x200B;**[!UICONTROL 選項]**&#x200B;功能表中。

1. 建立選項。

   ![自訂選項建立介面顯示名稱`sampleOption`和初始值「a」](assets/options-sample-create.png)

1. 設定&#x200B;**[!UICONTROL JavaScript程式碼]**&#x200B;活動並啟動工作流程。

   ![JavaScript程式碼活動設定介面](assets/options-sample-javascript.png)

1. 執行工作流程以在工作流程記錄檔中檢視更新的值。

   ![顯示自訂選項更新值的工作流程記錄檔](assets/options-sample-logs.png)

1. 更新的值現在會顯示在&#x200B;**[!UICONTROL 選項]**&#x200B;功能表中。

   ![選項功能表顯示自訂選項更新值](assets/options-sample-updated.png)

## 限制傳遞的寄件者電子郵件地址 {#restrict-sender-address}

根據預設，行銷人員可以在電子郵件傳遞的&#x200B;**[!UICONTROL 寄件者電子郵件]**&#x200B;欄位中輸入任何地址。 若要將此欄位限製為預先定義的地址清單，請建立或編輯內建`NmsDelivery_senderAddressMask`選項，並將其值設定為允許的寄件者地址逗號分隔清單，例如`abc@adobe.com,bcd@adobe.com`。

![從功能表限制值的選項](assets/option-restrict-from.png)

一旦此選項有值，**[!UICONTROL 來自電子郵件]**&#x200B;欄位就會變成僅包含這些地址的下拉式清單，而不是任意文字欄位。 如果選項不存在或其值為空白，則欄位仍會維持如前所述的任意文字。

![電子郵件中的可用值](assets/option-restrict-from2.png)

此限制是全域的。 它適用於每個品牌和傳遞範本，不支援個人化欄位，僅支援靜態地址。

如需&#x200B;**[!UICONTROL 來自電子郵件]**&#x200B;欄位的詳細資訊，請參閱[設定電子郵件內容](../email/edit-content.md#edit-content)。
