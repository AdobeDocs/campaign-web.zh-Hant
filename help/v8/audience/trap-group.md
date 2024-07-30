---
audience: end-user
title: 使用補漏白群組
hide: true
hidefromtoc: true
description: 瞭解如何在Campaign網頁使用者介面中使用陷阱群組進行傳遞
source-git-commit: 2feea0c5a1b021786e58bf6a69a2018ec37ea4b1
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 2%

---

# 使用&#x200B;**[!UICONTROL 陷阱群組]** {#trap-group}

**[!UICONTROL 陷阱群組]** （也稱為&#x200B;**[!UICONTROL 種子清單]**）可用來在您的傳遞中包含特定地址，以透過鎖定不符合定義的目標條件的設定檔來監控和驗證發佈程式。 如此一來，不在傳遞範圍的收件者可以像任何其他目標收件者一樣接收傳遞。
**[!UICONTROL 陷阱群組]**&#x200B;是AC Web UI上名為&#x200B;**[!UICONTROL 測試設定檔]**&#x200B;的&#x200B;**[!UICONTROL 種子位址]**&#x200B;群組。

## 為何使用&#x200B;**[!UICONTROL 設陷群組]**

您可以使用&#x200B;**[!UICONTROL 設陷群組]** ：

1. **作為證明** ： **[!UICONTROL 陷阱群組]**&#x200B;的每個成員都會收到傳遞，就像他們屬於對象一樣。


1. **為了保護您的郵寄清單** ：如果第三方使用郵寄清單，則透過接收對象將收到的內容，會注意到&#x200B;**[!UICONTROL Trap群組]**&#x200B;的每個&#x200B;**[!UICONTROL 測試設定檔]**。

>[!NOTE]
>
>設陷群組與建立傳遞](../email/create-email.md#preview-test)期間的[傳送校樣，以及與[控制組](control-group.md)不同。


## 關於&#x200B;**[!UICONTROL 陷阱群組]**

測試設定檔會自動從下列傳遞統計資料的報告中排除： **點按次數**、**開啟次數**、**取消訂閱**。 報表只說明真實受眾。

對於電子郵件傳遞，**[!UICONTROL 陷阱群組]**&#x200B;只需要電子郵件地址，其他欄位的個人化將由Campaign隨機填入。

## 如何在傳遞中設定&#x200B;**[!UICONTROL 陷阱群組]**

若要設定&#x200B;**[!UICONTROL 補漏白群組]**，請移至傳遞的&#x200B;**[!UICONTROL 對象]**&#x200B;設定。 您有2個選項：
- [選取測試設定檔](#select-test-profile)
- [建立條件](#create-condition)

![](assets/trap-group.png){zoomable="yes"}

### 選取測試設定檔 {#select-test-profiles}

選擇「選取測試設定檔」時，您會有以下視窗，邀請您&#x200B;**[!UICONTROL 新增測試設定檔]**：

![](assets/trap-no-test-profile.png){zoomable="yes"}

當您按一下按鈕時，您將可存取您可以新增&#x200B;**[!UICONTROL 補漏白群組]**的測試設定檔。 勾選您要使用的專案。
您可以建立新的測試設定檔。 [了解更多](#create-seed)

![](assets/trap-select-test-profiles.png){zoomable="yes"}

當您確認測試設定檔時，請檢查您在&#x200B;**[!UICONTROL 補漏白群組]**&#x200B;下是否有正確的號碼。

![](assets/trap-check.png){zoomable="yes"}

### 建立條件 {#create-condition}

透過&#x200B;**[!UICONTROL 建立條件]**&#x200B;選擇，您將獲得一個新視窗，您可以在其中自訂查詢以定義您要使用的測試設定檔：

![](assets/trap-create-condition.png){zoomable="yes"}

您的查詢將顯示在&#x200B;**[!UICONTROL 設陷群組]**&#x200B;下。

![](assets/trap-custom.png){zoomable="yes"}

## 如何建立新的&#x200B;**[!UICONTROL 測試設定檔]** {#create-seed}

您可以在&#x200B;**[!UICONTROL 總管]** > **[!UICONTROL 資源]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL 種子成員]**&#x200B;中建立新的&#x200B;**[!UICONTROL 測試設定檔]**

![](assets/trap-create.png){zoomable="yes"}

您可以完成&#x200B;**[!UICONTROL 測試設定檔]**&#x200B;的所有詳細資料，就像它是對象設定檔一樣：

![](assets/trap-create-contact.png){zoomable="yes"}