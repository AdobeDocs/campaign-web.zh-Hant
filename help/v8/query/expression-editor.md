---
audience: end-user
title: 使用查詢建模器建置您的第一個查詢
description: 瞭解如何在Adobe Campaign Web查詢建模器中建置您的第一個查詢。
source-git-commit: e620df0ff9af0d32fc353a904e3dde37501495d0
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 79%

---

# 編輯運算式 {#expression}

編輯運算式需要手動輸入條件以形成規則。 此模式可讓您使用進階功能。這些函式可讓您控制用於執行特定查詢的值，例如控制日期、字串、數值欄位、排序等。

這些操作可從查詢建模器「編輯運算式」按鈕取得，在設定自訂條件時可用於屬性和值欄位。

![](assets/edit-expression.png)

運算式編輯器提供：

* 定義運算式的輸入欄位。
* 可用欄位清單，可用於運算式中，並對應至查詢的定位維度。
* 可用函式的清單，按類別排序。

直接在輸入欄位中輸入運算式，或使用可用欄位和函式清單來編輯運算式。 若要這麼做，請將游標置於要新增元素的內文運算式中，然後按兩下所需的欄位或運算式。

您可使用工作流程的事件變數來建立運算式。有關詳細資訊，請參見xxxx。

## 運算式語法 {#expression-syntax}

### 標準語法 {#standard-syntax}

標準運算式由一或多個符合下列語法元素的條件組成：

* 每個條件都採用 **&lt;value1> &lt;comparison operator> &lt;value2>** 行式，其中：

   * **&lt;value1>** 是一個欄位或函式。例如，**@created** 適用於建立設定檔的日期，或是 **Year(@created)** 適用於建立設定檔的年份。
   * **&lt;comparison operator=&quot;&quot;>** 是「比較」運運算元區段中所列的運運算元。 此運算子定義 **&lt;value1>** 及 **&lt;value2>** 之間的比較方法。
   * **&lt;value2>** 是手動輸入的欄位、函式或值。

  >[!NOTE]
  >
  >**&lt;value1>** 及 **&lt;value2>** 類型資料必須相同。例如，如果 **&lt;value1>** 是日期，則 **&lt;value2>** 也必須是日期。

* 如果要使用多個條件，可以使用邏輯運算子將它們組合起來。

   * **[!UICONTROL 和]**：兩個條件相交。
   * **[!UICONTROL 或]**：兩個條件結合在一起。

例如：

```
Year(@created) = Year(GetDate()) AND Month(@created) = Month(GetDate())
```

在此範例中，會定位其建立日期為目前月份和年份的描述檔。

### JavaScript語法 {#javascript-syntax}

在定義 HTML 內容編輯器的文本類型區塊的可見性條件時，必須使用具有 JavaScript 類型語法的運算式。

JavaScript 運算式由一或多個條件組成，並使用下列語法元素：

* 每個條件都採用 **&lt;context> &lt;comparison operator> &lt;value2>** 行式，其中：

   * **&lt;context>** 是可讓您指定上下文的欄位或函式。例如，**context.profile.@email** 適用於設定檔的電子郵件地址，或者 **context.profile.firstName.length()** 適用於設定檔名字的字元數。
   * **&lt;comparison operator=&quot;&quot;>** 是「比較」運運算元區段中所列的運運算元。 此運算子定義 **&lt;context>** 及 **&lt;value2>** 之間的比較方法。
   * **&lt;value2>** 是手動輸入的欄位、函式或值。

  >[!NOTE]
  >
  **&lt;context>** 及 **&lt;value2>** 類型資料必須相同。例如，如果 **&lt;context>** 是日期，則 **&lt;value2>** 也必須是日期。

* 如果要使用多個條件，可以使用邏輯運算子將它們組合起來。

   * **[!UICONTROL &amp;&amp;]**：兩個條件相交。
   * **[!UICONTROL ||]**：兩個條件結合在一起。

例如：

```
context.profile.age > 21 && context.profile.firstName.length() > 0
```

在此範例中，已提供 21 歲以上且其名字的描述檔（以 **firstName** 欄位至少包含一個字元為例）。

## 比較運運算元 {#comparison-operators}

對於某些規則，查詢編輯器可讓您選取值來定義條件。

條件必須使用下列其中一個運算子連結至值。

<table> 
 <thead> 
  <tr> 
   <th> 運算元<br /> </th> 
   <th> 標準語法<br /> </th> 
   <th> JavaScript 語法<br /> </th> 
   <th> 說明<br /> </th> 
   <th> 範例 <br /> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <span class="uicontrol">Equal to</span> <br /> </td> 
   <td> =<br /> </td> 
   <td> ==<br /> </td> 
   <td> 第一個值必須與第二個值完全相同。<br /> </td> 
   <td> <strong>@lastName = Martin</strong> 會擷取其姓氏為　'Martin'　的描述檔，只會擷取這些相同字元。<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">Greater than</span> <br /> </td> 
   <td> &gt;<br /> </td> 
   <td> &gt;<br /> </td> 
   <td> 第一個值必須斷斷續續大於第二個值。<br /> </td> 
   <td> <strong>@age &gt; 50</strong> 會擷取早於　'50'、'51'、'52'　等描述檔。<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">Less than</span> <br /> </td> 
   <td> &lt;<br /> </td> 
   <td> &lt;<br /> </td> 
   <td> 第一個值必須斷斷續續小於第二個值。<br /> </td> 
   <td> <strong>@created &lt; DaysAgo(100)</strong>，搜尋在少於　100　天前的資料庫中建立的所有設定檔。<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">Greater than or equal to</span> <br /> </td> 
   <td> &gt;=<br /> </td> 
   <td> &gt;=<br /> </td> 
   <td> 第一個值必須大於或等於第二個值。<br /> </td> 
   <td> <strong>@age &gt;= 30</strong> 會擷取年齡在　30　歲以上的描述檔。<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">Less than or equal to</span> <br /> </td> 
   <td> &lt;=<br /> </td> 
   <td> &lt;=<br /> </td> 
   <td> 第一值必須小於或等於第二值。<br /> </td> 
   <td> <strong>@age &lt;= 60</strong> 會接取年齡在　60　歲或以下的設定檔。<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">Different </span> <br /> </td> 
   <td> !=<br /> </td> 
   <td> !=<br /> </td> 
   <td> 第一個值必須與第二個值不同。<br /> </td> 
   <td> <strong>@language ! = English</strong> 會擷取尚未設定為說英語的設定檔。<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">Contains</span> <br /> </td> 
   <td> IN<br /> </td> 
   <td> N/A<br /> </td> 
   <td> 第一個值必須包含第二個值。<br /> </td> 
   <td> <strong>@domain IN mail</strong>。在此處，結果將返回所有具有　'mail'　值的網域名稱。因此，'gmail.com'　網域名稱將構成傳回結果的一部分。<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">Like</span> <br /> </td> 
   <td> LIKE<br /> </td> 
   <td> N/A<br /> </td> 
   <td> <span class="uicontrol">Like</span> 與　<span class="uicontrol">Contains</span>　運算子非常類似。它可讓您在所搜尋的值中插入　<span class="uicontrol">%</span>　萬用字元。<br /> </td> 
   <td> <strong>@lastName LIKE Mart%n</strong>。在此處，替代字元 <strong>%</strong> (%)　作為　"joker"，在拼字不正確的假設情況下尋找名稱　"Martin"。<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">Not like</span> <br /> </td> 
   <td> NOT<br /> </td> 
   <td> N/A<br /> </td> 
   <td> 類似 <span class="uicontrol">Like</span>。它可讓您不復原輸入的值。在這裡，輸入的值也必須包含 <span class="uicontrol">%</span> 萬用字元。<br /> </td> 
   <td> <strong>@lastName NOT Smi%h</strong>。在這裡，與名稱　'Smi%h' （如　Smith　等）相對應的收件者不會被傳回為結果。<br /> </td> 
  </tr> 
  <tr> 
   <td> <span class="uicontrol">Is empty</span> <br /> </td> 
   <td> IS NULL<br /> </td> 
   <td> N/A<br /> </td> 
   <td> 第一個值必須對應至空值。<br /> </td> 
   <td> <strong>@mobilePhone IS NULL</strong> 會擷取所有尚未提供行動電話號碼的設定檔。<br /> </td> 
  </tr> 
 </tbody> 
</table>