---
title: Campaign Standard與Campaign v8之間的差異
description: 瞭解從Campaign Standard轉換至Campaign v8時有何變更，以及可在何處尋找詳細資訊
hide: true
robots: noindex
googlebot: noindex
role: User, Admin, Developer
level: Beginner
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
  - id: d0e9f0b2-1f2b-4134-9844-49cd4e950f27
    internal-label: Campaign v8
  - id: ccdd4c6f-8203-4e89-85f0-79883f86f5fd
    internal-label: Campaign v8 Web User Interface
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
    internal-label: Beginner
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
source-git-commit: 64a07e65b7e6d933288b10117aae99f48d13a8d8
workflow-type: tm+mt
source-wordcount: '1721'
ht-degree: 2%
---
# Campaign Standard與Campaign v8之間的差異 {#acs-v8-differences}

Campaign Standard和Campaign v8中的大多數概念相同。 此頁面會收集轉換後對您造成影響的差異，並連結至說明每個差異的頁面。 它可補充[行銷人員](marketers.md)以及[管理員和開發人員](admin-developers.md)的指南。

* 如需術語變更，請參閱[Campaign Standard與Campaign v8](overview.md#experiences)之間的主要差異。
* 若要執行檢查以及轉換後回報的問題，請參閱[轉換後的檢查與疑難排解](post-transition-checks.md)。
* 如需使用者端主控台中才有的功能，請參閱[Campaign Web和Campaign使用者端主控台](../../v8/get-started/capability-matrix.md)。

## 管道和內容 {#channels}

兩個產品中建立和傳送訊息的步驟都類似，如[行銷人員指南](marketers.md)所述。 以下差異與管道可用性、測試傳送、登入頁面及直接郵件工作流程有關。

| 哪些變更 | 了解更多 |
|---|---|
| 應用程式內頻道在Campaign v8中無法使用。 | [應用程式內頻道](marketers.md#acs-gs-marketers-in-app) |
| 若要轉換現有的推播工作流程與傳送，請聯絡您的Adobe Campaign轉換經理。 | [推播通知](marketers.md#acs-gs-marketers-push) |
| 在Campaign Standard中，測試設定檔可標示為&#x200B;**陷阱**&#x200B;以接收最終傳送。 在Campaign v8中，在傳遞的對象設定中新增&#x200B;**陷阱群組**。 | [設陷群組](../../v8/audience/trap-group.md) |
| 在Campaign網頁使用者介面中建立的登入頁面不支援隱藏的輸入欄位或自訂JavaScript。 | [登陸頁面](../../v8/landing-pages/get-started-lp.md) |
| 在Campaign Standard中，直接郵件活動的出站轉變也攜帶了產生的檔案。 在Campaign v8中，僅攜帶目標母體。 若要將檔案傳送至伺服器，請新增&#x200B;**資料擷取**&#x200B;活動，然後新增&#x200B;**檔案傳輸**&#x200B;活動。 | [直接郵件](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/direct-mail){target="_blank"} |

## 對象、工作流程和傳遞 {#data-and-workflows}

這些差異會影響從Campaign Standard移轉的對象和工作流程、循環傳遞和&#x200B;**檔案傳輸**&#x200B;活動的某些選項，以及動態報告的範圍。

| 哪些變更 | 了解更多 |
|---|---|
| 對象會在轉換期間轉換。 例如，使用「查詢」活動建立的對象會成為預先定義的篩選器，而檔案型別的對象會成為沒有維度的清單型別對象。 | [管理對象](marketers.md#acs-gs-marketers-audiences) |
| Campaign Standard中執行的工作流程歷史記錄不會移轉。 | [建立工作流程](marketers.md#acs-gs-marketers-wf) |
| 在Campaign Standard中，您可以選取循環電子郵件的彙總期間。 此選項在Campaign v8中無法使用。 | [頻道活動](../../v8/workflows/activities/channels.md) |
| 動態報告涵蓋電子郵件傳送、具有電子郵件傳送的行銷活動以及異動訊息。 | [報告](marketers.md#acs-gs-marketers-reporting) |

## 存取與安全性 {#access}

Campaign Standard安全性群組、角色和組織單位會在轉換期間對應至操作員群組、已命名的許可權和檔案夾許可權。 請檢閱下列幾點，尤其是如果某些使用者的許可權比以前更寬或更窄。

| 哪些變更 | 了解更多 |
|---|---|
| 安全性群組、角色和組織單位會對應至操作員群組、已命名的許可權和檔案夾許可權。 自訂角色不會移轉。 | [使用者存取管理](user-management-acs.md) |
| 具有&#x200B;**資料模型**&#x200B;角色但不具有&#x200B;**管理**&#x200B;角色的使用者可取得&#x200B;**管理**&#x200B;存取權。 | [使用者存取管理](user-management-acs.md#migration-approach-from-user-roles-to-named-rights) |
| 在Campaign v8中，指派給具有平行組織單位之安全性群組的使用者可以有更廣泛的存取權。 | [平行組織單位指派](user-management-acs.md#parallel-assignments) |
| 從執行例項存取交易API需要新的產品設定檔。 | [產品設定檔對應](user-management-acs.md#product-profile-mapping-to-access-rest-apis) |
| 隱私權請求可能會在Campaign Standard環境保持作用中期間同時送達Campaign Standard和Campaign v8。 | [隱私權與同意](admin-developers.md#privacy-and-consent) |

## API和整合 {#apis-and-integrations}

這些差異會影響透過REST API呼叫Campaign的整合功能，以及與其他Adobe解決方案和工具的整合功能。

| 哪些變更 | 了解更多 |
|---|---|
| PKEY值會在移轉後變更。 如果您將PKEY儲存在Campaign之外，請改為遵循API傳回的href。 | [金鑰使用方式](#key-usage) |
| 部分已移轉的設定檔欄位（例如時區和`ccpaOptOut`）只會由`profileAndServicesExt/profile` API傳回。 | [設定檔時區](#profile-timezone) |
| Adobe會移轉您的Adobe Analytics和Audience Manager設定。 您必須再次設定觸發器和Adobe Target整合。 | [管理Adobe Campaign整合](admin-developers.md#acs-gs-integrations) |

## REST API建議和限制 {#rest-api-limitations}

從Campaign Standard轉換至Campaign v8時，下列建議和限制適用於REST API。

### 許可權與安全性 {#permissions}

#### 產品設定檔對應 {#rest-product-profiles}

在Campaign Standard中，無論您獲指派的產品設定檔為何，皆已授予您較高許可權的API管理員角色存取權。 Campaign v8引入一組不同的產品設定檔，需要從Campaign Standard對應到Campaign v8產品設定檔。

移轉後，會將兩個產品設定檔新增至您現有或預先建立的技術帳戶：管理員和訊息中心（用於存取交易API）。 如果您不希望管理員產品設定檔對應至您的技術帳戶，請檢閱產品設定檔對應，並指派所需的產品設定檔。

#### 租用戶 ID

移轉後，對於未來的任何整合，建議在REST URL中使用您的&#x200B;**Campaign v8租使用者ID**，取代您之前的Campaign Standard租使用者ID。

#### 金鑰使用方法

Campaign Standard和Campaign v8的PKey值管理方式不同。 如果您使用Campaign Standard儲存PKeys，請確定您的實作會使用從先前API呼叫取得的PKeys或href，以動態方式形成後續API呼叫。

### 可用的API {#available-apis}

目前，下列REST API可供使用：

* **設定檔**
* **服務與訂閱**
* **自訂資源**
* **工作流程**
* **異動訊息**

>[!AVAILABILITY]
>
>目前無法使用&#x200B;**交易式訊息** REST API。
>
>下列REST API已過時，無法使用：
>* 行銷歷史記錄
>* 組織單位
>* 隱私權管理

### 篩選 {#rest-filtering}

* 若要在REST API裝載中使用篩選器，您需要在Campaign v8中編輯篩選器，並提供要在裝載中使用的名稱。 若要這麼做，請從&#x200B;**[!UICONTROL 引數]**&#x200B;索引標籤存取篩選器的其他引數，並在REST API **欄位的**&#x200B;篩選名稱中提供所需的名稱。

  ![](assets/api-filtering.png)


* 使用自訂篩選器所需的「by」首碼已不再需要。 篩選器名稱的使用方式應與請求相同。

  範例：

  `GET https://mc.adobe.io/<ORGANIZATION>/campaign/profileAndServicesExt/<resourceName>/<customFilterName>?<customFilterparam>=<customFilterValue>`

### 捨棄的資料庫欄位 {#dropped-fields}

移轉期間會捨棄資料庫中的部分欄位。 使用下拉欄位時，REST API會傳回空白值。 所有捨棄的欄位都將被取代和移除。

### 使用連結的資源張貼 {#post-linked}

使用下列要求內文格式時，「vehicleOwner」代表「nms:recipient」的連結：

```
{
    "vehicleNumber": "20009",
    "vehicleName": "Model E",
    "vehicleOwner":{
        "firstName":"tester 11",
        "lastName":"Smith 11"
    }
}
```

連結資訊會被忽略。 因此，「cusVehicle」下會產生只包含「vehicleNumber」和「vehicleName」值的新記錄。 不過，連結仍保持空值，導致「vehicleOwner」設定為null。

在Campaign v8中，當使用相同的要求內文結構且「vehicle」連結至設定檔時，會發生錯誤。 發生此錯誤是因為「firstName」屬性無法辨識為「cusVehicle」有效。 不過，請求內文僅包含屬性，卻不包含連結函式，且沒有任何問題。

### PATCH作業 {#patch}

* Campaign v8不支援具有空白請求本文的PATCH：它會傳回204無內容狀態。
* 雖然Campaign Standard對結構描述中的元素/屬性支援PATCH，但請注意Campaign v8不支援對位置的PATCH操作。 嘗試在位置上PATCH會導致500內部伺服器錯誤，並出現錯誤訊息，指出「zipCode」屬性對「profile」資源無效。

### REST回應 {#rest-responses}

下節列出Campaign Standard與v8 REST回應之間的細微差異。

* 對於單一GET記錄，回應會將href納入回應中。
* 透過屬性查詢時，Campaign v8會在回應中提供計數和分頁。
* POST作業之後，回應中會傳回連結資源的值。

### 錯誤碼和訊息 {#rest-errors}

下節列出Campaign Standard與Campaign v8錯誤代碼和訊息之間的差異。

| 情境 | Campaign Standard | Campaign v8 |
|  ---  |  ---  |  ---  |
| 在請求內文中使用無效的PKey | 500 - &#39;O5iRp40EGA&#39;屬性不明(請參閱&#39;Profiles (nms:recipient)&#39;結構描述的定義)。 XTK-170036無法剖析運算式&#39;@id = @O5iRp40EGA&#39;。 | 404 — 無法解密PKey。 (PKey=@jksad) |
| 在URI中使用無效的API | 500 - &#39;O5iRp40EGA&#39;屬性不明(請參閱&#39;Profiles (nms:recipient)&#39;結構描述的定義)。 XTK-170036無法剖析運算式&#39;@id = @O5iRp40EGA&#39;。 | 404 — 無法解密PKey。 (PKey=@jksad)不支援的端點。 (endpoint=rest/profileAndServices/profile/@jksad) |
| 在URI和請求內文中使用兩個不同的原始Pkey | 500 - RST-360011發生錯誤 — 請聯絡您的管理員。 RST-360012資源&#39;service&#39;上的作業不一致 — 無法將索引鍵&#39;SVC3&#39;更新為&#39;SVC4&#39;。 | 500 — 發生錯誤 — 請聯絡您的管理員。 |
| 在URI中使用PKey，並在請求內文中使用不同的原始PKey | 500 — 具有相同索引鍵&#39;SVC4&#39;的&#39;Service&#39;已經存在。 PGS-220000 PostgreSQL錯誤：錯誤：重複的索引鍵值違反唯一條件約束「nmsservice_name」。詳細資料：索引鍵(sname)=(SVC4)已存在。 | 500 — 發生錯誤 — 請聯絡您的管理員。 |
| 在URI中使用不存在的原始識別碼 | 404 - RST-360011發生錯誤 — 請聯絡您的管理員。 無法從索引鍵「adobe_nl：0」（結構描述為「service」且名稱為「adobe_nl」的檔案）找到路徑為「Service」的檔案 | 404 — 無法從索引鍵「adobe_nl」找到路徑為「Service」的檔案（結構描述為「service」且名稱為「adobe_nl」的檔案） |
| 在請求內文中使用不存在的原始ID | 404 - RST-360011發生錯誤 — 請聯絡您的管理員。 無法從索引鍵「adobe_nl」找到路徑為「Service」的檔案（結構描述為「service」且名稱為「adobe_nl」的檔案） | 404 — 無法從索引鍵「adobe_nl」找到路徑為「Service」的檔案（結構描述為「service」且名稱為「adobe_nl」的檔案） |
| - | 500 - RST-360011發生錯誤 — 請聯絡您的管理員。 | 500 — 發生錯誤 — 請聯絡您的管理員。 |
| 插入包含無效性別（或任何）列舉值的設定檔/服務 | 500 - RST-360011發生錯誤 — 請聯絡您的管理員。 &#39;invalid&#39;值對&#39;@gender&#39;欄位的&#39;nms:recipient:gender&#39;列舉無效 | 500 — 發生錯誤 — 請聯絡您的管理員。 |

### 輪廓時區 {#profile-timezone}

使用Campaign Standard時，時區會顯示為&#x200B;**profileAndServices/profile** REST API呼叫的JSON回應的一部分。

使用Campaign v8時，時區只會顯示為&#x200B;**profileAndServicesExt/profile** REST API呼叫的一部分。 它不是&#x200B;**profileAndServices/profile** REST API呼叫的一部分，因為它已新增至擴充型結構描述。

### 工作流程外部訊號 {#workflow-signals}

Campaign Standard工作流程GET API會傳回引數名稱，例如工作流程例項變數及其資料型別（布林值、字串等）。 用來在透過POST API呼叫觸發訊號時建立適當格式化的JSON要求內文。

Campaign v8不支援廣告工作流程執行個體變數，但預期開發人員會知道這些變數。 因此，在移轉後，若沒有GET API回應中的引數資訊，就必須建構POST要求內文中的引數資訊。
