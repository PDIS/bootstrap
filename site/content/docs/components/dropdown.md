---
layout: docs
title: 導覽列下拉選單 Navigation Dropdowns
description: 讓使用者從多個頁面選項中做一個或選擇，並跳轉到其選擇的頁面。
group: components
toc: true
---

### 關於導覽列下拉選單

導覽列的下拉選單是導覽的延伸。與常駐的導覽列不同，導覽列下拉選單是短暫的存在，依據使用者的互動輸入，觸發展開選單內容，並可以再次出發收納選單內容。使用者在選單展開時，可以從多個選項中做出單一選擇，選擇的目的是用來前往別的分頁。到達新的分頁後，下拉選單則自動收納起來，整個網頁回到原導覽列的常駐狀態。

### Guidance

#### When to use the select component

當導覽列有需要用到下拉式選單收納頁面連結，總數量不至於過多且層級（不含導覽列）不超過兩層時，請妥善利用導覽列下拉選單。

#### When to consider something else

- **選項過少。** 當連結數目不多，例如小於 3，且導覽列空間足夠時，建議直接將連結展開放置在導覽列上，供使用者一目了然的瀏覽並選擇想要前往的頁面。
- **選項過多。** 當選單內的項目太多，例如超過 15 項時，請先主動重新檢視網站的資訊架構。若無法更動，請參考 sidebar 搭配 header navigation 的呈現方式，避免用單一導覽列下拉選單一次收納過多資訊。否則，將過多內容收納在一處將會增加使用者的查找負擔。
- **選單數目過多。** 當導覽列上的導覽列下拉選單數量過多，甚至導覽列上每個連結都是用下拉選單呈現時，請參考 sidebar 搭配 header navigation 的呈現方式。

#### Usability

- **導覽列與下拉選單風格應一致。** 導覽列與其下拉選單皆為導覽用，其風格應一致，幫助使用者的潛在認知，降低額外學習成本。
- **導覽列與下拉選單底色區別。** 建議在導覽列的底色與下拉選單的底色使用不同顏色以作區別。因為下拉選單是暫時出現且蓋過背後網頁內容的元件，與常駐的導覽列顏色稍作區別，能幫助使用者在瀏覽網頁時的潛在認知。
- **避免不要的特效。** 下拉選單的內容可以直接覆蓋在原網頁的內容之上，請避免另外製作非必要的特效，例如逐項展開選單，或將網頁內容下推等。
- **避免選項數量過多。** 建議不要放超過 15 個選擇。

#### Accessbility

- **避免使用 hover 。** 請避免用 hover 觸發展開選單，儘量使用 click 觸發，以減少視覺負擔。

### Component

#### 滿版

當第二層級項目多 (> 7) 時，意即選單內容項目較多，適合使用滿版的形式將所有項目列出。同樣情況，當還有次層級時，滿版形式的導覽列下拉式選單也適用，可以再將次層級的項目也逐一列出。惟當次層級的項目也過多時，請重新檢視資訊架構，或考慮轉用 sidebar 搭配 header navigation 的呈現方式。

{{< example >}}

<div class="dropdown">
  <button class="dropdown-btn" type="button" id="dropdownMenuButton1" data-bs-toggle="dropdown" aria-expanded="false">
    服務項目名稱
  </button>
  <ul class="dropdown-menu" aria-labelledby="dropdownMenuButton1">
    <li><a class="dropdown-item" href="#">服務項目子項目</a></li>
    <li><a class="dropdown-item" href="#">寬度隨最長的內容文字調整</a></li>
    <li><a class="dropdown-item" href="#">服務項目子項目</a></li>
    <li><a class="dropdown-item" href="#">服務項目子項目</a></li>
    <li><a class="dropdown-item" href="#">服務項目子項目</a></li>
  </ul>
</div>

{{< /example >}}

#### 單欄式下拉

當第二層級項目少 (< 7) 時，意即選單內容項目較少，適合使用單欄式下拉的形式將所有項目列出。同樣情況，當次層級項目少 (<7) 時，點選箭頭圖標展開次層級選單。若次層級項目較多時，請重新檢視資訊架構，並考慮轉用 sidebar 搭配 header navigation 的呈現方式。
