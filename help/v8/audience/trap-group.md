---
audience: end-user
title: 使用補漏白群組
hide: true
hidefromtoc: true
description: 瞭解如何在Campaign網頁使用者介面中使用陷阱群組進行傳遞
source-git-commit: 15d8ea478a234136dc654683798957d6c7026327
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 3%

---

# 使用&#x200B;**[!UICONTROL 陷阱群組]** {#trap-group}

**[!UICONTROL 陷阱群組]**用於鎖定不符合已定義目標條件的收件者。 如此一來，不在傳遞範圍的收件者可以像任何其他目標收件者一樣接收傳遞。
**[!UICONTROL 陷阱群組]**&#x200B;是&#x200B;**[!UICONTROL 種子地址]**&#x200B;的群組。

## 為何使用&#x200B;**[!UICONTROL 陷阱群組]**

您可以使用&#x200B;**[!UICONTROL 設陷群組]** ：

1. **作為證明** ： **[!UICONTROL 陷阱群組]**&#x200B;的每個成員都會收到傳遞，就像他們屬於對象一樣。


1. **為了保護您的郵寄清單** ：如果第三方使用郵寄清單，則透過接收對象將收到的內容，會注意到&#x200B;**[!UICONTROL Trap群組]**&#x200B;的每個&#x200B;**[!UICONTROL 種子位址]**。

## 關於&#x200B;**[!UICONTROL 陷阱群組]**

系統會自動從下列傳遞統計資料的報表中排除種子地址： **點按**、**開啟**、**取消訂閱**。 報表只說明真實受眾。

對於電子郵件傳遞，**[!UICONTROL 陷阱群組]**&#x200B;只需要電子郵件地址，其他欄位的個人化將由Campaign隨機填入。

## 如何在傳遞中設定&#x200B;**[!UICONTROL 陷阱群組]**

若要設定&#x200B;**[!UICONTROL 補漏白群組]**，請移至傳遞的&#x200B;**[!UICONTROL 對象]**&#x200B;設定。 您有2個選項：
- [選取測試設定檔](#select-test-profile)
- [建立條件](#create-condition)

![](assets/trap-group.png){zoomable="yes"}

### 選取測試設定檔 {#select-test-profiles}

選擇「選取測試設定檔」時，您會有以下視窗，邀請您&#x200B;**[!UICONTROL 新增測試設定檔]**：

![](assets/trap-no-test-profile.png){zoomable="yes"}

當您按一下按鈕時，您將可存取您能新增&#x200B;**[!UICONTROL 補漏白群組]**的種子地址。 勾選您要使用的專案。
您可以建立新的種子地址。 [了解更多](#create-seed)

![](assets/trap-select-test-profiles.png){zoomable="yes"}

當您確認您的補漏白位址時，請檢查您在&#x200B;**[!UICONTROL 補漏白群組]**&#x200B;下是否有正確的號碼。

![](assets/trap-check.png){zoomable="yes"}

### 建立條件 {#create-condition}

透過&#x200B;**[!UICONTROL 建立條件]**&#x200B;選擇，您將獲得一個新視窗，您可以在其中自訂查詢以定義您要使用的種子地址：

![](assets/trap-create-condition.png){zoomable="yes"}

您的查詢將顯示在&#x200B;**[!UICONTROL 設陷群組]**&#x200B;下。

![](assets/trap-custom.png){zoomable="yes"}

## 如何建立新的&#x200B;**[!UICONTROL 種子地址]** {#create-seed}

您可以在&#x200B;**[!UICONTROL 總管]** > **[!UICONTROL 資源]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL 種子成員]**&#x200B;中建立新的&#x200B;**[!UICONTROL 種子地址]**

![](assets/trap-create.png){zoomable="yes"}

您可以填寫種子成員的所有詳細資訊，就像它是對象設定檔一樣：

![](assets/trap-create-contact.png){zoomable="yes"}