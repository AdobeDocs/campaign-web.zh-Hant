---
audience: end-user
title: 使用捕捉器群組
description: 瞭解如何在Campaign網頁使用者介面中使用陷阱群組進行傳遞
exl-id: 48c34581-8825-4798-b24e-c462303f7645
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 4%

---

# 使用捕捉器群組 {#trap-group}

**[!UICONTROL 陷阱群組]** （也稱為&#x200B;**[!UICONTROL 種子清單]**）可用來在您的傳遞中包含特定地址，以透過鎖定不符合定義的目標條件的設定檔來監控和驗證發佈程式。 如此一來，不在傳遞範圍的收件者可以像任何其他目標收件者一樣接收傳遞。

**[!UICONTROL 陷阱群組]**&#x200B;是Campaign網頁使用者介面中名為&#x200B;**[!UICONTROL 測試設定檔]**&#x200B;的&#x200B;**[!UICONTROL 種子位址]**&#x200B;群組。

## 為何使用補漏白群組 {#why-trap-group}

您可以使用&#x200B;**[!UICONTROL 設陷群組]**：

1. **作為證明**： **[!UICONTROL 陷阱群組]**&#x200B;的每個成員都會收到傳遞，就像他們屬於對象一樣。

1. **為了保護您的郵寄清單**：如果第三方使用郵寄清單，則透過接收對象將收到的內容，將會注意到&#x200B;**[!UICONTROL Trap群組]**&#x200B;的每個&#x200B;**[!UICONTROL 測試設定檔]**。

>[!NOTE]
>
>除了[在建立傳遞](../email/create-email.md#preview-test)期間和從[控制群組](control-group.md)傳送校樣之外，新增設陷群組也是測試對象的一種好方法。

## 關於陷阱群組 {#about-trap-group}

測試設定檔會自動從下列傳遞統計資料的報告中排除： **點按次數**、**開啟次數**、**取消訂閱**。 報表僅著重於真實受眾。

對於電子郵件傳遞，**[!UICONTROL 陷阱群組]**&#x200B;只需要電子郵件地址。 其他欄位的個人化由Campaign隨機填入。

## 在傳遞中新增補漏白群組 {#trap-group-in-delivery}

若要設定&#x200B;**[!UICONTROL 補漏白群組]**，請移至您傳送的&#x200B;**[!UICONTROL 對象]**&#x200B;設定。 您有兩個選項：

* [選取測試設定檔](#select-test-profiles)
* [建立條件](#create-condition)

[補漏白群組設定介面熒幕擷圖](assets/trap-group.png){zoomable="yes"}

### 選取測試設定檔 {#select-test-profiles}

當您選擇&#x200B;**選取測試設定檔**&#x200B;時，請使用&#x200B;**新增測試設定檔**&#x200B;按鈕，如下所示：

[新增測試設定檔按鈕熒幕擷圖](assets/trap-no-test-profile.png){zoomable="yes"}

當您按一下按鈕時，可以存取要新增至&#x200B;**[!UICONTROL 補漏白群組]**&#x200B;的測試設定檔。 選取您要使用的專案。

您也可以建立新的測試設定檔。 [了解更多](#create-seed)

[選取測試設定檔介面熒幕擷圖](assets/trap-select-test-profiles.png){zoomable="yes"}

確認測試設定檔後，請檢查在&#x200B;**[!UICONTROL 補漏白群組]**&#x200B;下是否顯示正確的號碼。

[補漏白群組確認熒幕擷圖](assets/trap-check.png){zoomable="yes"}

### 建立條件 {#create-condition}

使用&#x200B;**[!UICONTROL 建立條件]**&#x200B;選項，建立查詢以定義您要使用的測試設定檔：

[建立條件介面熒幕擷圖](assets/trap-create-condition.png){zoomable="yes"}

您的查詢會顯示在&#x200B;**[!UICONTROL 陷阱群組]**&#x200B;下。

[補漏白群組查詢顯示熒幕擷圖](assets/trap-custom.png){zoomable="yes"}

## 建立新的測試設定檔 {#create-seed}

您可以從&#x200B;**[!UICONTROL 總管]** > **[!UICONTROL 資源]** > **[!UICONTROL 行銷活動管理]** > **[!UICONTROL 種子成員]**&#x200B;資料夾，建立新的&#x200B;**[!UICONTROL 測試設定檔]**。

[建立測試設定檔導覽熒幕擷圖](assets/trap-create.png){zoomable="yes"}

設定您&#x200B;**[!UICONTROL 測試設定檔]**&#x200B;的所有設定，就像任何設定檔一樣：

[測試設定檔組態熒幕擷圖](assets/trap-create-contact.png){zoomable="yes"}