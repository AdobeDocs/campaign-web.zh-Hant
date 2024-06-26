---
audience: end-user
title: 從檔案載入電子郵件對象
description: 瞭解如何從外部檔案載入設定檔，以建立您的電子郵件對象
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: a0da65d8facedb3730947eb969e362a367e4d317
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 29%

---

# 從檔案載入電子郵件對象 {#audience-from-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="檔案選取"
>abstract="選取要上傳的本機檔案。支援的格式為 TXT 和 CSV。將您的檔案格式和以下連結的檔案範例保持一致。"

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="欄定義"
>abstract="檢查外部檔案的欄格式。"

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="格式化參數"
>abstract="指定外部文件的格式，確保可正確匯入資料。"

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_preview"
>title="預覽您的檔案"
>abstract="檢查外部檔案的欄預覽。此畫面最多僅顯示 30 筆記錄。"

Adobe Campaign Web使用者介面可讓您定位儲存在外部檔案中的設定檔。 載入設定檔後，輸入檔案中的所有欄位都可用於個人化您的傳送 [瞭解如何個人化您的內容](../personalization/personalize.md).

來自輸入檔案的設定檔不會新增至資料庫。 這些範本已載入，僅供此特定獨立電子郵件傳遞使用。

>[!NOTE]
>
>此頁面說明在建立獨立電子郵件傳送時，如何從檔案載入外部設定檔。 若要在工作流程內容中，從檔案載入資料，請參閱 [此頁面](../workflows/activities/load-file.md).

## 必讀 {#must-read}

* 此功能適用於 **電子郵件傳遞** 僅限。
* 支援的檔案格式為：文字(TXT)和逗號分隔值(CSV)。
* 從外部檔案載入目標母體時，您不能使用[控制組](control-group.md)。

## 選取並設定輸入檔案 {#upload}

若要從電子郵件中的檔案定位設定檔，請執行下列步驟：

1. 開啟現有的電子郵件傳遞，或 [建立新的電子郵件傳遞](../email/create-email.md).
1. 在 **對象** 區段，按一下 **選取對象** 按鈕，然後選擇 **從檔案選取**.

   ![](assets/select-from-file.png){zoomable=&quot;yes&quot;}

1. 選取要載入的本機檔案。 檔案格式必須與 [範例檔案](#sample-file).
1. 在畫面中央區段預覽並檢查資料的對應方式。

   ![](assets/select-from-file-map.png)

1. 指定包含電子郵件位址的欄， **位址列位** 下拉式清單。 如果輸入檔案中有這類資訊，您也可以選取「封鎖清單」欄。
1. 調整欄設定，以及如何從可用選項格式化資料。
1. 當設定正確時，按一下「**確認**」。

建立訊息內容時，您可以利用輸入檔案中的欄位來新增個人化。 [了解如何個人化內容](../personalization/personalize.md)

![](assets/select-external-perso.png){zoomable=&quot;yes&quot;}

## 範例檔案 {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="從檔案載入對象"
>abstract="支援的檔案格式為 TXT 和 CSV。使用第一行作為欄標題。讓您的檔案格式符合以下連結所提供的檔案範例。"

載入外部檔案以定位傳送中的設定檔時，請確定輸入檔案符合以下建議：

* 支援的格式為TXT和CSV。
* 檔案中的第一行是欄標題。
* 將檔案格式與下列範例檔案對齊：

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

使用從檔案上傳的對象時，Campaign Web可讓您預覽和傳送校樣。 要執行此操作，請依照下列步驟執行：

1. 按一下 **[!UICONTROL 模擬內容按鈕]** 在傳遞內容編輯畫面中按一下 **[!UICONTROL 新增測試設定檔]** 按鈕。

1. 上傳的檔案中包含的設定檔隨即顯示。 選取要用於預覽內容的設定檔，然後按一下 **[!UICONTROL 選取]**.

1. 傳遞內容的預覽會顯示在畫面的右側窗格中。 個人化元素會取代為左側窗格中選取之設定檔的資料。 [進一步瞭解傳遞內容預覽](../preview-test/preview-content.md)

   ![](assets/file-upload-preview.png){zoomable=&quot;yes&quot;}

1. 若要傳送校樣，請按一下 **[!UICONTROL 傳送證明]** 按鈕。

1. 按一下 **[!UICONTROL 上傳校訂設定檔]** 按鈕並選取包含校樣收件者的.txt或.csv檔案。

   >[!CAUTION]
   >
   >確保檔案格式符合用來上傳對象的格式。 任何格式錯誤都會顯示警報。

1. 新增校樣設定檔且您已準備好傳送校樣時，請按一下 **[!UICONTROL 傳送證明]** 按鈕並確認傳送。

   ![](assets/file-upload-test.png){zoomable=&quot;yes&quot;}

1. 您可以使用監控證明的傳送 **[!UICONTROL 檢視校樣]** 按鈕。 [進一步瞭解校訂監視](../preview-test/test-deliveries.md#access-test-deliveries)
