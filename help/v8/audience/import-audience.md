---
audience: end-user
title: 從檔案匯入收件者
description: 了解如何從外部檔案匯入收件者
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: ef8418294540ee0462725cdaf6824ba7ee4d9b59
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 10%

---

# 從檔案匯入收件者 {#audience-from-file}

您可以上傳文字檔案(TXT)或逗號分隔值檔案(CSV)，從傳送介面新增或更新連絡人。 然後將它們新增至資料庫。

>[!NOTE]
>
>您也可以建立匯入工作流程來新增或更新多個設定檔。


要直接從介面從本地檔案添加配置檔案，請執行以下步驟：

1. 在傳送建立視窗中，按一下 **選取對象** 按鈕並選取 **從檔案中選擇** 選項。
1. 選取要上傳的本機檔案。
1. 定義欄設定及資料格式。 您可以使用 **忽略列** 切換。
1. 在畫面的中央區段中預覽資料的對應方式。
1. 按一下 **確認** 一旦設定正確。

建立和個人化訊息內容時，您可以在「個人化」編輯器中從輸入檔案選取欄位。

## 範例檔案 {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="範例檔案"
>abstract="支援的檔案格式：txt、csv。 使用第一行作為欄標題."


```json
{
lastname,firstname,birthdate,email,crmID
Smith,Hayden,23/05/1989,hayden.smith@example.com,124365
Mars,Daniel,17/11/1987,dannymars@example.com,123545
Smith,Clara,08/02/1989,clara.smith@example.com,124567
Durance,Allison,15/12/1978,allison.durance@example.com,120987
}
```
