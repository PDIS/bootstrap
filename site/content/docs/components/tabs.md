---
layout: docs
title: 頁籤面板 Tabs
description: 一種將網頁內容分群管理的容器
group: components
---

### 關於頁籤面板元件

頁籤面板 (tabs) 常用於將相關的內容分成比較小的區塊以方便切換閱讀的焦點區塊，頁籤的切換並不會將使用者待到其他頁面，而是在同一頁面上切換內容面板上的不同資訊。頁籤面板含有三個元素：頁籤 (tab)、頁籤列表 (tab list)、與內容面板 (content panel)。每個頁籤上的文字為頁籤文字 (tab label)。

<img class="img-fluid" src="/docs/5.1/assets/img/tabs.png" >

預設上，頁籤列表中會有一個選項預設為選定頁籤 (selected tab) ，列表中的其他選項則為未選定頁籤 (unselected tabs)。

### 使用規範

#### 何時該使用頁籤面板

當有 2~9 個類別的資訊，且分類方式不易再更動。名稱較短、可預測，性質相近且放在起合乎邏輯時。特別是當類別名稱試放在頁籤面板上時，所有類別標籤可以寫在同一行。

#### 何時該考慮使用其他元件

- **列表數量少於二。** 當頁籤列表的數量只有一項時，可以不用頁籤面板，而改以其它方式呈現，例如：文字標題 (title)。
- **列表數量大於九。** 當頁籤列表的數量超過九項時，可以不用頁籤面板，而改以其它方式呈現，例如：下拉式選單 (dropdown)。

#### 頁籤面板易用性

- **勿使用頁籤做為主要導覽。** 頁籤是頁內導覽用，請勿過度依賴頁籤作為導覽。
- **列表行數保持在一行內最佳。** 當頁籤列表的數量多到超過版面空間，必須超出寬幅或到達第二行時，請優先重新檢視資訊架構，做適度的文字或項目刪減。
- **頁籤文字使用簡單明確的短名詞。** 文字請保持簡單、簡短，建議使用簡潔的短名詞，避免使用長文句以縮減文字長度。例如：「今日新聞」而非「點我看今日新聞」。建議字數儘量保持在四個字以內。
- **明確的區別選定頁籤 (selected tab) 與未選定頁籤 (unselected tab)。** 選定頁籤應明確的與未選定頁籤做區隔。
- **勿使用圖標 (icon) 替代文字。** 頁籤文字為必須存在的元素，請勿僅用圖標代替。
- **使用圖標 (icon) 時請與文字意思配合。** 頁籤文字為必須存在的元素，一般不建議使用太多花俏的圖標使版面過於繁亂。若真的有幫助或必要的情況下，可用圖標來補充文字意涵，但請注意圖標與文字意涵應相互配合。
- **勿使用圖片在頁籤中。** 頁籤是頁內導覽用，請勿用整張圖當作背景作為頁籤文字的替代。
- **請勿截斷文字。**
- **請先檢視資訊架構。** Tab 數量太多時一行塞不下，請先檢視資訊架構，決定使用者是否應可：
  - 一次看到所有 tab 的全部內容
  - 優先與排序高的 tab 互動

#### 頁籤面板近用性

- **符合指引五(鍵盤可操作)：讓所有的功能都能透過鍵盤使用。** 5.1（檢測等級 A）內容的所有功能都能透過鍵盤介面來操作，而且不能額外要求在限定時間內完成按鍵操作。特殊目的的網頁(例如遊戲網頁要求在特定時間內完成指定操作)不在此限。
- 相關稽核評量碼
  - EV1050100：提供由鍵盤觸發的事件處理程式
  - EV1050101：確認所有功能都能透過鍵盤介面來操作

### 設計元件

#### 基本款 頁籤式 (tab) vs 膠囊狀頁籤 (pill)

基本款的頁籤面板包含頁籤、頁籤列表與內容面板。您也可以使用膠囊狀頁籤的變形。在這個元件中我們展示的是頁籤列表數量較少（內容不超過一行）的情境。頁籤寬度的設定預設為依文字長 (label-based) ，頁籤的寬度可以依文字長度改變。

{{< example >}}

<div class="row">
  <div class="col-12">
    <ul class="nav nav-tabs" id="tab" role="tablist">
      <li class="nav-item" role="presentation">
        <button class="nav-link active" id="tab1" data-bs-toggle="tab" data-bs-target="#content1" type="button" role="tab" aria-controls="tab1" aria-selected="true">頁籤項目</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="tab2" data-bs-toggle="tab" data-bs-target="#content2" type="button" role="tab" aria-controls="tab2" aria-selected="false">頁籤項目</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="tab3" data-bs-toggle="tab" data-bs-target="#content3" type="button" role="tab" aria-controls="tab3" aria-selected="false">頁籤項目</button>
      </li>
    </ul>
    <div class="tab-content" id="tabContent">
      <div class="tab-pane fade show active" id="content1" role="tabpanel" aria-labelledby="content1">頁籤內容</div>
      <div class="tab-pane fade" id="content2" role="tabpanel" aria-labelledby="content2">頁籤內容</div>
      <div class="tab-pane fade" id="content3" role="tabpanel" aria-labelledby="content3">頁籤內容</div>
    </div>
  </div>
</div>
<br />
<div class="row">
  <div class="col-12">
    <ul class="nav nav-pills" id="pills-tab" role="tablist">
      <li class="nav-item" role="presentation">
        <button class="nav-link active" id="pills-tab1" data-bs-toggle="pill" data-bs-target="#pills-content1" type="button" role="tab" aria-controls="pills-tab1" aria-selected="true">頁籤項目</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="pills-tab2" data-bs-toggle="pill" data-bs-target="#pills-content2" type="button" role="tab" aria-controls="pills-tab2" aria-selected="false">頁籤項目</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="pills-tab3" data-bs-toggle="pill" data-bs-target="#pills-content3" type="button" role="tab" aria-controls="pills-tab3" aria-selected="false">頁籤項目</button>
      </li>
    </ul>
    <div class="tab-content" id="pills-tabContent">
      <div class="tab-pane fade show active" id="pills-content1" role="tabpanel" aria-labelledby="pills-content1">頁籤內容</div>
      <div class="tab-pane fade" id="pills-content2" role="tabpanel" aria-labelledby="pills-content2">頁籤內容</div>
      <div class="tab-pane fade" id="pills-content3" role="tabpanel" aria-labelledby="pills-content3">頁籤內容</div>
    </div>
  </div>
</div>

{{< /example >}}

#### 依版面寬 (screen based)

版面寬度固定的情況下，頁籤的長度依版面款度等比例分配。有時也會稱依文字長 (label-based) 為堆疊式 (stacked) ，依版面寬 (screen based) 則為等分式 (distributed)。如果文字長度超過頁籤寬度而換行時，建議用其他頁籤設計，如：基本款頁籤。

{{< example >}}

<div class="row">
  <div class="col-12">
    <ul class="nav nav-tabs nav-fill" id="tab-fill" role="tablist">
      <li class="nav-item" role="presentation">
        <button class="nav-link active" id="tab1-fill" data-bs-toggle="tab" data-bs-target="#content1-fill" type="button" role="tab" aria-controls="tab1-fill" aria-selected="true">頁籤項目</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="tab2-fill" data-bs-toggle="tab" data-bs-target="#content2-fill" type="button" role="tab" aria-controls="tab2-fill" aria-selected="false">頁籤項目</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="tab3-fill" data-bs-toggle="tab" data-bs-target="#content3-fill" type="button" role="tab" aria-controls="tab3-fill" aria-selected="false">頁籤項目</button>
      </li>
    </ul>
    <div class="tab-content" id="tabContent-fill">
      <div class="tab-pane fade show active" id="content1-fill" role="tabpanel" aria-labelledby="content1-fill">頁籤內容</div>
      <div class="tab-pane fade" id="content2-fill" role="tabpanel" aria-labelledby="content2-fill">頁籤內容</div>
      <div class="tab-pane fade" id="content3-fill" role="tabpanel" aria-labelledby="content3-fill">頁籤內容</div>
    </div>
  </div>
</div>
<br />
<div class="row">
  <div class="col-12">
    <ul class="nav nav-pills nav-fill" id="pills-tab-fill" role="tablist">
      <li class="nav-item" role="presentation">
        <button class="nav-link active" id="pills-tab1-fill" data-bs-toggle="pill" data-bs-target="#pills-content1-fill" type="button" role="tab" aria-controls="pills-tab1-fill" aria-selected="true">頁籤項目</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="pills-tab2-fill" data-bs-toggle="pill" data-bs-target="#pills-content2-fill" type="button" role="tab" aria-controls="pills-tab2-fill" aria-selected="false">頁籤項目</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="pills-tab3-fill" data-bs-toggle="pill" data-bs-target="#pills-content3-fill" type="button" role="tab" aria-controls="pills-tab3-fill" aria-selected="false">頁籤項目</button>
      </li>
    </ul>
    <div class="tab-content" id="pills-tabContent-fill">
      <div class="tab-pane fade show active" id="pills-content1-fill" role="tabpanel" aria-labelledby="pills-content1-fill">頁籤內容</div>
      <div class="tab-pane fade" id="pills-content2-fill" role="tabpanel" aria-labelledby="pills-content2-fill">頁籤內容</div>
      <div class="tab-pane fade" id="pills-content3-fill" role="tabpanel" aria-labelledby="pills-content3-fill">頁籤內容</div>
    </div>
  </div>
</div>

{{< /example >}}

#### 頁籤圖標 (iconed tab)

頁籤的文字前面可以加上簡單的圖標，方便使用者查找、瀏覽。

{{< example >}}

<div class="row">
  <div class="col-12">
    <ul class="nav nav-tabs" id="tab-icon" role="tablist">
      <li class="nav-item" role="presentation">
        <button class="nav-link active" id="tab1-icon" data-bs-toggle="tab" data-bs-target="#content1-icon" type="button" role="tab" aria-controls="tab1-icon" aria-selected="true"><i class="bi bi-box-seam icon"></i>寄包裹</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="tab2-icon" data-bs-toggle="tab" data-bs-target="#content2-icon" type="button" role="tab" aria-controls="tab2-icon" aria-selected="false"><i class="bi bi-envelope icon"></i>寄信件</button>
      </li>
    </ul>
    <div class="tab-content" id="tabContent-icon">
      <div class="tab-pane fade show active" id="content1-icon" role="tabpanel" aria-labelledby="content1-icon">頁籤內容</div>
      <div class="tab-pane fade" id="content2-icon" role="tabpanel" aria-labelledby="content2-icon">頁籤內容</div>
    </div>
  </div>
</div>
<br />
<div class="row">
  <div class="col-12">
    <ul class="nav nav-pills" id="pills-tab-icon" role="tablist">
      <li class="nav-item" role="presentation">
        <button class="nav-link active" id="pills-tab1-icon" data-bs-toggle="pill" data-bs-target="#pills-content1-icon" type="button" role="tab" aria-controls="pills-tab1-icon" aria-selected="true"><i class="bi bi-globe icon"></i>依地圖瀏覽</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="pills-tab2-icon" data-bs-toggle="pill" data-bs-target="#pills-content2-icon" type="button" role="tab" aria-controls="pills-tab2-icon" aria-selected="false"><i class="bi bi-table icon"></i>依日期瀏覽</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="pills-tab3-icon" data-bs-toggle="pill" data-bs-target="#pills-content3-icon" type="button" role="tab" aria-controls="pills-tab3-icon" aria-selected="false"><i class="bi bi-view-stacked icon"></i>依列表瀏覽</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="pills-tab4-icon" data-bs-toggle="pill" data-bs-target="#pills-content4-icon" type="button" role="tab" aria-controls="pills-tab4-icon" aria-selected="false"><i class="bi bi-ui-checks-grid icon"></i>依主題瀏覽</button>
      </li>
    </ul>
    <div class="tab-content" id="pills-tabContent-icon">
      <div class="tab-pane fade show active" id="pills-content1-icon" role="tabpanel" aria-labelledby="pills-content1-icon">頁籤內容</div>
      <div class="tab-pane fade" id="pills-content2-icon" role="tabpanel" aria-labelledby="pills-content2-icon">頁籤內容</div>
      <div class="tab-pane fade" id="pills-content3-icon" role="tabpanel" aria-labelledby="pills-content3-icon">頁籤內容</div>
      <div class="tab-pane fade" id="pills-content4-icon" role="tabpanel" aria-labelledby="pills-content4-icon">頁籤內容</div>
    </div>
  </div>
</div>

{{< /example >}}

#### 多頁籤 滾動式 (scrollable-tabs) vs 磚牆式 (pill-bricks)

當頁籤列表內容較多時，可將選用滾動式的頁籤面板，或是磚牆式的膠囊式頁籤延伸。磚牆式的好處是列表數量可以比較有機的增加，使用者仍然能夠一次看見所有的頁籤內容。滾動式的頁籤面板則必須將某幾個頁籤放在較低順位或藏起，因此使用者可能會在一開始看不到某幾個頁籤內容。

##### 滾動式多頁籤
{{< example >}}
<div class="row">
  <div class="col-12">
    <div class="nav-scroll">
      <button type="button" class="btn" onclick="Prev(this)"><i class="bi bi-caret-left"></i></button>
      <div class="nav-scroll-wrapper">
        <ul class="nav nav-tabs" role="tablist">
          <li class="nav-item" role="presentation">
            <button class="nav-link active" id="scroll-tab1" data-bs-toggle="tab" data-bs-target="#scroll-content1" type="button" role="tab" aria-controls="scroll-content1" aria-selected="true">頁籤項目</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-tab2" data-bs-toggle="tab" data-bs-target="#scroll-content2" type="button" role="tab" aria-controls="scroll-content2" aria-selected="false">頁籤項目</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-tab3" data-bs-toggle="tab" data-bs-target="#scroll-content3" type="button" role="tab" aria-controls="scroll-content3" aria-selected="false">頁籤項目</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-tab4" data-bs-toggle="tab" data-bs-target="#scroll-content4" type="button" role="tab" aria-controls="scroll-content4" aria-selected="false">頁籤項目</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-tab5" data-bs-toggle="tab" data-bs-target="#scroll-content5" type="button" role="tab" aria-controls="scroll-content5" aria-selected="false">頁籤項目</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-tab6" data-bs-toggle="tab" data-bs-target="#scroll-content6" type="button" role="tab" aria-controls="scroll-content6" aria-selected="false">頁籤項目</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-tab7" data-bs-toggle="tab" data-bs-target="#scroll-content7" type="button" role="tab" aria-controls="scroll-content7" aria-selected="false">頁籤項目</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-tab8" data-bs-toggle="tab" data-bs-target="#scroll-content8" type="button" role="tab" aria-controls="scroll-content8" aria-selected="false">頁籤項目</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-tab9" data-bs-toggle="tab" data-bs-target="#scroll-content9" type="button" role="tab" aria-controls="scroll-content9" aria-selected="false">頁籤項目</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-tab10" data-bs-toggle="tab" data-bs-target="#scroll-content10" type="button" role="tab" aria-controls="scroll-content10" aria-selected="false">頁籤項目</button>
          </li>
        </ul>
      </div>
      <button class="btn" onclick="Next(this)"><i class="bi bi-caret-right"></i></button>
    </div>
    <div class="tab-content" id="tabContent-scrollable">
      <div class="tab-pane fade show active" id="scroll-content1" role="tabpanel" aria-labelledby="scroll-tab1">頁籤內容1</div>
      <div class="tab-pane fade" id="scroll-content2" role="tabpanel" aria-labelledby="scroll-tab2">頁籤內容2</div>
      <div class="tab-pane fade" id="scroll-content3" role="tabpanel" aria-labelledby="scroll-tab3">頁籤內容3</div>
      <div class="tab-pane fade" id="scroll-content4" role="tabpanel" aria-labelledby="scroll-tab4">頁籤內容4</div>
      <div class="tab-pane fade" id="scroll-content5" role="tabpanel" aria-labelledby="scroll-tab5">頁籤內容5</div>
      <div class="tab-pane fade" id="scroll-content6" role="tabpanel" aria-labelledby="scroll-tab6">頁籤內容6</div>
      <div class="tab-pane fade" id="scroll-content7" role="tabpanel" aria-labelledby="scroll-tab7">頁籤內容7</div>
      <div class="tab-pane fade" id="scroll-content8" role="tabpanel" aria-labelledby="scroll-tab8">頁籤內容8</div>
      <div class="tab-pane fade" id="scroll-content9" role="tabpanel" aria-labelledby="scroll-tab9">頁籤內容9</div>
      <div class="tab-pane fade" id="scroll-content10" role="tabpanel" aria-labelledby="scroll-tab10">頁籤內容10</div>
    </div>
  </div>
</div>
<br />
<div class="row">
  <div class="col-12">
    <div class="nav-scroll">
      <button type="button" class="btn" onclick="Prev(this)"><i class="bi bi-caret-left"></i></button>
      <div class="nav-scroll-wrapper">
        <ul class="nav nav-pills" role="tablist">
          <li class="nav-item" role="presentation">
            <button class="nav-link active" id="scroll-pills-tab1" data-bs-toggle="pill" data-bs-target="#scroll-pills-content1" type="button" role="tab" aria-controls="scroll-pills-content1" aria-selected="true">頁籤項目</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-pills-tab2" data-bs-toggle="pill" data-bs-target="#scroll-pills-content2" type="button" role="tab" aria-controls="scroll-pills-content2" aria-selected="false">頁籤項目</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-pills-tab3" data-bs-toggle="pill" data-bs-target="#scroll-pills-content3" type="button" role="tab" aria-controls="scroll-pills-content3" aria-selected="false">頁籤項目</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-pills-tab4" data-bs-toggle="pill" data-bs-target="#scroll-pills-content4" type="button" role="tab" aria-controls="scroll-pills-content4" aria-selected="false">頁籤項目</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-pills-tab5" data-bs-toggle="pill" data-bs-target="#scroll-pills-content5" type="button" role="tab" aria-controls="scroll-pills-content5" aria-selected="false">頁籤項目</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-pills-tab6" data-bs-toggle="pill" data-bs-target="#scroll-pills-content6" type="button" role="tab" aria-controls="scroll-pills-content6" aria-selected="false">頁籤項目</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-pills-tab7" data-bs-toggle="pill" data-bs-target="#scroll-pills-content7" type="button" role="tab" aria-controls="scroll-pills-content7" aria-selected="false">頁籤項目</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-pills-tab8" data-bs-toggle="pill" data-bs-target="#scroll-pills-content8" type="button" role="tab" aria-controls="scroll-pills-content8" aria-selected="false">頁籤項目</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-pills-tab9" data-bs-toggle="pill" data-bs-target="#scroll-pills-content9" type="button" role="tab" aria-controls="scroll-pills-content9" aria-selected="false">頁籤項目</button>
          </li>
          <li class="nav-item" role="presentation">
            <button class="nav-link" id="scroll-pills-tab10" data-bs-toggle="pill" data-bs-target="#scroll-pills-content10" type="button" role="tab" aria-controls="scroll-pills-content10" aria-selected="false">頁籤項目</button>
          </li>
        </ul>
      </div>
      <button class="btn" onclick="Next(this)"><i class="bi bi-caret-right"></i></button>
    </div>
    <div class="tab-content" id="tabContent-scrollable">
      <div class="tab-pane fade show active" id="scroll-pills-content1" role="tabpanel" aria-labelledby="scroll-pills-tab1">頁籤內容1</div>
      <div class="tab-pane fade" id="scroll-pills-content2" role="tabpanel" aria-labelledby="scroll-pills-tab2">頁籤內容2</div>
      <div class="tab-pane fade" id="scroll-pills-content3" role="tabpanel" aria-labelledby="scroll-pills-tab3">頁籤內容3</div>
      <div class="tab-pane fade" id="scroll-pills-content4" role="tabpanel" aria-labelledby="scroll-pills-tab4">頁籤內容4</div>
      <div class="tab-pane fade" id="scroll-pills-content5" role="tabpanel" aria-labelledby="scroll-pills-tab5">頁籤內容5</div>
      <div class="tab-pane fade" id="scroll-pills-content6" role="tabpanel" aria-labelledby="scroll-pills-tab6">頁籤內容6</div>
      <div class="tab-pane fade" id="scroll-pills-content7" role="tabpanel" aria-labelledby="scroll-pills-tab7">頁籤內容7</div>
      <div class="tab-pane fade" id="scroll-pills-content8" role="tabpanel" aria-labelledby="scroll-pills-tab8">頁籤內容8</div>
      <div class="tab-pane fade" id="scroll-pills-content9" role="tabpanel" aria-labelledby="scroll-pills-tab9">頁籤內容9</div>
      <div class="tab-pane fade" id="scroll-pills-content10" role="tabpanel" aria-labelledby="scroll-pills-tab10">頁籤內容10</div>
    </div>
  </div>
</div>


<script>
  // Script only for scrollable tabs
  const Prev = (e) => {
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
  }

  const Next = (e) => {
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
    
  }

</script>

{{< /example >}}
##### 磚牆式多頁籤
{{< example >}}
<div class="row">
  <div class="col-12">
    <ul class="nav nav-tabs" id="brick-tab" role="tablist">
      <li class="nav-item" role="presentation">
        <button class="nav-link active" id="brick-tab1" data-bs-toggle="tab" data-bs-target="#brick-tab-content1" type="button" role="tab" aria-controls="brick-content1" aria-selected="true">頁籤項目</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-tab2" data-bs-toggle="tab" data-bs-target="#brick-content2" type="button" role="tab" aria-controls="brick-content2" aria-selected="false">頁籤項目</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-tab3" data-bs-toggle="tab" data-bs-target="#brick-content3" type="button" role="tab" aria-controls="brick-content3" aria-selected="false">頁籤項目</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-tab4" data-bs-toggle="tab" data-bs-target="#brick-content4" type="button" role="tab" aria-controls="brick-content4" aria-selected="false">頁籤項目</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-tab5" data-bs-toggle="tab" data-bs-target="#brick-content5" type="button" role="tab" aria-controls="brick-content5" aria-selected="false">頁籤項目</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-tab6" data-bs-toggle="tab" data-bs-target="#brick-content6" type="button" role="tab" aria-controls="brick-content6" aria-selected="false">頁籤項目</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-tab7" data-bs-toggle="tab" data-bs-target="#brick-content7" type="button" role="tab" aria-controls="brick-content7" aria-selected="false">頁籤項目</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-tab8" data-bs-toggle="tab" data-bs-target="#brick-content8" type="button" role="tab" aria-controls="brick-content8" aria-selected="false">頁籤項目</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-tab9" data-bs-toggle="tab" data-bs-target="#brick-content9" type="button" role="tab" aria-controls="brick-content9" aria-selected="false">頁籤項目</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-tab10" data-bs-toggle="tab" data-bs-target="#brick-content10" type="button" role="tab" aria-controls="brick-content10" aria-selected="false">頁籤項目</button>
      </li>
    </ul>
    <div class="tab-content" id="brick-tabContent">
      <div class="tab-pane fade show active" id="brick-content1" role="tabpanel" aria-labelledby="brick-content1">頁籤內容1</div>
      <div class="tab-pane fade" id="brick-content2" role="tabpanel" aria-labelledby="brick-content2">頁籤內容2</div>
      <div class="tab-pane fade" id="brick-content3" role="tabpanel" aria-labelledby="brick-content3">頁籤內容3</div>
      <div class="tab-pane fade" id="brick-content4" role="tabpanel" aria-labelledby="brick-content4">頁籤內容4</div>
      <div class="tab-pane fade" id="brick-content5" role="tabpanel" aria-labelledby="brick-content5">頁籤內容5</div>
      <div class="tab-pane fade" id="brick-content6" role="tabpanel" aria-labelledby="brick-content6">頁籤內容6</div>
      <div class="tab-pane fade" id="brick-content7" role="tabpanel" aria-labelledby="brick-content7">頁籤內容7</div>
      <div class="tab-pane fade" id="brick-content8" role="tabpanel" aria-labelledby="brick-content8">頁籤內容8</div>
      <div class="tab-pane fade" id="brick-content9" role="tabpanel" aria-labelledby="brick-content9">頁籤內容9</div>
      <div class="tab-pane fade" id="brick-content10" role="tabpanel" aria-labelledby="brick-content10">頁籤內容10</div>
    </div>
  </div>
</div>
<br>
<div class="row">
  <div class="col-12">
    <ul class="nav nav-pills" id="brick-pills-tab" role="tablist">
      <li class="nav-item" role="presentation">
        <button class="nav-link active" id="brick-pills-tab1" data-bs-toggle="pill" data-bs-target="#brick-pills-content1" type="button" role="tab" aria-controls="brick-pills-content1" aria-selected="true">頁籤項目</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-pills-tab2" data-bs-toggle="pill" data-bs-target="#brick-pills-content2" type="button" role="tab" aria-controls="brick-pills-content2" aria-selected="false">頁籤項目</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-pills-tab3" data-bs-toggle="pill" data-bs-target="#brick-pills-content3" type="button" role="tab" aria-controls="brick-pills-content3" aria-selected="false">頁籤項目</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-pills-tab4" data-bs-toggle="pill" data-bs-target="#brick-pills-content4" type="button" role="tab" aria-controls="brick-pills-content4" aria-selected="false">頁籤項目</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-pills-tab5" data-bs-toggle="pill" data-bs-target="#brick-pills-content5" type="button" role="tab" aria-controls="brick-pills-content5" aria-selected="false">頁籤項目</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-pills-tab6" data-bs-toggle="pill" data-bs-target="#brick-pills-content6" type="button" role="tab" aria-controls="brick-pills-content6" aria-selected="false">頁籤項目</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-pills-tab7" data-bs-toggle="pill" data-bs-target="#brick-pills-content7" type="button" role="tab" aria-controls="brick-pills-content7" aria-selected="false">頁籤項目</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-pills-tab8" data-bs-toggle="pill" data-bs-target="#brick-pills-content8" type="button" role="tab" aria-controls="brick-pills-content8" aria-selected="false">頁籤項目</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-pills-tab9" data-bs-toggle="pill" data-bs-target="#brick-pills-content9" type="button" role="tab" aria-controls="brick-pills-content9" aria-selected="false">頁籤項目</button>
      </li>
      <li class="nav-item" role="presentation">
        <button class="nav-link" id="brick-pills-tab10" data-bs-toggle="pill" data-bs-target="#brick-pills-content10" type="button" role="tab" aria-controls="brick-pills-content10" aria-selected="false">頁籤項目</button>
      </li>
    </ul>
    <div class="tab-content" id="brick-pills-tabContent">
      <div class="tab-pane fade show active" id="brick-pills-content1" role="tabpanel" aria-labelledby="brick-pills-content1">頁籤內容1</div>
      <div class="tab-pane fade" id="brick-pills-content2" role="tabpanel" aria-labelledby="brick-pills-content2">頁籤內容2</div>
      <div class="tab-pane fade" id="brick-pills-content3" role="tabpanel" aria-labelledby="brick-pills-content3">頁籤內容3</div>
      <div class="tab-pane fade" id="brick-pills-content4" role="tabpanel" aria-labelledby="brick-pills-content4">頁籤內容4</div>
      <div class="tab-pane fade" id="brick-pills-content5" role="tabpanel" aria-labelledby="brick-pills-content5">頁籤內容5</div>
      <div class="tab-pane fade" id="brick-pills-content6" role="tabpanel" aria-labelledby="brick-pills-content6">頁籤內容6</div>
      <div class="tab-pane fade" id="brick-pills-content7" role="tabpanel" aria-labelledby="brick-pills-content7">頁籤內容7</div>
      <div class="tab-pane fade" id="brick-pills-content8" role="tabpanel" aria-labelledby="brick-pills-content8">頁籤內容8</div>
      <div class="tab-pane fade" id="brick-pills-content9" role="tabpanel" aria-labelledby="brick-pills-content9">頁籤內容9</div>
      <div class="tab-pane fade" id="brick-pills-content10" role="tabpanel" aria-labelledby="brick-pills-content10">頁籤內容10</div>
    </div>
  </div>
</div>
{{< /example >}}

#### 下拉式選單 (select)

當您認為使用者應該不需要一次看到所有頁籤內容時，請考慮使用另一個元件：下拉式選單。

{{< example >}}

<div class="row">
  <div class="col-md-6">
    <div class="d-flex align-items-center">
      <label for="select1" class="horizontal-label">頁籤標題</label>
      <select class="select" id="select1" aria-label="select1">
        <option class="option" selected>請選擇一個選項</option>
        <option class="option" value="1">頁籤項目</option>
        <option class="option" value="2">頁籤項目</option>
        <option class="option" value="3">頁籤項目</option>
        <option class="option" value="4">頁籤項目</option>
        <option class="option" value="5">頁籤項目</option>
        <option class="option" value="6">頁籤項目</option>
        <option class="option" value="7">頁籤項目</option>
        <option class="option" value="8">頁籤項目</option>
      </select>
    </div>
  </div>
</div>

{{< /example >}}

#### 行動版頁籤導覽

在行動裝置上，因為空間較為稀缺，我們建議從以下三種設計中擇一使用。從左至右分別為：下拉式選單、滾動式頁籤與磚牆式頁籤。
