---
layout: docs
title: 卡片 Card
description: 卡片是一個常用來彙整或列舉資訊的呈現方式。
group: components
---

## 關於卡片

卡片是一個常用來彙整或列舉資訊的方式，是一種可擴展的內容容器。

卡片可以將特定主題的內容與行動放在一個容器裡，提供使用者一個整理好的資訊呈現。一張卡面上通常會放標題、內文與行動。內文的部分可以用圖片、文字段落、列表與連結擴充，行動則是以按鈕表現，讓使用者在初步了解之後，透過按鈕被帶往下一層更深入、更準確的行為。

也因此，卡片通常是另一個更詳細資訊頁面的入口，使用者在點擊卡片之後會被帶往更多資訊的面進行下一步動作。

## 使用規範

### 何時該使用卡片

卡片是成群出現的，極少有單獨存在的機會。將一群相關的內容分主題呈現，不同主題的卡片通常以陣列形式座落在頁面上，方便使用者一次瀏覽各式內容，例如各式文章主題、各式服務類別、各式活動類型。

並且，卡片本身的存在是獨立的，並不會因與前後卡片之間的順序調動就影響到卡片的意涵。卡片與卡片之間的差別在於他們的內容不同。在頁面上的卡片因為有框線、色差、或是陰影而與頁面背景有所區別。

### 何時該考慮使用其他元件

1. **表格資料。** 請勿用卡片呈現一個表格的列 (row of table) 就可以呈現的資訊。
2. **簡單的行動呼籲 (call to action)。** 若只是簡單的想引導使用者到下一步，請直接用按鈕 (button) 實作在網頁上，毋需以卡片做過多的包裝。
3. **單獨存在的內容。** 考慮其他較適合單獨存在的元件。
4. **序列文字、連續的文字。** 卡片本身所呈現的內容應獨立在一張卡片上面，如果讀者需要從一張卡片讀到下一張卡片，那麼請考慮換成使用列表 (list)。
5. **沒有明確的下一步。** 卡片應要可以引導使用者點擊行動呼籲或是點選整張卡片進入內容頁。若沒有明確的下一步，請考慮用其他純展示、不需可操作、無互動的元件。

### 卡片易用性

1. **讓卡片是可以操作的。** 卡片上放的是一段資訊的總結，因此在使用卡片時，要確保可以讓卡片連到更詳細的資訊（例如：了解更多）或是下一步的動作（例如：報名活動）。若設計上決定卡片中是沒有行動按鈕的，請將整張卡片實作爲可以點擊，並進入更多相關資訊。
2. **請勿將卡片僅作為裝飾用的線框。** 卡片的使用有其整理資訊、引導下一步操作的目的性，請勿隨意將任何需要線框的內容直接套進卡片元件裡實作。若無下一步動作，請使用其他元件實作。
3. **用卡片作為不同內容的整理呈現方式。** 請勿將重複的內容放到同一組卡片上（例如：在同一組的每張卡片上放一模一樣的圖片），因為這樣讓使用者很難迅速分別出不同卡片的差異。
4. **確保圖片的長寬比例正確。** 卡片的長寬常隨著不同裝置、不同螢幕大小而異，在卡片上使用圖片時請確保所有裝置上的圖片比例皆正確，沒有被擠壓拉伸。
5. **風格儘量乾淨簡單。** 請避免用太過於花俏的特效、擬真的視覺設計來吸引使用者注意力。使用者注意力的引導應藉由導覽來執行，請勿取巧利用元件本身的設計分散使用者在整體體驗中的注意力。

### 卡片近用性

1. **使用無序列表 (unordered list)實作。** 將 Card group 用 `ul` 包起來，裡面的每張卡則用 `li` 來寫。這樣能讓確保螢幕報讀軟體 (screen reader) 順利計算卡片數量，啟動快捷功能。
2. **使用正確的標題層級 (heading level)。** 檢查你的頁面中的所有標題的標題層級 (heading level)，確保表題之間的邏輯正確，以利螢幕報讀軟體 (screen reader) 順利讀取頁面的內容。

## 元件設計

### 基本款卡片 Basic card

基本款卡片包含卡片本身、標題、內文與圖片。

{{< example >}}

<div class="row d-flex justify-content-center">
  <div class="col-lg-4">
    <div class="card">
      <img src="/docs/5.1/assets/img/bg-card.png" class="card-img-top" alt="...">  
      <div class="card-body">
        <div class="card-title">標題文字</div>
        <div class="card-text">此部分為卡片之內文部分文字或副標題內容</div>
        <div class="card-actions">
          <button type="button" class="btn btn-primary">預設按鈕</button>
        </div>
      </div>
    </div>
  </div>
</div>

{{< /example >}}

### 框線風格 Border Style

- Outlined：用框線將卡片本身與背景區隔開。
- Elevated：將卡片視覺上做提升浮起的效果，以與背景區隔。

{{< example >}}

<div class="row d-flex justify-content-center">
  <div class="col-lg-4">
    <div class="card">
      <img src="/docs/5.1/assets/img/bg-card.png" class="card-img-top" alt="..."/>
      <div class="card-body">
        <div class="card-title">標題文字</div>
        <div class="card-text">此部分為卡片之內文部分文字或副標題內容</div>
        <div class="card-actions">
          <button type="button" class="btn btn-primary">預設按鈕</button>
        </div>
      </div>
    </div>
  </div>
  <div class="col-lg-4">
    <div class="card elevated">
      <img src="/docs/5.1/assets/img/bg-card.png" class="card-img-top" alt="..."/>
      <div class="card-body">
        <div class="card-title">標題文字</div>
        <div class="card-text">此部分為卡片之內文部分文字或副標題內容</div>
        <div class="card-actions">
          <button type="button" class="btn btn-primary">預設按鈕</button>
        </div>
      </div>
    </div>
  </div>
</div>

{{< /example >}}

### 方向 Direction

- Vertical：圖片在內文上方。
- Horizonal：圖片在內文左邊。

{{< example >}}

<div class="row gy-5 d-flex justify-content-center">
  <div class="col-lg-4">
    <div class="card">
      <img src="/docs/5.1/assets/img/bg-card.png" class="card-img-top" alt="..."/>
      <div class="card-body">
        <div class="card-title">標題文字</div>
        <div class="card-text">此部分為卡片之內文部分文字或副標題內容</div>
        <div class="card-actions">
          <button type="button" class="btn btn-primary">預設按鈕</button>
        </div>
      </div>
    </div>
  </div>
  <div class="col-lg-8">
    <div class="card">
      <div class="row align-items-center">
        <div class="col-lg-4">
          <div class="card-image rounded-start" style="background: url('/docs/5.1/assets/img/bg-card.png')"></div>
        </div>
        <div class="col-lg-8">
          <div class="card-body">
            <div class="card-title">標題文字</div>
            <div class="card-text">
              此部分為卡片之內文部分文字或副標題內容
            </div>
            <div class="card-actions">
            <button type="button" class="btn btn-primary">預設按鈕</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

{{< /example >}}

### 文字對齊 Text Alignment

- Center：文字、按鈕與標籤都置中
- Left：文字、按鈕與標籤都向左對齊

{{< example >}}

<div class="row gy-5 d-flex justify-content-center">
  <div class="col-lg-4">
    <div class="card">
      <img src="/docs/5.1/assets/img/bg-card.png" class="card-img-top" alt="..."/>
      <div class="card-body">
        <div class="card-title">標題文字</div>
        <div class="badge-group">
          <span class="badge">主題標籤</span
          ><span class="badge">主題標籤</span
          ><span class="badge">主題標籤</span>
        </div>
        <div class="card-text">此部分為卡片之內文部分文字或副標題內容</div>
        <div class="card-actions">
          <button type="button" class="btn btn-primary">預設按鈕</button>
        </div>
      </div>
    </div>
  </div>
  <div class="col-lg-4">
    <div class="card text-center">
      <img src="/docs/5.1/assets/img/bg-card.png" class="card-img-top" alt="..."/>
      <div class="card-body">
        <div class="card-title">標題文字</div>
        <div class="badge-group">
          <span class="badge">主題標籤</span
          ><span class="badge">主題標籤</span
          ><span class="badge">主題標籤</span>
        </div>
        <div class="card-text">此部分為卡片之內文部分文字或副標題內容</div>
        <div class="card-actions">
          <button type="button" class="btn btn-primary">預設按鈕</button>
        </div>
      </div>
    </div>
  </div>
</div>

{{< /example >}}

### 按鈕變形 Button Variation
依據按鈕的呈現方式可以有以下變形：

- One：單一按鈕，通常為行動按鈕 (Action Button)。
- TwoRight：兩個按紐，通常一個為主要行動按鈕，另一個為次要按鈕，例如「暸解詳情」。
- Icon：只有圖示按鈕，目前預設為向右的箭頭圖示。

在有按鈕的時候，只有按鈕的部分可以點擊，但若卡片是沒有按鈕的，整張卡片可以點擊。

{{< example >}}

<div class="row gy-5 d-flex justify-content-center">
  <div class="col-lg-4">
    <div class="card">
      <img src="/docs/5.1/assets/img/bg-card.png" class="card-img-top" alt="..."/>
      <div class="card-body">
        <div class="card-title">標題文字</div>
        <div class="badge-group">
          <span class="badge">主題標籤</span
          ><span class="badge">主題標籤</span
          ><span class="badge">主題標籤</span>
        </div>
        <div class="card-text">此部分為卡片之內文部分文字或副標題內容</div>
        <div class="card-actions">
          <button type="button" class="btn btn-primary">預設按鈕</button>
        </div>
      </div>
    </div>
  </div>
  <div class="col-lg-4">
    <div class="card text-center">
      <img src="/docs/5.1/assets/img/bg-card.png" class="card-img-top" alt="..."/>
      <div class="card-body">
        <div class="card-title">標題文字</div>
        <div class="badge-group">
          <span class="badge">主題標籤</span
          ><span class="badge">主題標籤</span
          ><span class="badge">主題標籤</span>
        </div>
        <div class="card-text">此部分為卡片之內文部分文字或副標題內容</div>
        <div class="card-actions text-end">
          <button type="button" class="btn btn-primary">預設按鈕</button>
          <button type="button" class="btn btn-tertiary">
            預設按鈕
          </button>
        </div>
      </div>
    </div>
  </div>
</div>
<div class="row gy-5 d-flex justify-content-center mt-3">
  <div class="col-lg-4">
    <div class="card">
      <img src="/docs/5.1/assets/img/bg-card.png" class="card-img-top" alt="..."/>
      <div class="card-body">
        <div class="card-title">標題文字</div>
        <div class="badge-group">
          <span class="badge">主題標籤</span
          ><span class="badge">主題標籤</span
          ><span class="badge">主題標籤</span>
        </div>
        <div class="card-text">此部分為卡片之內文部分文字或副標題內容</div>
        <div class="text-end">
          <button class="btn btn-less-important" alt="...">
            <i class="bi bi-arrow-right"></i>
          </button>
        </div>
      </div>
    </div>
  </div>
  <div class="col-lg-4">
    <div class="card clickable" onclick="location.href='#'">
      <img src="/docs/5.1/assets/img/bg-card.png" class="card-img-top" alt="..."/>
      <div class="card-body">
        <div class="card-title">標題文字</div>
        <div class="badge-group">
          <span class="badge">主題標籤</span
          ><span class="badge">主題標籤</span
          ><span class="badge">主題標籤</span>
        </div>
        <div class="card-text">此部分為卡片之內文部分文字或副標題內容</div>
      </div>
    </div>
  </div>
</div>

{{< /example >}}

### 含有列表群組的卡片 Card with list group

卡片內容需要以列表群組呈現時，可以使用此元件。卡片內容可以混合並搭配多個內容形式。以下範例將圖片、文字樣式、列表群組以及連結全部包裝在一個固定寬度的卡片中。

{{< example >}}

<div class="row gy-5 d-flex justify-content-center">
  <div class="col-lg-4">
    <div class="card masonry-card">
      <div class="card-header">服務項目類別</div>
      <div class="card-body">
        <div class="card-title">標題</div>
        <div class="card-text">
          卡片內文或補充說明。
        </div>
        <hr />
        <ul class="list-group">
          <a href="#" class="list-group-item">
            <i class="bi bi-bell-fill"></i>
            <div>列表主要文字</div>
          </a>
          <a href="#" class="list-group-item">
            <i class="bi bi-bell-fill"></i>
            <div>列表主要文字</div>
          </a>
          <a href="#" class="list-group-item">
            <i class="bi bi-bell-fill"></i>
            <div>列表主要文字</div>
          </a>
          <a href="#" class="list-group-item">
            <i class="bi bi-bell-fill"></i>
            <div>列表主要文字</div>
          </a>
        </ul>
      </div>
    </div>
  </div>
  <div class="col-lg-4">
    <div class="card masonry-card text-center">
      <div class="card-header">服務項目類別</div>
      <div class="card-body">
        <div class="card-title">標題</div>
        <div class="card-text">
          卡片內文或補充說明。
        </div>
        <hr />
        <ul class="list-group">
          <a href="#" class="list-group-item">
            <i class="bi bi-bell-fill"></i>
            <div>列表主要文字</div>
          </a>
          <a href="#" class="list-group-item">
            <i class="bi bi-bell-fill"></i>
            <div>列表主要文字</div>
          </a>
          <a href="#" class="list-group-item">
            <i class="bi bi-bell-fill"></i>
            <div>列表主要文字</div>
          </a>
          <a href="#" class="list-group-item">
            <i class="bi bi-bell-fill"></i>
            <div>列表主要文字</div>
          </a>
        </ul>
      </div>
    </div>
  </div>
</div>
<div class="row gy-5 d-flex justify-content-center mt-3">
  <div class="col-lg-4">
    <div class="card masonry-card">
      <div class="card-header">服務項目類別</div>
      <div class="card-body">
        <img src="/docs/5.1/assets/img/bg-list-card.png" class="img-fluid" alt="..."/>
        <div class="card-title">標題</div>
        <div class="card-text">
          卡片內文或補充說明。
        </div>
        <hr />
        <ul class="list-group">
          <a href="#" class="list-group-item">
            <i class="bi bi-bell-fill"></i>
            <div>列表主要文字</div>
          </a>
          <a href="#" class="list-group-item">
            <i class="bi bi-bell-fill"></i>
            <div>列表主要文字</div>
          </a>
          <a href="#" class="list-group-item">
            <i class="bi bi-bell-fill"></i>
            <div>列表主要文字</div>
          </a>
          <a href="#" class="list-group-item">
            <i class="bi bi-bell-fill"></i>
            <div>列表主要文字</div>
          </a>
        </ul>
      </div>
    </div>
  </div>
  <div class="col-lg-4">
    <div class="card masonry-card text-center">
      <div class="card-header">服務項目類別</div>
      <div class="card-body">
        <img src="/docs/5.1/assets/img/bg-list-card.png" class="img-fluid" alt="..."/>
        <div class="card-title">標題</div>
        <div class="card-text">
          卡片內文或補充說明。
        </div>
        <hr />
        <ul class="list-group">
          <a href="#" class="list-group-item">
            <i class="bi bi-bell-fill"></i>
            <div>列表主要文字</div>
          </a>
          <a href="#" class="list-group-item">
            <i class="bi bi-bell-fill"></i>
            <div>列表主要文字</div>
          </a>
          <a href="#" class="list-group-item">
            <i class="bi bi-bell-fill"></i>
            <div>列表主要文字</div>
          </a>
          <a href="#" class="list-group-item">
            <i class="bi bi-bell-fill"></i>
            <div>列表主要文字</div>
          </a>
        </ul>
      </div>
    </div>
  </div>
</div>

{{< /example >}}

### 文字卡 Masonry Card

純文字的卡片，若有圖片則為背景。若使用背景圖片時請注意色彩對比度。

{{< example >}}

<div class="row gy-5">
  <div class="col-lg-4">
    <div class="card masonry-card">
      <div class="card-header">服務項目類別</div>
      <div class="card-body">
        <div class="card-title">標題</div>
        <div class="card-text">
          此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明。
        </div>
      </div>
    </div>
  </div>
  <div class="col-lg-4">
    <div class="card masonry-card">
      <div class="card-header bg-brand-flat-strong">服務項目類別</div>
      <div class="card-body bg-brand-flat">
        <div class="card-title">標題</div>
        <div class="card-text">
          此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明。
        </div>
      </div>
    </div>
  </div>
  <div class="col-lg-4">
    <div class="card masonry-card">
      <div class="card-header bg-accent-flat-strong">服務項目類別</div>
      <div class="card-body bg-accent-flat">
        <div class="card-title">標題</div>
        <div class="card-text">
          此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明。
        </div>
      </div>
    </div>
  </div>
  <div class="col-lg-4">
    <div class="card masonry-card">
      <div class="card-header bg-positive-flat-strong">服務項目類別</div>
      <div class="card-body bg-positive-flat">
        <div class="card-title">標題</div>
        <div class="card-text">
          此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明。
        </div>
      </div>
    </div>
  </div>
  <div class="col-lg-4">
    <div class="card masonry-card">
      <div class="card-header bg-negative-flat-strong">服務項目類別</div>
      <div class="card-body bg-negative-flat">
        <div class="card-title">標題</div>
        <div class="card-text">
          此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明。
        </div>
      </div>
    </div>
  </div>
  <div class="col-lg-4">
    <div class="card masonry-card">
      <div class="card-header bg-information-flat-strong">服務項目類別</div>
      <div class="card-body bg-information-flat">
        <div class="card-title">標題</div>
        <div class="card-text">
          此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明。
        </div>
      </div>
    </div>
  </div>
  <div class="col-lg-4">
    <div class="card masonry-card">
      <div class="card-header bg-warning-flat-strong">服務項目類別</div>
      <div class="card-body bg-warning-flat">
        <div class="card-title">標題</div>
        <div class="card-text">
          此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明。
        </div>
      </div>
    </div>
  </div>
</div>

{{< /example >}}