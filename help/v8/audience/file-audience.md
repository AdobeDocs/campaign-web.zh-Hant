---
audience: end-user
title: 以檔案中的收件者為目標
description: 了解如何使用外部檔案中的收件者來建置您的電子郵件對象
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: fd9a5724aa9b97bffc6d143853742e0107bd3483
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 100%

---

# 從檔案載入收件者 {#audience-from-file}

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

您可以從外部檔案上傳聯絡人。此功能僅適用於電子郵件傳遞。支援的檔案格式包括：文字 (TXT) 和逗號分隔值 (CSV)。設定檔不會新增到資料庫中，但輸入檔案中的所有欄位都可用於個人化。

>[!NOTE]
>
>您可以建置匯入工作流程以便在資料庫中新增或更新多個設定檔。了解更多


若要直接從介面鎖定來自本機檔案的設定檔，請依照以下步驟進行：

1. 在電子郵件傳遞建立視窗中，在「**對象**」區段按一下「**選取對象**」按鈕，並選擇「**從檔案中選取**」選項。

   ![](assets/select-from-file.png)

1. 選取要上傳的本機檔案。
1. 在畫面中央區段預覽並檢查資料的對應方式。
1. 從「**地址欄位**」下拉式清單中選擇包含電子郵件地址的欄。如果輸入檔案中有這類資訊，您也可以選取「封鎖清單」欄。
1. 調整欄設定以及從可用選項中格式化資料的方式。
1. 當設定正確時，按一下「**確認**」。

建立和個人化訊息內容時，您可以在個人化編輯器中從輸入檔案選取欄位。

![](assets/select-external-perso.png)

>[!CAUTION]
>
>從外部檔案載入目標母體時，您不能使用[控制組](control-group.md)。

## 範例檔案 {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="範例檔案"
>abstract="支援的檔案格式：txt、csv。使用第一行作為欄標題。"


```json
{
lastname,firstname,city,birthdate,email,denylist
Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
Mars,Daniel,London,17/11/1999,dannymars@example.com,0
Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
}
```
