---
layout: docs
title: 頁籤
description: 將內容分群管理的切換器。
group: components
---

## 關於頁籤

頁籤常用於將相關的內容分成比較小的區塊以方便切換閱讀的焦點區塊，頁籤的切換並不會將使用者帶往其他頁面，而是在同一頁面上切換內容面板上的不同資訊。

## 使用規範

### 何時該使用頁籤

當有多個類別的資訊，且分類方式不易再更動時，適合使用頁籤。名稱較短、可預測，性質相近且放在一起合乎邏輯時，適合使用頁籤。理想情況下，頁籤列表可以在同一列呈現，但我們也提供兩列的變形以供參考。（詳見[基本頁籤](/docs/components/tabs/#基本款頁籤-basic-tab)與[膠囊式頁籤](/docs/components/tabs/#膠囊式頁籤-pill-tab)）


### 何時該考慮使用其他元件

- **列表數量少於二。** 當頁籤列表的數量太少，甚至只有一項時，可以不用頁籤面板，而改以其它方式呈現，例如：文字標題 (title)。
- **列表數量大於九。** 當頁籤列表的數量大多，甚至超過九項時，可以不用頁籤面板，而改以其它方式呈現，例如：下拉選單 (dropdown)。

### 頁籤易用性

- **勿使用頁籤做為主要導覽。** 頁籤是頁內導覽用，請勿過度依賴頁籤作為導覽。
- **頁籤列表保持在一列內呈現最佳。** 當頁籤列表的數量多到超過版面空間，必須超出寬幅或到達第二列時，請優先重新檢視資訊架構，做適度的文字或項目刪減。
- **頁籤文字使用簡單明確的短名詞。** 文字請保持簡單、簡短，建議使用簡潔的短名詞，避免使用長文句以縮減文字長度。例如：「今日新聞」而非「點我看今日新聞」。一般來說建議字數儘量保持在四個字以內。
- **明確的區別選定頁籤 (selected tab) 與未選定頁籤 (unselected tab)。** 選定頁籤應明確的與未選定頁籤做區隔。
- **勿使用圖示 (icon) 替代文字。** 頁籤文字為必須存在的元素，請勿只用圖示代替。
- **使用圖示 (icon) 時請與文字意思配合。** 頁籤文字為必須存在的元素，一般不建議使用太多花俏的圖示使版面過於繁亂。若真的有幫助或必要的情況下，可用圖示來補充文字意涵，但請注意圖示與文字意涵應相互配合，且不同頁籤的圖示風格應儘量一致。
- **勿在頁籤中使用圖片。** 頁籤是頁內導覽用，請勿用整張圖片當作背景作為頁籤文字的替代。
- **請勿截斷文字。**
- **請記得檢視資訊架構。** Tab 數量太多無法在一列呈現時，請先檢視資訊架構。或是判斷使用者是否應該：
  - 一次看到所有 tab 的全部內容 
  - 優先與排序高的 tab 互動

### 頁籤近用性

網頁內容的所有功能應都能透過鍵盤介面來操作，請注意頁籤的切換應可以透過由鍵盤觸發的事件來操作。

## 元件設計

### 基本款頁籤 Basic tab

基本款的頁籤預設是有底線形式的頁籤。在這個元件中我們展示的是多個頁籤組成的頁籤列表，且數量較少（內容不超過一行）的情境。

頁籤在被 hover, select, disable 等狀態都有不同的樣式。您可以試圖將滑鼠移動到元件上，觀看效果。

頁籤寬度的設定預設為依文字長 (label-based) ，也就是說頁籤的寬度會依文字的長度變化。

{{< example >}}

<div class="row">
  <div class="col">
    <ul class="nav nav-tabs" id="tab" role="tablist">
      <li class="nav-item" role="presentation">
        <button class="nav-link active" id="tab1" data-bs-toggle="tab" data-bs-target="#content1" type="button" role="tab" aria-controls="tab1" aria-selected="true">頁籤 01</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="tab2" data-bs-toggle="tab" data-bs-target="#content2" type="button" role="tab" aria-controls="tab2" aria-selected="false">頁籤 02</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="tab3" data-bs-toggle="tab" data-bs-target="#content3" type="button" role="tab" aria-controls="tab3" aria-selected="false">頁籤 03</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="tab4" data-bs-toggle="tab" data-bs-target="#content4" type="button" role="tab" aria-controls="tab4" aria-selected="false">頁籤 04 寬度依文字長</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="tab5" data-bs-toggle="tab" data-bs-target="#content5" type="button" role="tab" aria-controls="tab5" aria-selected="false" disabled>頁籤 05</button>
      </li>
    </ul>
    <div class="tab-content" id="tabContent">
      <div class="tab-pane fade show active" id="content1" role="tabpanel" aria-labelledby="content1">頁籤 01 示範內容</div>
      <div class="tab-pane fade" id="content2" role="tabpanel" aria-labelledby="content2">頁籤 02 示範內容</div>
      <div class="tab-pane fade" id="content3" role="tabpanel" aria-labelledby="content3">頁籤 03 示範內容</div>
        <div class="tab-pane fade" id="content4" role="tabpanel" aria-labelledby="content4">頁籤 04 頁籤寬度的設定預設為依文字長 (label-based) ，也就是說頁籤的寬度會依文字的長度變化。</div>
        <div class="tab-pane fade" id="content5" role="tabpanel" aria-labelledby="content5">頁籤 05 示範內容</div>
    </div>
  </div>
</div>

{{< /example >}}

### 膠囊式頁籤 Pill tab

我們也提供另一種樣式選擇：膠囊式頁籤。與底線式頁籤不同的地方是它更適合於垂直方向的堆疊排列。當頁籤數量較多的情境，當頁籤列表必須排到第二行時，膠囊式頁籤會更爲適合。

{{< example >}}

<div class="row">
  <div class="col-6">
    <ul class="nav nav-pills" id="pills-tab" role="tablist">
      <li class="nav-item" role="presentation">
        <button class="nav-link active" id="pills-tab1" data-bs-toggle="pill" data-bs-target="#pills-content1" type="button" role="tab" aria-controls="pills-tab1" aria-selected="true">頁籤 01</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="pills-tab2" data-bs-toggle="pill" data-bs-target="#pills-content2" type="button" role="tab" aria-controls="pills-tab2" aria-selected="false">頁籤 02</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="pills-tab3" data-bs-toggle="pill" data-bs-target="#pills-content3" type="button" role="tab" aria-controls="pills-tab3" aria-selected="false">頁籤 03</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="pills-tab4" data-bs-toggle="pill" data-bs-target="#pills-content4" type="button" role="tab" aria-controls="pills-tab4" aria-selected="false">頁籤 04</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="pills-tab5" data-bs-toggle="pill" data-bs-target="#pills-content5" type="button" role="tab" aria-controls="pills-tab5" aria-selected="false">頁籤 05</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="pills-tab6" data-bs-toggle="pill" data-bs-target="#pills-content6" type="button" role="tab" aria-controls="pills-tab6" aria-selected="false">頁籤 06</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="pills-tab7" data-bs-toggle="pill" data-bs-target="#pills-content7" type="button" role="tab" aria-controls="pills-tab7" aria-selected="false">頁籤 07</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="pills-tab8" data-bs-toggle="pill" data-bs-target="#pills-content8" type="button" role="tab" aria-controls="pills-tab8" aria-selected="false" disabled>頁籤 08</button>
      </li>
    </ul>
    <div class="tab-content" id="pills-tabContent">
      <div class="tab-pane fade show active" id="pills-content1" role="tabpanel" aria-labelledby="pills-content1">頁籤 01 當頁籤數量較多的情境，當頁籤列表必須排到第二行時，膠囊式頁籤會更爲適合。</div>
      <div class="tab-pane fade" id="pills-content2" role="tabpanel" aria-labelledby="pills-content2">頁籤 02 示範內容</div>
      <div class="tab-pane fade" id="pills-content3" role="tabpanel" aria-labelledby="pills-content3">頁籤 03 示範內容</div>
      <div class="tab-pane fade" id="pills-content4" role="tabpanel" aria-labelledby="pills-content4">頁籤 04 示範內容</div>
      <div class="tab-pane fade" id="pills-content5" role="tabpanel" aria-labelledby="pills-content5">頁籤 05 示範內容</div>
      <div class="tab-pane fade" id="pills-content6" role="tabpanel" aria-labelledby="pills-content6">頁籤 06 當頁籤數量較多的情境，當頁籤列表必須排到第二行時，膠囊式頁籤會更爲適合。</div>
      <div class="tab-pane fade" id="pills-content7" role="tabpanel" aria-labelledby="pills-content7">頁籤 07 示範內容</div>
      <div class="tab-pane fade" id="pills-content8" role="tabpanel" aria-labelledby="pills-content8">頁籤 08 示範內容</div>
    </div>
  </div>
</div>

{{< /example >}}

### 依版面寬 Screen-based distribution

內容按照比例分配空間。相對於依文字長 (label-based) 為堆疊式 (stacked) ，依版面寬 (screen-based) 則為分佈式 (distributed)。值得注意的是，這種形式的空間配置方式會讓所有頁籤共同佔用所有的水平空間，但並不是每個頁籤都具有相同寬度。

{{< example >}}

<div class="row py-5">
  <div class="col">
    <ul class="nav nav-pills nav-fill" id="pills-tab-fill" role="tablist">
      <li class="nav-item" role="presentation">
        <button class="nav-link active" id="pills-tab1-fill" data-bs-toggle="pill" data-bs-target="#pills-content1-fill" type="button" role="tab" aria-controls="pills-tab1-fill" aria-selected="true">頁籤 01</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="pills-tab2-fill" data-bs-toggle="pill" data-bs-target="#pills-content2-fill" type="button" role="tab" aria-controls="pills-tab2-fill" aria-selected="false">頁籤 02 共同佔滿版面寬</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="pills-tab3-fill" data-bs-toggle="pill" data-bs-target="#pills-content3-fill" type="button" role="tab" aria-controls="pills-tab3-fill" aria-selected="false">頁籤 03 </button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="pills-tab4-fill" data-bs-toggle="pill" data-bs-target="#pills-content4-fill" type="button" role="tab" aria-controls="pills-tab4-fill" aria-selected="false">頁籤 04 </button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="pills-tab5-fill" data-bs-toggle="pill" data-bs-target="#pills-content5-fill" type="button" role="tab" aria-controls="pills-tab5-fill" aria-selected="false" disabled>頁籤 05</button>
      </li>
    </ul>
    <div class="tab-content" id="pills-tabContent-fill">
      <div class="tab-pane fade show active" id="pills-content1-fill" role="tabpanel" aria-labelledby="pills-content1-fill">頁籤 01 所有頁籤文字共同分享並佔滿所有的水平空間。</div>
      <div class="tab-pane fade" id="pills-content2-fill" role="tabpanel" aria-labelledby="pills-content2-fill">頁籤 02 示範內容</div>
      <div class="tab-pane fade" id="pills-content3-fill" role="tabpanel" aria-labelledby="pills-content3-fill">頁籤 03 示範內容</div>
      <div class="tab-pane fade" id="pills-content4-fill" role="tabpanel" aria-labelledby="pills-content4-fill">頁籤 04 示範內容</div>
      <div class="tab-pane fade" id="pills-content5-fill" role="tabpanel" aria-labelledby="pills-content5-fill">頁籤 05 示範內容</div>
    </div>
  </div>
</div>
<div class="row py-5">
  <div class="col">
    <ul class="nav nav-tabs nav-fill" id="tab-fill" role="tablist">
      <li class="nav-item" role="presentation">
        <button class="nav-link active" id="tab1-fill" data-bs-toggle="tab" data-bs-target="#content1-fill" type="button" role="tab" aria-controls="tab1-fill" aria-selected="true">頁籤 01</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="tab2-fill" data-bs-toggle="tab" data-bs-target="#content2-fill" type="button" role="tab" aria-controls="tab2-fill" aria-selected="false">頁籤 02 共同佔滿版面寬</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="tab3-fill" data-bs-toggle="tab" data-bs-target="#content3-fill" type="button" role="tab" aria-controls="tab3-fill" aria-selected="false">頁籤 03 </button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="tab4-fill" data-bs-toggle="tab" data-bs-target="#content4-fill" type="button" role="tab" aria-controls="tab4-fill" aria-selected="false">頁籤 04 </button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="tab5-fill" data-bs-toggle="tab" data-bs-target="#content5-fill" type="button" role="tab" aria-controls="tab5-fill" aria-selected="false" disabled>頁籤 05</button>
      </li>
    </ul>
    <div class="tab-content" id="tabContent-fill">
      <div class="tab-pane fade show active" id="content1-fill" role="tabpanel" aria-labelledby="content1-fill">頁籤項目01 所有頁籤文字共同分享並佔滿所有的水平空間。</div>
      <div class="tab-pane fade" id="content2-fill" role="tabpanel" aria-labelledby="content2-fill">頁籤項目02 示範內容</div>
      <div class="tab-pane fade" id="content3-fill" role="tabpanel" aria-labelledby="content3-fill">頁籤項目03 示範內容</div>
      <div class="tab-pane fade" id="content4-fill" role="tabpanel" aria-labelledby="content4-fill">頁籤項目04 示範內容</div>
      <div class="tab-pane fade" id="content5-fill" role="tabpanel" aria-labelledby="content5-fill">頁籤項目05 示範內容</div>
    </div>
  </div>
</div>

{{< /example >}}

### 頁籤帶圖示 Tab with icon

頁籤的文字前後可以加上簡單的圖示，方便使用者查找或瀏覽。

{{< example >}}

<div class="row py-5">
  <div class="col">
    <ul class="nav nav-pills" id="pills-tab-icon2" role="tablist">
      <li class="nav-item" role="presentation">
        <button class="nav-link active" id="pills-tab1-icon2" data-bs-toggle="pill" data-bs-target="#pills-content1-icon2" type="button" role="tab" aria-controls="pills-tab1-icon" aria-selected="true"><i class="bi bi-house-door"></i><span>頁籤 01</span></button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="pills-tab2-ico2" data-bs-toggle="pill" data-bs-target="#pills-content2-icon2" type="button" role="tab" aria-controls="pills-tab2-icon2" aria-selected="false"><i class="bi bi-inbox"></i><span>頁籤 02</span></button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="pills-tab3-icon2" data-bs-toggle="pill" data-bs-target="#pills-content3-icon2" type="button" role="tab" aria-controls="pills-tab3-icon2" aria-selected="false"><i class="bi bi-info-circle"></i><span>頁籤 03</span></button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="pills-tab4-icon2" data-bs-toggle="pill" data-bs-target="#pills-content4-icon2" type="button" role="tab" aria-controls="pills-tab4-icon2" aria-selected="false"><i class="bi bi-joystick"></i><span>頁籤 04</span></button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="pills-tab5-icon2" data-bs-toggle="pill" data-bs-target="#pills-content5-icon2" type="button" role="tab" aria-controls="pills-tab5-icon2" aria-selected="false" disabled><i class="bi bi-journal-arrow-down"></i><span>頁籤 05</span></button>
      </li>
    </ul>
    <div class="tab-content" id="pills-tabContent-icon2">
      <div class="tab-pane fade show active" id="pills-content1-icon2" role="tabpanel" aria-labelledby="pills-content1-icon2"> 頁籤 01 頁籤的文字前可以加上 Icon</div>
      <div class="tab-pane fade" id="pills-content2-icon2" role="tabpanel" aria-labelledby="pills-content2-icon2">頁籤 02 示範內容</div>
      <div class="tab-pane fade" id="pills-content3-icon2" role="tabpanel" aria-labelledby="pills-content3-icon2">頁籤 03 示範內容</div>
      <div class="tab-pane fade" id="pills-content4-icon2" role="tabpanel" aria-labelledby="pills-content4-icon2">頁籤 04 示範內容</div>
      <div class="tab-pane fade" id="pills-content5-icon2" role="tabpanel" aria-labelledby="pills-content5-icon2">頁籤 05 示範內容</div>
    </div>
  </div>
</div>
<div class="row py-5">
  <div class="col">
    <ul class="nav nav-tabs" id="tab-icon" role="tablist">
      <li class="nav-item" role="presentation">
        <button class="nav-link active" id="tab1-icon" data-bs-toggle="tab" data-bs-target="#content1-icon" type="button" role="tab" aria-controls="tab1-icon" aria-selected="true"><i class="bi bi-house-door"></i><span>頁籤 01</span></button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="tab2-icon" data-bs-toggle="tab" data-bs-target="#content2-icon" type="button" role="tab" aria-controls="tab2-icon" aria-selected="false"><i class="bi bi-inbox"></i><span>頁籤 02</span></button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="tab3-icon" data-bs-toggle="tab" data-bs-target="#content3-icon" type="button" role="tab" aria-controls="tab3-icon" aria-selected="false"><i class="bi bi-info-circle"></i><span>頁籤 03</span></button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="tab4-icon" data-bs-toggle="tab" data-bs-target="#content4-icon" type="button" role="tab" aria-controls="tab4-icon" aria-selected="false"><i class="bi bi-joystick"></i><span>頁籤 04</span></button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="tab5-icon" data-bs-toggle="tab" data-bs-target="#content5-icon" type="button" role="tab" aria-controls="tab5-icon" aria-selected="false" disabled><i class="bi bi-journal-arrow-down"></i><span>頁籤 05</span></button>
      </li>
    </ul>
    <div class="tab-content" id="tabContent-icon">
      <div class="tab-pane fade show active" id="content1-icon" role="tabpanel" aria-labelledby="content1-icon">頁籤 01 頁籤的文字前可以加上 Icon</div>
      <div class="tab-pane fade" id="content2-icon" role="tabpanel" aria-labelledby="content2-icon">頁籤 02 示範內容</div>
      <div class="tab-pane fade" id="content3-icon" role="tabpanel" aria-labelledby="content3-icon">頁籤 03 示範內容</div>
      <div class="tab-pane fade" id="content4-icon" role="tabpanel" aria-labelledby="content4-icon">頁籤 04 示範內容</div>
      <div class="tab-pane fade" id="content5-icon" role="tabpanel" aria-labelledby="content5-icon">頁籤 05 示範內容</div>
    </div>
  </div>
</div>
 <div class="row py-5">
  <div class="col">
    <ul class="nav nav-pills" id="pills-tab-icon" role="tablist">
      <li class="nav-item" role="presentation">
        <button class="nav-link active" id="pills-tab1-icon" data-bs-toggle="pill" data-bs-target="#pills-content1-icon" type="button" role="tab" aria-controls="pills-tab1-icon" aria-selected="true"><span>頁籤 01</span><i class="bi bi-house-door"></i></button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="pills-tab2-icon" data-bs-toggle="pill" data-bs-target="#pills-content2-icon" type="button" role="tab" aria-controls="pills-tab2-icon" aria-selected="false"><span>頁籤 02</span><i class="bi bi-inbox"></i></button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="pills-tab3-icon" data-bs-toggle="pill" data-bs-target="#pills-content3-icon" type="button" role="tab" aria-controls="pills-tab3-icon" aria-selected="false"><span>頁籤 03</span><i class="bi bi-info-circle"></i></button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="pills-tab4-icon" data-bs-toggle="pill" data-bs-target="#pills-content4-icon" type="button" role="tab" aria-controls="pills-tab4-icon" aria-selected="false"><span>頁籤 04</span><i class="bi bi-joystick"></i></button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="pills-tab5-icon" data-bs-toggle="pill" data-bs-target="#pills-content5-icon" type="button" role="tab" aria-controls="pills-tab5-icon" aria-selected="false" disabled><span>頁籤 05</span><i class="bi bi-journal-arrow-down"></i></button>
      </li>
    </ul>
    <div class="tab-content" id="pills-tabContent-icon">
      <div class="tab-pane fade show active" id="pills-content1-icon" role="tabpanel" aria-labelledby="pills-content1-icon">頁籤 01 頁籤的文字後可以加上 Icon</div>
      <div class="tab-pane fade" id="pills-content2-icon" role="tabpanel" aria-labelledby="pills-content2-icon">頁籤 02 示範內容</div>
      <div class="tab-pane fade" id="pills-content3-icon" role="tabpanel" aria-labelledby="pills-content3-icon">頁籤 03 示範內容</div>
      <div class="tab-pane fade" id="pills-content4-icon" role="tabpanel" aria-labelledby="pills-content4-icon">頁籤 04 示範內容</div>
      <div class="tab-pane fade" id="pills-content5-icon" role="tabpanel" aria-labelledby="pills-content5-icon">頁籤 05 示範內容</div>
    </div>
  </div>
</div>
<div class="row py-5">
  <div class="col">
    <ul class="nav nav-tabs" id="tab-icon" role="tablist">
      <li class="nav-item" role="presentation">
        <button class="nav-link active" id="tab1-icon2" data-bs-toggle="tab" data-bs-target="#content1-icon2" type="button" role="tab" aria-controls="tab1-icon2" aria-selected="true"><span>頁籤 01</span><i class="bi bi-house-door"></i></button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="tab2-icon2" data-bs-toggle="tab" data-bs-target="#content2-icon2" type="button" role="tab" aria-controls="tab2-icon2" aria-selected="false"><span>頁籤 02</span><i class="bi bi-inbox"></i></button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="tab3-icon2" data-bs-toggle="tab" data-bs-target="#content3-icon2" type="button" role="tab" aria-controls="tab3-icon2" aria-selected="false"><span>頁籤 03</span><i class="bi bi-info-circle"></i></button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="tab4-icon2" data-bs-toggle="tab" data-bs-target="#content4-icon2" type="button" role="tab" aria-controls="tab4-icon2" aria-selected="false"><span>頁籤 04</span><i class="bi bi-joystick"></i></button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="tab5-icon2" data-bs-toggle="tab" data-bs-target="#content5-icon2" type="button" role="tab" aria-controls="tab5-icon2" aria-selected="false" disabled><span>頁籤 05</span><i class="bi bi-journal-arrow-down"></i></button>
      </li>
    </ul>
    <div class="tab-content" id="tabContent-icon">
      <div class="tab-pane fade show active" id="content1-icon2" role="tabpanel" aria-labelledby="content1-icon2">頁籤 01 頁籤的文字後可以加上 Icon </div>
      <div class="tab-pane fade" id="content2-icon2" role="tabpanel" aria-labelledby="content2-icon2">頁籤 02 示範內容</div>
      <div class="tab-pane fade" id="content3-icon2" role="tabpanel" aria-labelledby="content3-icon2">頁籤 03 示範內容</div>
      <div class="tab-pane fade" id="content4-icon2" role="tabpanel" aria-labelledby="content4-icon2">頁籤 04 示範內容</div>
      <div class="tab-pane fade" id="content5-icon2" role="tabpanel" aria-labelledby="content5-icon2">頁籤 05 示範內容</div>
    </div>
  </div>
</div>

{{< /example >}}

### 滾動式頁籤列表與堆疊式頁籤列表 Scrollable tabs and stackable tabs
當頁籤列表內容較多時，除了垂直堆疊，也可以用滾動式的頁籤列表。兩者各有優缺點：

- 堆疊式頁籤列表：使用者能夠一次看見所有的頁籤標題，頁籤數量也可以比較有機的增加。但若資訊太多，整體視覺可能比較雜亂。
- 滾動式頁籤列表：視覺較為美觀，重要的資訊顯示，次要的資訊則收納起來。但使用者可能會在因為在一開始看不到某幾個頁籤標題，找不到對的資訊而迷航。

{{< example >}}

<div class="row py-5">
  <div class="col-9">
    <div class="nav-scroll">
      <button type="button" class="btn btn-less-important" onclick="Prev(this)"><i class="bi bi-chevron-left"></i></button>
      <div class="nav-scroll-wrapper">
        <ul class="nav nav-tabs" role="tablist">
          <li class="nav-item" role="presentation">
            <button class="nav-link active" id="scroll-tab1" data-bs-toggle="tab" data-bs-target="#scroll-content1" type="button" role="tab" aria-controls="scroll-content1" aria-selected="true">頁籤 01</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-tab2" data-bs-toggle="tab" data-bs-target="#scroll-content2" type="button" role="tab" aria-controls="scroll-content2" aria-selected="false">頁籤 02</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-tab3" data-bs-toggle="tab" data-bs-target="#scroll-content3" type="button" role="tab" aria-controls="scroll-content3" aria-selected="false">頁籤 03</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-tab4" data-bs-toggle="tab" data-bs-target="#scroll-content4" type="button" role="tab" aria-controls="scroll-content4" aria-selected="false">頁籤 04</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-tab5" data-bs-toggle="tab" data-bs-target="#scroll-content5" type="button" role="tab" aria-controls="scroll-content5" aria-selected="false">頁籤 05</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-tab6" data-bs-toggle="tab" data-bs-target="#scroll-content6" type="button" role="tab" aria-controls="scroll-content6" aria-selected="false">頁籤 06</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-tab7" data-bs-toggle="tab" data-bs-target="#scroll-content7" type="button" role="tab" aria-controls="scroll-content7" aria-selected="false">頁籤 07</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-tab8" data-bs-toggle="tab" data-bs-target="#scroll-content8" type="button" role="tab" aria-controls="scroll-content8" aria-selected="false">頁籤 08</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-tab9" data-bs-toggle="tab" data-bs-target="#scroll-content9" type="button" role="tab" aria-controls="scroll-content9" aria-selected="false">頁籤 09</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-tab10" data-bs-toggle="tab" data-bs-target="#scroll-content10" type="button" role="tab" aria-controls="scroll-content10" aria-selected="false">頁籤 10</button>
          </li>
        </ul>
      </div>
      <button class="btn btn-less-important" onclick="Next(this)"><i class="bi bi-chevron-right"></i></button>
    </div>
    <div class="tab-content" id="tabContent-scrollable">
      <div class="tab-pane fade show active" id="scroll-content1" role="tabpanel" aria-labelledby="scroll-tab1">頁籤 01 滾動式頁籤列表展示，點擊左右方向符號做橫向滾動瀏覽。</div>
      <div class="tab-pane fade" id="scroll-content2" role="tabpanel" aria-labelledby="scroll-tab2">頁籤 02 示範內容</div>
      <div class="tab-pane fade" id="scroll-content3" role="tabpanel" aria-labelledby="scroll-tab3">頁籤 03 示範內容</div>
      <div class="tab-pane fade" id="scroll-content4" role="tabpanel" aria-labelledby="scroll-tab4">頁籤 04 示範內容</div>
      <div class="tab-pane fade" id="scroll-content5" role="tabpanel" aria-labelledby="scroll-tab5">頁籤 05 示範內容</div>
      <div class="tab-pane fade" id="scroll-content6" role="tabpanel" aria-labelledby="scroll-tab6">頁籤 06 示範內容</div>
      <div class="tab-pane fade" id="scroll-content7" role="tabpanel" aria-labelledby="scroll-tab7">頁籤 07 示範內容</div>
      <div class="tab-pane fade" id="scroll-content8" role="tabpanel" aria-labelledby="scroll-tab8">頁籤 08 示範內容</div>
      <div class="tab-pane fade" id="scroll-content9" role="tabpanel" aria-labelledby="scroll-tab9">頁籤 09 示範內容</div>
      <div class="tab-pane fade" id="scroll-content10" role="tabpanel" aria-labelledby="scroll-tab10">頁籤 10 示範內容</div>
    </div>
  </div>
</div>
<div class="row py-5">
  <div class="col-9">
    <div class="nav-scroll">
      <button type="button" class="btn btn-less-important" onclick="Prev(this)"><i class="bi bi-chevron-left"></i></button>
      <div class="nav-scroll-wrapper">
        <ul class="nav nav-pills" role="tablist">
          <li class="nav-item" role="presentation">
            <button class="nav-link active" id="scroll-pills-tab1" data-bs-toggle="pill" data-bs-target="#scroll-pills-content1" type="button" role="tab" aria-controls="scroll-pills-content1" aria-selected="true">頁籤 01</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-pills-tab2" data-bs-toggle="pill" data-bs-target="#scroll-pills-content2" type="button" role="tab" aria-controls="scroll-pills-content2" aria-selected="false">頁籤 02</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-pills-tab3" data-bs-toggle="pill" data-bs-target="#scroll-pills-content3" type="button" role="tab" aria-controls="scroll-pills-content3" aria-selected="false">頁籤 03</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-pills-tab4" data-bs-toggle="pill" data-bs-target="#scroll-pills-content4" type="button" role="tab" aria-controls="scroll-pills-content4" aria-selected="false">頁籤 04</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-pills-tab5" data-bs-toggle="pill" data-bs-target="#scroll-pills-content5" type="button" role="tab" aria-controls="scroll-pills-content5" aria-selected="false">頁籤 05</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-pills-tab6" data-bs-toggle="pill" data-bs-target="#scroll-pills-content6" type="button" role="tab" aria-controls="scroll-pills-content6" aria-selected="false">頁籤 06</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-pills-tab7" data-bs-toggle="pill" data-bs-target="#scroll-pills-content7" type="button" role="tab" aria-controls="scroll-pills-content7" aria-selected="false">頁籤 07</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-pills-tab8" data-bs-toggle="pill" data-bs-target="#scroll-pills-content8" type="button" role="tab" aria-controls="scroll-pills-content8" aria-selected="false">頁籤 08</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-pills-tab9" data-bs-toggle="pill" data-bs-target="#scroll-pills-content9" type="button" role="tab" aria-controls="scroll-pills-content9" aria-selected="false">頁籤 09</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-pills-tab10" data-bs-toggle="pill" data-bs-target="#scroll-pills-content10" type="button" role="tab" aria-controls="scroll-pills-content10" aria-selected="false">頁籤 10</button>
          </li>
        </ul>
      </div>
      <button class="btn btn-less-important" onclick="Next(this)"><i class="bi bi-chevron-right"></i></button>
    </div>
    <div class="tab-content" id="tabContent-scrollable">
      <div class="tab-pane fade show active" id="scroll-pills-content1" role="tabpanel" aria-labelledby="scroll-pills-tab1">頁籤 01 滾動式頁籤列表展示，點擊左右方向符號做橫向滾動瀏覽。</div>
      <div class="tab-pane fade" id="scroll-pills-content2" role="tabpanel" aria-labelledby="scroll-pills-tab2">頁籤 02 示範內容</div>
      <div class="tab-pane fade" id="scroll-pills-content3" role="tabpanel" aria-labelledby="scroll-pills-tab3">頁籤 03 示範內容</div>
      <div class="tab-pane fade" id="scroll-pills-content4" role="tabpanel" aria-labelledby="scroll-pills-tab4">頁籤 04 示範內容</div>
      <div class="tab-pane fade" id="scroll-pills-content5" role="tabpanel" aria-labelledby="scroll-pills-tab5">頁籤 05 示範內容</div>
      <div class="tab-pane fade" id="scroll-pills-content6" role="tabpanel" aria-labelledby="scroll-pills-tab6">頁籤 06 示範內容</div>
      <div class="tab-pane fade" id="scroll-pills-content7" role="tabpanel" aria-labelledby="scroll-pills-tab7">頁籤 07 示範內容</div>
      <div class="tab-pane fade" id="scroll-pills-content8" role="tabpanel" aria-labelledby="scroll-pills-tab8">頁籤 08 示範內容</div>
      <div class="tab-pane fade" id="scroll-pills-content9" role="tabpanel" aria-labelledby="scroll-pills-tab9">頁籤 09 示範內容</div>
      <div class="tab-pane fade" id="scroll-pills-content10" role="tabpanel" aria-labelledby="scroll-pills-tab10">頁籤 10 示範內容</div>
    </div>
  </div>
</div>
<div class="row py-5">
  <div class="col-9">
    <ul class="nav nav-tabs" id="brick-tab" role="tablist">
      <li class="nav-item" role="presentation">
        <button class="nav-link active" id="brick-tab1" data-bs-toggle="tab" data-bs-target="#brick-tab-content1" type="button" role="tab" aria-controls="brick-content1" aria-selected="true">頁籤 01</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-tab2" data-bs-toggle="tab" data-bs-target="#brick-content2" type="button" role="tab" aria-controls="brick-content2" aria-selected="false">頁籤 02</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-tab3" data-bs-toggle="tab" data-bs-target="#brick-content3" type="button" role="tab" aria-controls="brick-content3" aria-selected="false">頁籤 03</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-tab4" data-bs-toggle="tab" data-bs-target="#brick-content4" type="button" role="tab" aria-controls="brick-content4" aria-selected="false">頁籤 04</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-tab5" data-bs-toggle="tab" data-bs-target="#brick-content5" type="button" role="tab" aria-controls="brick-content5" aria-selected="false">頁籤 05</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-tab6" data-bs-toggle="tab" data-bs-target="#brick-content6" type="button" role="tab" aria-controls="brick-content6" aria-selected="false">頁籤 06</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-tab7" data-bs-toggle="tab" data-bs-target="#brick-content7" type="button" role="tab" aria-controls="brick-content7" aria-selected="false">頁籤 07</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-tab8" data-bs-toggle="tab" data-bs-target="#brick-content8" type="button" role="tab" aria-controls="brick-content8" aria-selected="false">頁籤 08</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-tab9" data-bs-toggle="tab" data-bs-target="#brick-content9" type="button" role="tab" aria-controls="brick-content9" aria-selected="false">頁籤 09</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-tab10" data-bs-toggle="tab" data-bs-target="#brick-content10" type="button" role="tab" aria-controls="brick-content10" aria-selected="false">頁籤 10</button>
      </li>
    </ul>
    <div class="tab-content" id="brick-tabContent">
      <div class="tab-pane fade show active" id="brick-content1" role="tabpanel" aria-labelledby="brick-content1">頁籤 01 堆疊式頁籤列表展示，一次看見所有的頁籤標題。</div>
      <div class="tab-pane fade" id="brick-content2" role="tabpanel" aria-labelledby="brick-content2">頁籤 02 示範內容</div>
      <div class="tab-pane fade" id="brick-content3" role="tabpanel" aria-labelledby="brick-content3">頁籤 03 示範內容</div>
      <div class="tab-pane fade" id="brick-content4" role="tabpanel" aria-labelledby="brick-content4">頁籤 04 示範內容</div>
      <div class="tab-pane fade" id="brick-content5" role="tabpanel" aria-labelledby="brick-content5">頁籤 05 示範內容</div>
      <div class="tab-pane fade" id="brick-content6" role="tabpanel" aria-labelledby="brick-content6">頁籤 06 示範內容</div>
      <div class="tab-pane fade" id="brick-content7" role="tabpanel" aria-labelledby="brick-content7">頁籤 07 示範內容</div>
      <div class="tab-pane fade" id="brick-content8" role="tabpanel" aria-labelledby="brick-content8">頁籤 08 示範內容</div>
      <div class="tab-pane fade" id="brick-content9" role="tabpanel" aria-labelledby="brick-content9">頁籤 09 示範內容</div>
      <div class="tab-pane fade" id="brick-content10" role="tabpanel" aria-labelledby="brick-content10">頁籤 10 示範內容</div>
    </div>
  </div>
</div>
<div class="row py-5">
  <div class="col-9">
    <ul class="nav nav-pills" id="brick-pills-tab" role="tablist">
      <li class="nav-item" role="presentation">
        <button class="nav-link active" id="brick-pills-tab1" data-bs-toggle="pill" data-bs-target="#brick-pills-content1" type="button" role="tab" aria-controls="brick-pills-content1" aria-selected="true">頁籤 01</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-pills-tab2" data-bs-toggle="pill" data-bs-target="#brick-pills-content2" type="button" role="tab" aria-controls="brick-pills-content2" aria-selected="false">頁籤 02</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-pills-tab3" data-bs-toggle="pill" data-bs-target="#brick-pills-content3" type="button" role="tab" aria-controls="brick-pills-content3" aria-selected="false">頁籤 03</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-pills-tab4" data-bs-toggle="pill" data-bs-target="#brick-pills-content4" type="button" role="tab" aria-controls="brick-pills-content4" aria-selected="false">頁籤 04</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-pills-tab5" data-bs-toggle="pill" data-bs-target="#brick-pills-content5" type="button" role="tab" aria-controls="brick-pills-content5" aria-selected="false">頁籤 05</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-pills-tab6" data-bs-toggle="pill" data-bs-target="#brick-pills-content6" type="button" role="tab" aria-controls="brick-pills-content6" aria-selected="false">頁籤 06</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-pills-tab7" data-bs-toggle="pill" data-bs-target="#brick-pills-content7" type="button" role="tab" aria-controls="brick-pills-content7" aria-selected="false">頁籤 07</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-pills-tab8" data-bs-toggle="pill" data-bs-target="#brick-pills-content8" type="button" role="tab" aria-controls="brick-pills-content8" aria-selected="false">頁籤 08</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-pills-tab9" data-bs-toggle="pill" data-bs-target="#brick-pills-content9" type="button" role="tab" aria-controls="brick-pills-content9" aria-selected="false">頁籤 09</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-pills-tab10" data-bs-toggle="pill" data-bs-target="#brick-pills-content10" type="button" role="tab" aria-controls="brick-pills-content10" aria-selected="false">頁籤 10</button>
      </li>
    </ul>
    <div class="tab-content" id="brick-pills-tabContent">
      <div class="tab-pane fade show active" id="brick-pills-content1" role="tabpanel" aria-labelledby="brick-pills-content1">頁籤 01 堆疊式頁籤列表展示，一次看見所有的頁籤標題。</div>
      <div class="tab-pane fade" id="brick-pills-content2" role="tabpanel" aria-labelledby="brick-pills-content2">頁籤 02 示範內容</div>
      <div class="tab-pane fade" id="brick-pills-content3" role="tabpanel" aria-labelledby="brick-pills-content3">頁籤 03 示範內容</div>
      <div class="tab-pane fade" id="brick-pills-content4" role="tabpanel" aria-labelledby="brick-pills-content4">頁籤 04 示範內容</div>
      <div class="tab-pane fade" id="brick-pills-content5" role="tabpanel" aria-labelledby="brick-pills-content5">頁籤 05 示範內容</div>
      <div class="tab-pane fade" id="brick-pills-content6" role="tabpanel" aria-labelledby="brick-pills-content6">頁籤 06 示範內容</div>
      <div class="tab-pane fade" id="brick-pills-content7" role="tabpanel" aria-labelledby="brick-pills-content7">頁籤 07 示範內容</div>
      <div class="tab-pane fade" id="brick-pills-content8" role="tabpanel" aria-labelledby="brick-pills-content8">頁籤 08 示範內容</div>
      <div class="tab-pane fade" id="brick-pills-content9" role="tabpanel" aria-labelledby="brick-pills-content9">頁籤 09 示範內容</div>
      <div class="tab-pane fade" id="brick-pills-content10" role="tabpanel" aria-labelledby="brick-pills-content10">頁籤 10 示範內容</div>
    </div>
  </div>
</div>

<script>
window.onload = () => {
  for (var wrapper of document.querySelectorAll(".nav-scroll-wrapper")) {
    if (!("translate" in wrapper.dataset)) {
      wrapper.parentElement.querySelector("button").disabled = true
    }
  }
}

const Prev = (e) => {
  ([...e.parentElement.querySelectorAll("button")].pop()).disabled = false
  const scrollWrapper = e.parentElement.querySelector(".nav-scroll-wrapper");
  const scrollContainer = e.parentElement.querySelector(".nav");
  let translateDistance = "translate" in scrollWrapper.dataset ? parseInt(scrollWrapper.dataset.translate) : 0;
  translateDistance += scrollContainer.offsetWidth % scrollWrapper.offsetWidth;
  if (translateDistance <= 0 ) {
    scrollContainer.style.transform = `translate(${translateDistance}px)`;
    scrollWrapper.dataset.translate = translateDistance;
    scrollContainer.style.transition = "all 1s";
  } else {
    scrollContainer.style.transform = "translate(0px)";
    scrollWrapper.dataset.translate = 0;
    scrollContainer.style.transition = "all 1s";
  }

  if (translateDistance >= 0) {
    e.disabled = true
  }
}

const Next = (e) => {
  (e.parentElement.querySelector("button")).disabled = false
  const scrollWrapper = e.parentElement.querySelector(".nav-scroll-wrapper");
  const scrollContainer = e.parentElement.querySelector(".nav");

  let translateDistance = "translate" in scrollWrapper.dataset ? parseInt(scrollWrapper.dataset.translate) : 0;
  translateDistance -= scrollContainer.offsetWidth % scrollWrapper.offsetWidth;
  const widthGap = scrollWrapper.offsetWidth - scrollContainer.offsetWidth;
  if (translateDistance >= widthGap) {
    scrollContainer.style.transform = `translate(${translateDistance}px)`;
    scrollWrapper.dataset.translate = translateDistance;
    scrollContainer.style.transition = "all 1s";
  } else {
    scrollContainer.style.transform = `translate(${widthGap}px)`;
    scrollWrapper.dataset.translate = widthGap;
    scrollContainer.style.transition = "all 1s";
  }
  
  if (translateDistance < 0) {
    e.disabled = true
  }
}
</script>

{{< /example >}}

