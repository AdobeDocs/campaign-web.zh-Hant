---
audience: end-user
title: 檔案中的目標收件人
description: 瞭解如何使用外部檔案中的收件人構建電子郵件受眾
badge: label="Alpha" type="Positive"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: a6c85aeed30726532ab6060fec5cb4b5e398d9ec
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 34%

---

# 檔案中的目標收件人 {#audience-from-file}

可以從外部檔案上載聯繫人。 此功能僅可用於電子郵件遞送。支援的格式為：文本檔案(TXT)或逗號分隔值檔案(CSV)。 然後將它們新增至資料庫。

>[!NOTE]
>
>您可以構建導入工作流以添加或更新多個配置檔案。  了解更多


要直接從介面從本地檔案目標配置式，請執行以下步驟：

1. 在「電子郵件傳遞建立」窗口中，按一下 **選擇受眾** 按鈕 **從檔案中選擇** 的雙曲餘切值。

   ![](assets/select-from-file.png)

1. 選取要上傳的本機檔案。
1. 在畫面中央預覽資料的對應方式。
1. 從中選擇包含電子郵件地址的列 **地址欄位** 下拉。
1. 調整列設定以及如何從可用選項設定資料格式。
1. 當設定正確時，按一下「**確認**」。

建立和個人化訊息內容時，您可以在個人化編輯器中從輸入檔案選取欄位。

![](assets/select-external-perso.png)

## 範例檔案 {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="範例檔案"
>abstract="支援的檔案格式：文本。 使用第一行作為欄標題。"


```json
{
lastname,firstname,city,birthdate,email,denylist
Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
Mars,Daniel,London,17/11/1999,dannymars@example.com,0
Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
}
```
