---
audience: end-user
title: 使用查詢建模器建置您的第一個查詢
description: 瞭解如何在Adobe Campaign Web查詢建模器中建置您的第一個查詢。
exl-id: efd762b5-a7ae-49b4-ab74-5b43da1e574d
source-git-commit: a9c7ac9a7b43166bd3adba0d3463020b7f9353ab
workflow-type: tm+mt
source-wordcount: '2863'
ht-degree: 7%

---


# 建置您的第一個查詢 {#build-query}

若要開始建立查詢，請根據您要執行的動作，從您選擇的位置存取查詢建模器。 查詢建模器會以空白畫布開啟。 按一下&#x200B;**+**&#x200B;按鈕，設定查詢的第一個節點。

>[!IMPORTANT]
>
>可以使用全新的查詢建模器介面。 全新的規則產生器擁有簡化的介面，讓您更輕鬆地建立查詢。 若要切換至此體驗，請按一下右上角的切換按鈕。 您可以隨時返回傳統查詢建模器，只要按回切換鍵以停用新介面即可。 您可以在此新介面中套用與查詢建模程式相同的原則。
>&#x200B;>![顯示新規則產生器介面](assets/query-modeler-toggle.png){zoomable="yes"}切換的影像

您可以新增兩種型別的元素：

* **篩選元件** （自訂條件、選取對象、預先定義的篩選器）可讓您建立自己的規則、選取對象，或使用預先定義的篩選器來縮小查詢範圍。 它們會新增在查詢的開頭和虛線轉變上。 [瞭解如何使用篩選元件](#filtering)

  範例： *訂閱了&#39;Sports&#39;電子報的收件者*、*住在紐約的收件者*、*住在舊金山的收件者*

>[!BEGINTABS]

>[!TAB 傳統查詢模型工具]

![新增篩選元件至查詢的範例。](assets/query-add-component.png){zoomable="yes"}


>[!TAB 新規則產生器]

![新增篩選元件至查詢的範例。](assets/ruleb-1.png){zoomable="yes"}

>[!ENDTABS]



* **群組運運算元** (AND、OR、EXCEPT)可讓您將圖表中的篩選元件分組。 它們會在篩選元件之前新增到現有轉變上。 [瞭解如何使用運運算元](#filtering)

  範例： *超級VIP **和** VIP的收件者，可獎勵&#x200B;**或** VIP示範，**EXCEPT** 21歲或以上（含）的收件者。

>[!BEGINTABS]

>[!TAB 傳統查詢模型工具]

![描述：將群組運運算元新增至查詢的範例。](assets/ruleb-13.png){zoomable="yes"}

>[!TAB 新規則產生器]

![新增篩選元件至查詢的範例。](assets/ruleb-14.png){zoomable="yes"}

>[!ENDTABS]


## 查詢中的數值分佈 {#distribution-values-query}

值分佈會根據目前的查詢引數，顯示表格中欄位每個值的百分比。 瞭解查詢中值的分佈有助於調整分段。

若要存取此選項，請在查詢中按一下屬性選取按鈕，如下所示。 然後，按一下所選屬性旁的&#x200B;**[!UICONTROL 資訊]**&#x200B;圖示。 您可以存取&#x200B;**[!UICONTROL 值的分佈]**&#x200B;按鈕。

![描述：存取查詢中的值分佈選項。](assets/values_query.png){zoomable="yes"}

>[!NOTE]
>
>* 對於具有許多值的欄位，只會顯示前20個值。 在這種情況下，通知&#x200B;**[!UICONTROL 部分載入]**&#x200B;會警告您。
>* 每個屬性選擇器中都可以存取&#x200B;**[!UICONTROL 值分佈]**&#x200B;選項。 [瞭解如何選取屬性](../get-started/attributes.md)
>* 您可以使用&#x200B;**[ !A進階篩選器]**&#x200B;在結果上新增條件。 [若要了解更多資訊，請參閱此處](../get-started/work-with-folders.md#filter-the-values)。

## 新增篩選元件 {#filtering}

篩選元件可讓您使用下列專案來縮小查詢範圍：

* **[自訂條件](#custom-condition)**：使用資料庫和進階運算式的屬性建立您自己的條件，以篩選您的查詢。
* **[對象](#audiences)**：使用現有的對象來篩選查詢。
* **[預先定義的篩選器](#predefined-filters)**：使用現有的預先定義的篩選器來篩選查詢。

### 設定自訂條件 {#custom-condition}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_customcondition"
>title="自訂條件"
>abstract="自訂條件是篩選元件，允許您使用資料庫中的屬性和進階運算式來建立自己的條件，藉此篩選查詢。"

若要使用自訂條件篩選查詢，請執行下列步驟：

1. 按一下所需節點上的&#x200B;**+**&#x200B;按鈕，然後選取&#x200B;**[!UICONTROL 自訂條件]**。 自訂條件屬性窗格會在右側開啟。

1. 在&#x200B;**屬性**&#x200B;欄位中，從資料庫中選取要用來建立條件的屬性。 屬性清單包含campaign資料庫中的所有屬性，包括連結表格的屬性。 [瞭解如何選取屬性並將其新增至我的最愛](../get-started/attributes.md)

   ![在查詢中選取自訂條件的屬性。](assets/query-custom-condition-fields.png){zoomable="yes"}

   >[!NOTE]
   >
   >**編輯運算式**&#x200B;按鈕可讓您使用Campaign Web運算式編輯器，使用資料庫和協助程式函式的欄位來手動定義運算式。 [瞭解如何編輯運算式](expression-editor.md)

1. 從下拉式清單中選取要套用的運運算元。 可以使用各種運運算元。 請注意，下拉式清單中可用的運運算元取決於屬性的資料型別。

   +++可用運運算元清單

   | 操作員 | 用途 | 範例 |
   |---|---|---|
   | 等於 | 傳回與第二個「值」欄中所輸入資料相同的結果。 | 姓氏(@lastName)等於&#39;Jones&#39;只會傳回姓氏為Jones的收件者。 |
   | 不等於 | 傳回所有與輸入值不相同的值。 | 語言(@language)不等於&#39;English&#39;。 |
   | 大於 | 傳回大於輸入值的值。 | 年齡(@age)大於50會傳回所有大於「50」的值，例如「51」、「52」。 |
   | 小於 | 傳回小於輸入值的值。 | 「DaysAgo(100)」之前的建立日期(@created)將傳回所有在100天前建立的收件者。 |
   | 大於或等於 | 傳回等於或大於輸入值的所有值。 | 年齡(@age)大於或等於「30」將會傳回年齡等於或大於30歲的所有收件者。 |
   | 小於或等於 | 傳回等於或小於輸入值的所有值。 | 年齡(@age)小於或等於「60」將會傳回年齡等於或小於60歲的所有收件者。 |
   | 包含在 | 傳回指定值中包含的結果。 這些值必須以逗號分隔。 | 包含在「12/10/1979,12/10/1984」中的出生日期(@birthDate)將傳回這些日期之間出生的收件者。 |
   | 不在 | 其運作方式與「包含於」運運算元類似。 在這裡，收件者會根據輸入的值排除。 | 出生日期(@birthDate)不包含在&#39;12/10/1979,12/10/1984&#39;中。 將不會傳回在這些日期內出生的收件者。 |
   | 是空的 | 傳回與第二個「值」欄中的空值相符的結果。 | 行動裝置(@mobilePhone)為空白會傳回所有沒有行動號碼的收件者。 |
   | 不是空的 | 與Is empty運運算元相反的運作方式。 不需要在第二個「值」欄中輸入資料。 | 電子郵件(@email)不是空的。 |
   | 開始於 | 傳回以輸入值開頭的結果。 | 帳戶# (@account)以「32010」開頭。 |
   | 開頭不是 | 傳回不是以輸入值開頭的結果。 | 帳戶# (@account)的開頭不是&#39;20&#39;。 |
   | 包含 | 傳回至少包含輸入值的結果。 | 包含&#39;mail&#39;的電子郵件網域(@domain)將傳回包含&#39;mail&#39;的所有網域名稱，例如&#39;gmail.com&#39;。 |
   | 不包含 | 傳回不包含輸入值的結果。 | 電子郵件網域(@domain)不包含「vo」。 包含&#39;vo&#39;的網域名稱（例如&#39;voila.fr&#39;）將不會顯示在結果中。 |
   | 類似 | 與Contains運運算元類似，它可讓您在值中插入%萬用字元。 | 姓氏(@lastName)類似&#39;Jon%s&#39;。 萬用字元可當做「小丑」來尋找「Jones」之類的名稱。 |
   | Not like | 與Contains運運算元類似，它可讓您在值中插入%萬用字元。 | 姓氏(@lastName)不像&#39;Smi%h&#39;。 不會傳回姓氏為&#39;Smith&#39;的收件者。 |

   +++

1. 在&#x200B;**值**&#x200B;欄位中，定義預期的值。 您也可以使用Campaign網頁運算式編輯器，以使用資料庫和協助程式函式的欄位，手動定義運算式。 若要這麼做，請按一下&#x200B;**編輯運算式**&#x200B;按鈕。 [瞭解如何編輯運算式](expression-editor.md)

   *傳回21歲或以上所有設定檔的查詢範例：*

>[!BEGINTABS]

>[!TAB 傳統查詢模型工具]

![以年齡為21歲或以上的設定檔為目標的查詢範例。](assets/query-custom-condition.png){zoomable="yes"}

>[!TAB 新規則產生器]

![以年齡為21歲或以上的設定檔為目標的查詢範例。](assets/ruleb-3.png){zoomable="yes"}

>[!ENDTABS]

對於日期型別屬性，預先定義的值可使用&#x200B;**[!UICONTROL 預設集]**&#x200B;選項。

>[!BEGINTABS]

>[!TAB 傳統查詢模型工具]

![在查詢中使用日期預設集的範例。](assets/date-presets.png){zoomable="yes"}

>[!TAB 新規則產生器]

![在查詢中使用日期預設集的範例。](assets/ruleb-4.png){zoomable="yes"}

>[!ENDTABS]

#### 連結表格的自訂條件（1-1和1-N連結）{#links}

自訂條件可讓您查詢連結至規則目前使用之表格的表格。 這包括具有1-1基數連結的表格，或集合表格（1-N連結）。

若為&#x200B;**1-1連結**，請瀏覽至連結的資料表，選取所需的屬性並定義預期值。

您也可以直接選取&#x200B;**值**&#x200B;選擇器中的資料表連結並進行確認。 在此情況下，必須使用專用的選擇器來選取可用於所選表格的值，如以下範例所示。

+++查詢範例

在此，查詢會鎖定其標籤為「執行中」的品牌。

1. 在&#x200B;**Brand**&#x200B;資料表中導覽，並選取&#x200B;**標籤**&#x200B;屬性。

   ![品牌資料表的熒幕擷圖](assets/1-1-attribute.png){zoomable="yes"}{width="85%" align="center"}

1. 定義屬性的預期值。

   ![已定義預期值的範例](assets/1-1-table.png){zoomable="yes"}{width="85%" align="center"}

以下是已直接選取表格連結的查詢範例。 必須從專用選擇器選取此資料表的可用值。

![查詢範例的範例](assets/1-1-table-direct.png){zoomable="yes"}{width="85%" align="center"}

+++

對於&#x200B;**1-N連結**，您可以定義子條件來調整查詢，如下列範例所示。

+++查詢範例

在此，查詢會鎖定進行與BrewMaster產品相關購買的總金額至少為100$的收件者。

1. 選取&#x200B;**Purchases**&#x200B;資料表並確認。

   ![購買資料表的熒幕擷圖](assets/1-N-collection.png){zoomable="yes"}{width="50%" align="center"}

1. 會新增出站轉變，讓您建立子條件。

   ![外站轉變的範例](assets/1-n-subcondition.png){zoomable="yes"}{width="85%" align="center"}

1. 選取&#x200B;**價格**&#x200B;屬性，並且目標購買為1000$或更多

   ![Price屬性的熒幕擷圖](assets/1-n-price.png){zoomable="yes"}{width="85%" align="center"}

1. 新增子條件以符合您的需求。 我們在此處新增條件，以定位購買BrewMaster產品的設定檔。

   ![子條件的範例](assets/custom-condition-1-N.png){zoomable="yes"}{width="85%" align="center"}

+++

#### 使用彙總資料 {#aggregate}

自訂條件可讓您執行彙總作業。 若要這麼做，您必須直接從集合表格中選取屬性：

1. 在所需的集合表格內導覽，並選取您要執行彙總作業的屬性。

   ![屬性清單的熒幕擷圖](assets/aggregate-attribute.png){zoomable="yes"}{width="85%" align="center"}

1. 在屬性窗格中，開啟&#x200B;**彙總資料**&#x200B;選項並選取所需的彙總函式。

>[!BEGINTABS]

>[!TAB 傳統查詢模型工具]

![彙總資料選項的熒幕擷圖](assets/aggregate.png){zoomable="yes"}{width="85%" align="center"}

>[!TAB 新規則產生器]

![彙總資料選項的熒幕擷圖](assets/ruleb-5.png){zoomable="yes"}{width="85%" align="center"}

>[!ENDTABS]

### 選取客群 {#audiences}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_selectaudience"
>title="選取客群"
>abstract="透過使用「**選取客群**」選項，您可以選擇要用來篩選查詢的客群。"

若要使用現有對象篩選查詢，請執行下列步驟：

>[!BEGINTABS]

>[!TAB 傳統查詢模型工具]

1. 按一下所需節點上的&#x200B;**+**&#x200B;按鈕，然後選擇&#x200B;**[!UICONTROL 選取對象]**。

1. **選取對象**&#x200B;屬性窗格會在右側開啟。 選擇您要用來篩選查詢的對象。

   *查詢範例，傳回所有屬於「節日出席者」對象的設定檔：*

   ![查詢範例的Screenshof](assets/query-audience.png){zoomable="yes"}

>[!TAB 新規則產生器]

1. 按一下&#x200B;**[!UICONTROL 新增條件]**&#x200B;按鈕旁的&#x200B;**展開**&#x200B;按鈕，然後選擇&#x200B;**[!UICONTROL 選取對象]**。

1. **選取對象**&#x200B;屬性窗格會在右側開啟。 選擇您要用來篩選查詢的對象。

   *查詢範例，傳回屬於「Coffee Works」對象的所有設定檔：*

   ![查詢範例的Screenshof](assets/ruleb-7.png){zoomable="yes"}

>[!ENDTABS]

### 使用預先定義的篩選器 {#predefined-filters}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_predefinedfilter"
>title="預先定義的篩選器"
>abstract="透過使用「**預先定義的篩選器**」選項，您可以從自訂篩選器清單或常用篩選器中選取預先定義的篩選器。"

若要使用預先定義的篩選器來篩選查詢，請執行下列步驟：

>[!BEGINTABS]

>[!TAB 傳統查詢模型工具]

1. 按一下所需節點上的&#x200B;**+**&#x200B;按鈕，然後選取&#x200B;**[!UICONTROL 預先定義的篩選器]**。

1. **預先定義的篩選器**&#x200B;屬性窗格會在右側開啟。 從自訂篩選器清單或我的最愛選取預先定義的篩選器。

   *查詢範例，傳回與「非使用中客戶」預先定義篩選器對應的所有設定檔：*

   ![查詢範例的熒幕擷圖](assets/query-predefined-filter.png){zoomable="yes"}

>[!TAB 新規則產生器]

1. 按一下&#x200B;**[!UICONTROL 新增條件]**&#x200B;按鈕旁的&#x200B;**展開**&#x200B;按鈕，並選取&#x200B;**[!UICONTROL 預先定義的篩選器]**。

1. **預先定義的篩選器**&#x200B;屬性窗格會在右側開啟。 從自訂篩選器清單或我的最愛選取預先定義的篩選器。

   *查詢範例，傳回與「非使用中客戶」預先定義篩選器對應的所有設定檔：*

   ![查詢範例的熒幕擷圖](assets/ruleb-8.png){zoomable="yes"}

>[!ENDTABS]

### 複製貼上元件 {#copy}

查詢建模器可讓您複製一個或多個篩選元件，並在轉變結束時貼上這些元件。 此操作可在目前查詢畫布內執行，或在您執行個體內的任何畫布中執行。

>[!NOTE]
>
>只要您正在執行個體中工作，就會保留複製的選取範圍。 如果您登出並重新登入，您的選取範圍將無法再用於貼上。

>[!IMPORTANT]
>
>目前無法複製和貼上新規則產生器體驗中的元件。 若要依照這些後續步驟進行，請按一下頂端的&#x200B;**[!UICONTROL 回到傳統體驗]**&#x200B;切換按鈕，以使用傳統查詢模型工具。


若要複製貼上篩選元件，請執行下列步驟：

1. 在查詢畫布中按一下要複製的篩選元件，以選取該元件。 若要選取多個元件，請使用位於畫布右上角的工具列中可用的多重選取工具。

1. 在元件的屬性窗格中或熒幕底部的藍色功能區中（如果您已選取多個元件），按一下「**[!UICONTROL 複製]**」按鈕。

   | 複製單一元件 | 複製多個元件 |
   |  ---  |  ---  |
   | ![](assets/copy-single-component.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} | ![](assets/copy-multiple-components.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} |

1. 若要貼上元件，請按一下所需轉變結尾的+按鈕，並選取&#x200B;**貼上專案**。

   ![貼上元件的範例](assets/copy-paste.png){zoomable="yes"}

## 拖放元件 {#drag-and-drop}

>[!IMPORTANT]
>
>此功能僅適用於新的規則產生器體驗。

將元件新增至查詢時，您可以使用拖放功能上下移動元件。

在每個元件的左側，您可以按一下這些點並按住它們，以根據您想要放置和群組元件的位置來上下拖曳元件。

![Gif顯示如何在新規則產生器中拖放元件](assets/ruleb-drag.gif){zoomable="yes"}

## 將篩選元件與運算子結合 {#operators}

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_group"
>title="群組"
>abstract="在此窗格中，您可以變更用來將篩選條件連結在一起的運算子。"

每次將新的篩選元件新增到查詢時，它都會由&#x200B;**AND**&#x200B;運運算元自動連結到另一個元件。 這表示兩個篩選元件的結果會合併。

在此範例中，我們在第二個轉變中新增了對象型別的篩選元件。 元件連結至具有&#x200B;**AND**&#x200B;運運算元的預先定義篩選條件，這表示查詢結果包含「電子報訂閱者 — 馬德里」預先定義篩選器鎖定的收件者，且屬於「購買者（所有時間）」對象。

>[!BEGINTABS]

>[!TAB 傳統查詢模型工具]

![查詢範例](assets/query-operator.png){zoomable="yes"}

若要變更用來連結篩選條件的運運算元，請按一下該運運算元，然後在右側開啟的&#x200B;**群組**&#x200B;窗格中選取所需的運運算元。

可用的運運算元包括：

* **AND （交集）**：結合符合出站轉變中所有篩選元件的結果。
* **OR （聯集）**：包含至少符合出站轉變中一個篩選元件的結果。
* **EXCEPT （排除）**：排除符合出站轉變中所有篩選元件的結果。

![查詢範例](assets/query-operator-change.png){zoomable="yes"}

此外，您可以將元件分組到相同群組中，並將它們連結在一起，以建立中繼元件群組。 如此一來，預設會放入AND運運算元，然後您可以將其變更為所需的運運算元。

>[!TAB 新規則產生器]

![查詢範例](assets/ruleb-9.png){zoomable="yes"}

若要變更用來將篩選條件連結在一起的運運算元，請按一下該運運算元，它將會變更為「或」、「除外」，然後變更回「與」，並選取所需的運運算元。

可用的運運算元包括：

* **AND （交集）**：結合符合出站轉變中所有篩選元件的結果。
* **OR （聯集）**：包含至少符合出站轉變中一個篩選元件的結果。
* **EXCEPT （排除）**：排除符合出站轉變中所有篩選元件的結果。

![查詢範例](assets/ruleb-10.gif){zoomable="yes"}

>[!ENDTABS]

在下列範例中，我們已建立中繼群組以包含「要獎勵的VIP」或「超級VIP」對象的結果。

>[!BEGINTABS]

>[!TAB 傳統查詢模型工具]

![查詢範例](assets/query-intermediate-group.png){zoomable="yes"}

>[!TAB 新規則產生器]

![新規則產生器中的查詢範例](assets/ruleb-11.png){zoomable="yes"}

>[!ENDTABS]

## 檢查並驗證您的查詢

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_ruleproperties"
>title="規則屬性"
>abstract="在畫布中建立查詢後，您可以使用右側的&#x200B;**規則屬性**&#x200B;窗格進行檢查。<br/>此窗格可讓您顯示結果資料、擷取查詢的 SQL 程式碼版本，以及檢查目標記錄的數量。<br/>使用「**選取或儲存篩選器**」按鈕，將您的查詢儲存為預先定義篩選器，或將畫布內容更換為現有的篩選器。"

在畫布中建立查詢後，您可以使用右側的&#x200B;**規則屬性**&#x200B;窗格來檢查查詢。建立查詢以建立對象時，會顯示此窗格。 可用的操作包括：

* **檢視結果：**&#x200B;顯示查詢產生的資料。
* **程式碼檢視**：顯示SQL查詢的程式碼型版本。
* **計算**：更新並顯示查詢所定位的記錄數目。
* **選取或儲存篩選器**：選擇現有的預先定義篩選器以用於畫布中，或將您的查詢儲存為預先定義的篩選器，以供日後重複使用。 [瞭解如何使用預先定義的篩選器](../get-started/predefined-filters.md)

  >[!IMPORTANT]
  >
  >從「規則屬性」窗格中選取預先定義的篩選器，以選取的篩選器取代畫布中建立的查詢。

當您的查詢準備就緒時，請按一下右上角的&#x200B;**[!UICONTROL 確認]**&#x200B;按鈕以儲存查詢。


>[!BEGINTABS]

>[!TAB 傳統查詢模型工具]

您可以隨時透過開啟查詢來修改查詢。 請記住，開啟現有查詢時，它會顯示於簡化檢視中，而沒有&#x200B;**+**&#x200B;按鈕的可見度。 若要新增元素至查詢，請在畫布上選取元件或運運算元以顯示&#x200B;**+**&#x200B;按鈕。

![查詢範例](assets/edit-audience.png){zoomable="yes"}

>[!TAB 新規則產生器]

您可以隨時透過開啟查詢來修改查詢，若要這樣做，請按一下左上角的&#x200B;**[!UICONTROL 新增條件]**&#x200B;按鈕。

![新規則產生器中的查詢範例](assets/ruleb-11.png){zoomable="yes"}

>[!ENDTABS]
