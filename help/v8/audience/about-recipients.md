---
title: 與收件者和對象合作
description: 瞭解如何使用收件者Campaign Web
badge: label="Beta"
source-git-commit: 5183dd0045c7f13e79f65eca5b31dfd4cde2f31d
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 34%

---

# 與收件者和對象合作 {#about-recipients}

>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="收件者的 360 檢視"
>abstract="建立新的收件者，並透過強大的報表和工具進行監控。存取收件者的屬性、互動和紀錄。使用篩選選項瀏覽收件者清單、編輯和更新其設定檔。"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="請參閱版本注意事項"


>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="設定檔"
>abstract="設定檔代表個人，旨在接收 Adobe Campaign 傳送的訊息。在 Adobe Campaign 中，收件者是用於傳送遞送內容 (電子郵件、SMS 等) 的預設設定檔。在此清單中，您可以根據您的權限查看收件者的設定檔。使用篩選選項瀏覽此清單。您可以編輯和更新一組小型收件者屬性。"

收件者是一個設定檔，旨在接收 Adobe Campaign 傳送的訊息。在 Adobe　Campaign 中，收件者是用於傳送內容 (電子郵件、簡訊等) 的預設用戶檔案。儲存在資料庫中的收件者資料可讓您建立將接收任何指定傳遞的對象，並在傳遞內容中新增個人化資料。 其他型別的設定檔儲存在資料庫中。 這些設定檔是針對不同用途而設計：例如，種子設定檔是用來在傳送給最終對象之前測試您的傳送。

只能從Campaign使用者端主控台新增收件者。 不過，您可以在Campaign網頁的 **收件者** 左側導覽邊欄的專案。 您也可以從該畫面編輯收件者的屬性。

若要編輯收件者的資料，請按一下其名稱旁邊的三個點，然後選擇 **編輯……**.

![編輯收件者設定檔](assets/recipient-edit.png)

您可以更新有限的屬性集，包括：名字、姓氏、電子郵件和電話號碼。

![更新收件者設定檔](assets/recipient-update.png)

>[!NOTE]
>
>此有限的設定檔編輯表單僅供測試版計畫測試使用。 它將在未來版本中改進。 它可讓使用者快速將電子郵件地址和電話號碼新增到任何設定檔，以便他/她可以測試電子郵件和簡訊頻道，並接收傳送的訊息。

您可以使用搜尋欄位從以下網址篩選收件者： **顯示篩選器** 按鈕。

您也可以從以下位置存取收件者： **瀏覽器** 檢視、瀏覽及建立檔案夾和子檔案夾，以及檢查相關的許可權。

![從總管檢視的收件者清單](assets/recipients-from-explorer.png)

>[!NOTE]
>
>根據您的許可權，您可能無法存取資料庫中儲存的完整收件者清單。 若要了解權限的詳細資訊，請參閱[本章節](../get-started/permissions.md)。

此外，您可以管理收件者對電子報等服務的訂閱和取消訂閱。 瞭解如何使用中的訂閱服務 [此頁面](manage-services.md)

您可以建立工作流程，以刪除重複、擴充、合併設定檔，以及建立對象。 若要了解詳細資訊，請參閱[本章節](../workflows/gs-workflows.md)。
