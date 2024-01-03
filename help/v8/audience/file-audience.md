---
audience: end-user
title: 以檔案中的收件者為目標
description: 了解如何使用外部檔案中的收件者來建置您的電子郵件對象
badge: label="Beta"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: 6dcdfae8aa6d6346fc02217db77a96cf6d219fdc
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 35%

---

# 從檔案載入電子郵件對象 {#audience-from-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="檔案選取"
>abstract="選取要上傳的本機檔案。支援的格式為 TXT 和 CSV。將您的檔案格式和以下連結的檔案範例保持一致。"

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="欄定義"
>abstract="檢查外部檔案中的欄格式。"

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="格式化參數"
>abstract="檢查外部檔案的格式引數。"


>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_preview"
>title="預覽您的檔案"
>abstract="檢查外部檔案的欄預覽。 此畫面最多僅顯示 30 筆記錄。"


您可以定位儲存在外部檔案中的設定檔。 設定檔不會新增至資料庫，但輸入檔案中的所有欄位都可用於 [個人化](../personalization/gs-personalization.md). 支援的檔案格式包括：文字 (TXT) 和逗號分隔值 (CSV)。本文會說明在建立獨立電子郵件傳遞時，如何載入外部設定檔。 若要從工作流程中的檔案載入資料，請參閱 [此頁面](../workflows/activities/load-file.md).

>[!CAUTION]
>
>* 此功能僅適用於 **電子郵件傳遞**. 無法與SMS或推播傳遞搭配使用。
>
>* 從外部檔案載入目標母體時，您不能使用[控制組](control-group.md)。
>
>* 設定檔不會新增至資料庫，僅會載入並可用於此特定的獨立電子郵件傳送。

## 選取並設定您的檔案 {#upload}

若要直接從電子郵件介面從本機檔案定位設定檔，請遵循下列步驟：

1. 開啟現有的電子郵件傳遞，或 [建立新的電子郵件傳遞](../email/create-email.md).
1. 在電子郵件傳遞建立視窗中，在「**對象**」區段按一下「**選取對象**」按鈕，並選擇「**從檔案中選取**」選項。

   ![](assets/select-from-file.png)

1. 選取要使用的本機檔案。 格式必須與 [範例檔案](#sample-file).
1. 在畫面中央區段預覽並檢查資料的對應方式。
1. 從「**地址欄位**」下拉式清單中選擇包含電子郵件地址的欄。如果輸入檔案中有這類資訊，您也可以選取「封鎖清單」欄。
1. 調整欄設定以及從可用選項中格式化資料的方式。
1. 當設定正確時，按一下「**確認**」。

建立及個人化訊息內容時，您可以從輸入檔案中選取欄位： [個人化編輯器](../personalization/gs-personalization.md).

![](assets/select-external-perso.png)

## 範例檔案 {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="從檔案載入對象"
>abstract="支援的檔案格式為 TXT 和 CSV。使用第一行作為欄標題。讓您的檔案格式符合以下連結所提供的檔案範例。"

支援的格式為 TXT 和 CSV。第一行是欄標題。

將檔案格式與下列範例檔案對齊：

```javascript
{
lastname,firstname,city,birthdate,email,denylist
Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
Mars,Daniel,London,17/11/1999,danny.mars@example.com,0
Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
}
```

## 預覽和測試您的電子郵件 {#test}

使用從檔案上傳的對象時，Campaign Web可讓您預覽和傳送測試電子郵件。 要執行此操作，請依照下列步驟執行：

1. 按一下 **[!UICONTROL 模擬內容按鈕]** 在傳遞內容編輯畫面中按一下 **[!UICONTROL 新增測試設定檔]** 按鈕。

1. 上傳的檔案中包含的設定檔隨即顯示。 選取要用於預覽內容的設定檔，然後按一下 **[!UICONTROL 選取]**.

1. 傳遞內容的預覽會顯示在畫面的右側窗格中。 個人化元素會取代為左側窗格中選取之設定檔的資料。 [進一步瞭解傳遞內容預覽](../preview-test/preview-content.md)

   ![](assets/file-upload-preview.png)

1. 若要傳送測試電子郵件，請按一下 **[!UICONTROL 測試]** 按鈕。

1. 按一下 **[!UICONTROL 上傳校訂設定檔]** 按鈕並選取包含校樣收件者的.txt或.csv檔案。

   >[!CAUTION]
   >
   >確保檔案格式符合用來上傳對象的格式。 任何格式錯誤都會顯示警報。

1. 當校樣收件者新增且您已準備好傳送校樣時，請按一下 **[!UICONTROL 傳送測試電子郵件]** 按鈕並確認傳送。

   ![](assets/file-upload-test.png)

1. 您可以使用監控測試電子郵件的傳送 **[!UICONTROL 檢視測試電子郵件記錄]** 按鈕。 [進一步瞭解測試電子郵件監控](../preview-test/test-deliveries.md#access-test-deliveries)
