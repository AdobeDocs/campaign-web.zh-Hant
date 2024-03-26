---
audience: end-user
title: 設計直接郵件傳送
description: 瞭解如何使用Adobe Campaign Web設計您的直接郵件傳送
exl-id: aefba651-4125-4b1e-992f-1fe90fd95e4c
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 22%

---

# 設計摘取檔案 {#design-direct-mail}

>[!CONTEXTUALHELP]
>id="acw_directmail_content"
>title="摘取檔案內容"
>abstract="按一下&#x200B;**編輯內容**&#x200B;按鈕開始設計直接郵件提供者要求的摘取檔案。這可讓您定義檔案屬性 (例如標籤和格式)，並指定要包含在檔案中的欄。"

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_file"
>title="檔案屬性"
>abstract="設定摘取檔案的屬性，例如名稱和格式。您可以使用運算式編輯器運用資料庫中的屬性來個人化檔案名稱。"

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_content"
>title="內容"
>abstract="在此區段中，指定要在摘取檔案中顯示的欄。完成後，您可以使用&#x200B;**模擬內容**&#x200B;按鈕來預覽摘取檔案。"

若要設計直接郵件傳遞所產生之擷取檔案的內容，請按一下 **[!UICONTROL 編輯內容]** 按鈕，然後設定檔案屬性和內容。

## 設定擷取檔案屬性 {#properties}

1. 在 **[!UICONTROL 檔案名稱]** 欄位中，指定解壓縮檔案的所需名稱。 您可以使用資料庫的屬性來個人化檔案名稱。 若要這麼做，請按一下 **[!UICONTROL 開啟個人化對話方塊]** 圖示以開啟運算式編輯器。 [了解如何個人化您的內容](../personalization/personalize.md)

1. 在 **[!UICONTROL 檔案格式]** 欄位中，選擇所需的解壓縮檔案格式； **文字**， **文字使用與欄一起固定**， **CSV (Excel)** 或 **XML**.

1. 展開 **[!UICONTROL 擷取格式]** 區段，以存取與解壓縮檔案格式相關的特定選項。 可用值視選取的格式而定。

+++ 可用的擷取格式選項

   * **[!UICONTROL 使用第一行作為欄標題]** (文字/CSV (Excel)格式)：開啟此選項即可使用第一欄作為標題。
   * **[!UICONTROL 欄分隔符號]** （文字格式）：指定在解壓縮檔案中做為欄分隔符號使用的字元。
   * **[!UICONTROL 字串分隔符號]** （文字格式）：指定如何在擷取檔案中分隔字串。
   * **[!UICONTROL 行尾]** （文字格式）：指定如何在擷取檔案中分隔行尾。
   * **[!UICONTROL 編碼]**：選擇解壓縮檔案的編碼。
   * **[!UICONTROL 日期格式和分隔符號]**：指定在解壓縮檔案中日期應如何格式。
   * **[!UICONTROL 數字格式]**：指定解壓縮檔案中數字的格式設定。
   * **[!UICONTROL 匯出標籤而不是分項清單的內部值]**：如果您匯出分項清單值，而且想要擷取欄標籤（與內部ID不同，這些標籤較容易理解），請將此選項切換為開啟。

+++

1. 切換至 **[!UICONTROL 請求的數量]** 用於限制您傳遞的收件者人數的選項。

   ![](assets/dm-content-details.png){zoomable=&quot;yes&quot;}

## 設定擷取檔案欄 {#content}

在 **[!UICONTROL 內容]** 部分，指定要在擷取檔案中顯示的欄。 要執行此操作，請依照下列步驟執行：

1. 按一下 **[!UICONTROL 新增屬性]** 按鈕以建立新欄。
1. 選擇要顯示在欄中的屬性，然後確認。 新增欄之後，您可以變更其標籤，並使用編輯圖示修改關聯的屬性。
1. 重複這些步驟，視需要為解壓縮檔案新增任意數目的欄。
1. 若要使用其中一個欄來排序解壓縮檔案，請按一下 **[!UICONTROL 排序]** 欄並選取所需的排序方法。
1. 若要變更欄的位置，請使用向上鍵和向下鍵。

![](assets/dm-content-attributes.png)

您現在可以預覽解壓縮檔案，並傳送傳遞以產生解壓縮檔案。 [瞭解如何測試和傳送直接郵件訊息](send-direct-mail.md)
