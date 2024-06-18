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

# 使用 **[!UICONTROL 陷阱群組]** {#trap-group}

A **[!UICONTROL 陷阱群組]** 用於鎖定不符合所定義目標條件的收件者。 如此一來，不在傳遞範圍的收件者可以像任何其他目標收件者一樣接收傳遞。
A **[!UICONTROL 陷阱群組]** 是一組 **[!UICONTROL 種子地址]**.

## 為何使用 **[!UICONTROL 陷阱群組]**

您可以使用 **[!UICONTROL 陷阱群組]** ：

1. **作為證明** ：每個成員 **[!UICONTROL 陷阱群組]** 將會收到傳送，就像是對象的一部分一樣。


1. **保護您的郵寄清單** ：透過接收對象將收到的內容，每個 **[!UICONTROL 種子地址]** 的 **[!UICONTROL 陷阱群組]** 若第三方使用郵寄清單，則會引起注意。

## 關於 **[!UICONTROL 陷阱群組]**

系統會自動從下列傳遞統計資料的報表中排除種子地址： **點按次數**， **開啟次數**， **取消訂閱**. 報表只說明真實受眾。

對於電子郵件傳遞，只需要電子郵件地址 **[!UICONTROL 陷阱群組]**，其他欄位的個人化將由Campaign隨機填入。

## 如何設定 **[!UICONTROL 陷阱群組]** 在傳遞中

若要設定 **[!UICONTROL 陷阱群組]**，前往 **[!UICONTROL 對象]** 傳送的設定。 您有2個選項：
- [選取測試設定檔](#select-test-profile)
- [建立條件](#create-condition)

![](assets/trap-group.png){zoomable="yes"}

### 選取測試設定檔 {#select-test-profiles}

選擇「選取測試設定檔」時，您會有一個視窗，邀請您前往 **[!UICONTROL 新增測試設定檔]** ：

![](assets/trap-no-test-profile.png){zoomable="yes"}

當您按一下按鈕時，您將有權存取您可新增的種子地址 **[!UICONTROL 陷阱群組]**. 勾選您要使用的專案。
您可以建立新的種子地址。 [了解更多](#create-seed)

![](assets/trap-select-test-profiles.png){zoomable="yes"}

當您確認補漏白位址時，請檢查下方的號碼是否正確 **[!UICONTROL 陷阱群組]**.

![](assets/trap-check.png){zoomable="yes"}

### 建立條件 {#create-condition}

使用 **[!UICONTROL 建立條件]** 選擇，您會看到一個新視窗，您可以在其中自訂查詢，以定義您要使用的種子地址：

![](assets/trap-create-condition.png){zoomable="yes"}

您的查詢將顯示在 **[!UICONTROL 陷阱群組]**.

![](assets/trap-custom.png){zoomable="yes"}

## 如何建立新的 **[!UICONTROL 種子地址]** {#create-seed}

您可以建立新的 **[!UICONTROL 種子地址]** 在 **[!UICONTROL 瀏覽器]** > **[!UICONTROL 資源]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL 種子成員]**

![](assets/trap-create.png){zoomable="yes"}

您可以填寫種子成員的所有詳細資訊，就像它是對象設定檔一樣：

![](assets/trap-create-contact.png){zoomable="yes"}