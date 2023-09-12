---
audience: end-user
title: 以檔案中的收件者為目標
description: 了解如何使用外部檔案中的收件者來建置您的電子郵件對象
badge: label="Beta"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: ed9d67c5d84826035785e9543f4ed7655aa094f1
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 50%

---

# 從檔案載入電子郵件對象 {#audience-from-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="檔案選取"
>abstract="選取要上傳的本機檔案。支援的格式為 TXT 和 CSV。將您的檔案格式和以下連結的檔案範例保持一致。"

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="欄定義"
>abstract="檢查要從本機檔案插入的欄格式。"

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="格式化參數"
>abstract="檢查檔案的格式化參數。"

您可以從外部檔案上傳聯絡人。設定檔不會新增至資料庫，但輸入檔案中的所有欄位都可用於 [個人化](../personalization/gs-personalization.md). 支援的檔案格式包括：文字 (TXT) 和逗號分隔值 (CSV)。

>[!CAUTION]
>
>* 此功能僅適用於 **獨立電子郵件傳遞**. 它不能用於工作流程，也不能用於SMS或推播傳遞。
>
>* 從外部檔案載入目標母體時，您不能使用[控制組](control-group.md)。

## 上傳檔案 {#upload}

若要直接從電子郵件介面從本機檔案定位設定檔，請遵循下列步驟：

1. 開啟現有的電子郵件傳遞，或 [建立新的電子郵件傳遞](../email/create-email.md).
1. 在電子郵件傳遞建立視窗中，在「**對象**」區段按一下「**選取對象**」按鈕，並選擇「**從檔案中選取**」選項。

   ![](assets/select-from-file.png)

1. 選取要上傳的本機檔案。格式必須與 [範例檔案](#sample-file).
1. 在畫面中央區段預覽並檢查資料的對應方式。
1. 從「**地址欄位**」下拉式清單中選擇包含電子郵件地址的欄。如果輸入檔案中有這類資訊，您也可以選取「封鎖清單」欄。
1. 調整欄設定以及從可用選項中格式化資料的方式。
1. 當設定正確時，按一下「**確認**」。

建立及個人化訊息內容時，您可以從輸入檔案中選取欄位： [個人化編輯器](../personalization/gs-personalization.md).

![](assets/select-external-perso.png)

## 預覽和測試您的電子郵件 {#test}

使用從檔案上傳的對象時，Campaign Web可讓您預覽和傳送測試電子郵件。 要執行此操作，請依照下列步驟執行：

1. 模擬內容
1. 開啟預覽。 按一下選取設定檔：從要使用的檔案中選取設定檔
1. 若要傳送測試電子郵件，請按一下測試
1. 測試模式：定義校樣目標
1. 從第二個檔案上傳測試電子郵件的目標（或使用相同的檔案）。 檔案格式設定遵循與上傳的檔案相同的方式
1. 對檔案格式執行的檢查
1. 按一下傳送

+ 預覽和測試區段的連結

**問題：**
* 沒有可用的檔案替代？

## 範例檔案 {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="從檔案載入對象"
>abstract="支援的檔案格式為TXT和CSV。 使用第一行作為欄標題。將您的檔案格式與下列連結中提供的範例檔案對齊。"

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
