---
layout: docs
title: 卡片 Card
description: 卡片是一個常用來彙整或列舉資訊的呈現方式。
group: components
---

### 關於卡片元件

卡片是一個常用來彙整或列舉資訊的方式，一個基本的卡片可以將特定主題的內容與行動放在一個容器裡。一張卡面上通常可以有標題、圖片、文字段落、列表、按鈕與連結。卡片通常是另一個更詳細資訊頁面的入口，使用者在點擊卡片之後會被帶往更多資訊的面進行下一步動作。

### 使用規範

#### 何時該使用卡片

卡片是成群出現的，極少有單獨存在的機會。將一群相關的內容分主題呈現，不同主題的卡片通常以陣列形式座落在頁面上，方便使用者一次瀏覽各式內容，例如各式文章主題、各式服務類別、各式活動類型。

並且，卡片本身的存在是獨立的，並不會因與前後卡片之間的順序調動就影響到卡片的意涵。卡片與卡片之間的差別在於他們的內容不同。在頁面上的卡片因為有框線、色差、或是陰影而與頁面背景有所區別。

#### 何時該考慮使用其他元件

1. **表格資料。** 請勿用卡片呈現一個表格的列 (row of table)。
2. **簡單的行動呼籲 (call to action)。** 若只是簡單的想引導使用者到下一步，請直接用按鈕 (button) 實作。
3. **單獨存在的內容。** 考慮其他較適合單獨存在的元件。
4. **序列文字、連續的文字。** 卡片本身所呈現的內容應獨立在一張卡片上面，如果讀者需要從一張卡片讀到下一張卡片，那麼請考慮換成使用列表 (list)。
5. **沒有明確的下一步。** 卡片應要可以引導使用者點擊行動呼籲或是點選整張卡片進入內容頁。若沒有明確的下一步，請考慮用其他純展示、不需可操作、無互動的元件。

#### 卡片易用性

1. **讓卡片是可以操作的。** 卡片上放的是一段資訊的總結，因此在使用卡片時，要確保可以讓卡片連到更詳細的資訊（例如：了解更多）或是下一步的動作（例如：報名活動）。
2. **請勿將卡片僅作為裝飾用的線框。** 卡片的使用有其整理資訊、引導下一步操作的目的性，請勿隨意將任何需要線框的內容直接套進卡片元件裡實作。
3. **用卡片作為不同內容的整理呈現方式。** 請勿將重複的內容放到同一組卡片上（例如：在同一組的每張卡片上放一模一樣的圖片），因為這樣讓使用者很難迅速分別出不同卡片的差異。
4. **確保圖片的長寬比例正確。** 卡片的長寬常隨著不同裝置、不同螢幕大小而異，在卡片上使用圖片時請確保所有裝置上的圖片比例皆正確，沒有被擠壓拉伸。
5. **風格儘量乾淨簡單。** 請避免用太過於花俏的特效、擬真的視覺設計來吸引使用者注意力。使用者注意力的引導應藉由導覽來執行，請勿取巧利用元件本身的設計分散使用者在整體體驗中的注意力。

#### 卡片近用性

1. **使用無序列表 (unordered list)實作。** 將 Card group 用 ul 包起來，裡面的每張卡則用 li 來寫。這樣能讓確保螢幕報讀軟體 (screen reader) 順利計算卡片數量，啟動快捷功能。
2. **使用正確的標題層級 (heading level)。** 檢查你的頁面中的所有標題的標題層級 (heading level)，確保表題之間的邏輯正確，以利螢幕報讀軟體 (screen reader) 順利讀取頁面的內容。

### 設計元件

#### 基本款卡片 Basic card

基本款卡片包含卡片本身、標題、內文與圖片。

{{< example >}}

<div class="row d-flex justify-content-center">
  <div class="col-md-4">
    <div class="card">
      <img src="/docs/5.1/assets/img/bg-card.png" class="image card-img-top" alt="...">  
      <div class="card-body">
        <div class="card-title">標題文字</div>
        <div class="badge-group">
          <span class="badge">主題標籤</span><span class="badge">主題標籤</span><span class="badge">主題標籤</span>
        </div>
        <div class="card-text">此部分為卡片之內文部分文字或副標題內容</div>
        <div class="card-actions">
          <button type="button" class="btn btn-primary">預設按鈕</button>
        </div>
      </div>
    </div>
  </div>
</div>


<div class="row d-flex justify-content-center">
  <div class="col-md-4">
    <div class="card masonry-card" onclick="location.href='#'">
      <div class="card-header">服務項目類別</div>
      <div class="card-body">
        <div class="card-title">標題</div>
        <div class="card-text">卡片內文或補充說明。 </div>
      </div>
    </div>
  </div>
</div>


<div class="row d-flex justify-content-center">
  <div class="col">
    <div class="card">
      <div class="row align-items-center">
        <div class="col-lg-4">
          <div class="card-image rounded-start" style="background: url('/docs/5.1/assets/img/bg-card.png')"></div>  
        </div>
        <div class="col-lg-8">
          <div class="card-body">
            <div class="card-title">標題文字</div>
            <div class="card-text">此部分為卡片之內文部分文字或副標題內容</div>
            <button type="button" class="btn btn-primary">預設按鈕</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
<br/>
<div class="row d-flex justify-content-center">
  <div class="col-md-5">
    <div class="card masonry-card">
      <div class="card-header">服務項目類別</div>
      <div class="card-body">
        <img src="/docs/5.1/assets/img/bg-list-card.png" class="img-fluid" alt="...">  
        <div class="card-title">標題</div>
        <div class="card-text">卡片內文或補充說明。
          <ol>
            <li>文字列表</li>
            <li>文字列表</li>
          </ol>
        </div>
        <hr>
        <ul class="list-group">
          <a href="#" class="list-group-item"><i class="bi bi-bell-fill"></i><div>列表主要文字</div></a>
          <a href="#" class="list-group-item"><i class="bi bi-bell-fill"></i><div>列表主要文字</div></a>
          <a href="#" class="list-group-item"><i class="bi bi-bell-fill"></i><div>列表主要文字</div></a>
          <a href="#" class="list-group-item"><i class="bi bi-bell-fill"></i><div>列表主要文字</div></a>
        </ul>
        <ul class="list-group list-group-horizontal">
          <a href="#" class="list-group-item flex-fill">額外連結</a>
          <a href="#" class="list-group-item flex-fill">額外連結</a>
          <a href="#" class="list-group-item flex-fill">額外連結</a>
        </ul>
    </div>
  </div>
</div>
<br/>
<div class="row d-flex justify-content-center">
  <div class="col-md-5">
    <div class="card masonry-card">
      <div class="card-header">服務項目類別</div>
      <div class="card-body">
        <div class="card-title">標題</div>
        <div class="card-text">卡片內文或補充說明。
          <ol>
            <li>文字列表</li>
            <li>文字列表</li>
          </ol>
        </div>
      </div>
      <div class="card-actions">
        <button type="button" class="btn btn-primary">預設按鈕</button>
      </div>
      <ul class="list-group">
        <li class="list-group-item"><i class="bi bi-award text-information icon"></i><a href="#">列表</a></li>
        <li class="list-group-item"><i class="bi bi-award text-information icon"></i><a href="#">列表</a></li>
        <li class="list-group-item"><i class="bi bi-award text-information icon"></i><a href="#">列表</a></li>
        <li class="list-group-item"><i class="bi bi-award text-information icon"></i><a href="#">列表</a></li>
      </ul>
    </div>
  </div>
</div>


{{< /example >}}

#### 文字對齊 Text Alignment

卡片內的標題與內文可以靠左或置中。

{{< example >}}

<div class="row d-flex justify-content-center">
  <div class="col-md-4">
    <div class="card">
      <img src="/docs/5.1/assets/img/bg-card.png" class="card-img-top" alt="...">  
      <div class="card-body">
        <h5 class="card-title">標題文字</h5>
        <p class="card-text">此部分為卡片之內文。</p>
      </div>
    </div>
  </div>
  <div class="col-md-4">
    <div class="card text-center">
      <img src="/docs/5.1/assets/img/bg-card.png" class="card-img-top" alt="...">  
      <div class="card-body">
        <h5 class="card-title">標題文字</h5>
        <p class="card-text">此部分為卡片之內文。</p>
      </div>
    </div>
  </div>
</div>

{{< /example >}}

#### 標題位置 Title Arrangement

標題的位置可以在圖片下方或上方。

{{< example >}}

<div class="row d-flex justify-content-center">
  <div class="col-md-4">
    <div class="card">
      <img src="/docs/5.1/assets/img/bg-card.png" class="card-img-top" alt="...">  
      <div class="card-body">
        <h5 class="card-title">標題文字</h5>
        <p class="card-text">此部分為卡片之內文。</p>
      </div>
    </div>
  </div>
  <div class="col-md-4">
    <div class="card">
      <div class="card-body">
        <h5 class="card-title">標題文字</h5>
        <p class="card-text">此部分為卡片之內文。</p>
      </div>
      <img src="/docs/5.1/assets/img/bg-card.png" class="card-img-top" alt="...">  
    </div>
  </div>
</div>

{{< /example >}}

#### 卡片框線風格 Card Border Style

框線的選擇有無框線、有框線、陰影。選擇無框線的卡片風格時，請注意元件本身與背景的色彩對比度。

{{< example >}}

<div class="container" style="padding: 1rem; background: #F8F9FA">
  <div class="row d-flex justify-content-center">
    <div class="col-md-4">
      <div class="card border-0">
        <img src="/docs/5.1/assets/img/bg-card.png" class="card-img-top" alt="...">  
        <div class="card-body">
          <h5 class="card-title">標題文字</h5>
          <p class="card-text">此部分為卡片之內文。</p>
        </div>
      </div>
    </div>
      <div class="col-md-4">
      <div class="card">
        <img src="/docs/5.1/assets/img/bg-card.png" class="card-img-top" alt="...">  
        <div class="card-body">
          <h5 class="card-title">標題文字</h5>
          <p class="card-text">此部分為卡片之內文。</p>
        </div>
      </div>
    </div>
      <div class="col-md-4">
      <div class="card shadow-sm">
        <img src="/docs/5.1/assets/img/bg-card.png" class="card-img-top" alt="...">  
        <div class="card-body">
          <h5 class="card-title">標題文字</h5>
          <p class="card-text">此部分為卡片之內文。</p>
        </div>
      </div>
    </div>
  </div>
</div>

{{< /example >}}

#### 一般卡片加按鈕 Card with button

按鈕的位置與內文對齊。

{{< example >}}

<div class="row d-flex justify-content-center">
  <div class="col-md-4">
    <div class="card">
      <img src="/docs/5.1/assets/img/bg-card.png" class="card-img-top" alt="...">  
      <div class="card-body">
        <h5 class="card-title">標題文字</h5>
        <p class="card-text">此部分為卡片之內文。</p>
        <a href="#" class="btn btn-primary">前往報名</a>
      </div>
    </div>
  </div>
    <div class="col-md-4">
    <div class="card text-center">
      <img src="/docs/5.1/assets/img/bg-card.png" class="card-img-top" alt="...">  
      <div class="card-body">
        <h5 class="card-title">標題文字</h5>
        <p class="card-text">此部分為卡片之內文。</p>
        <a href="#" class="btn btn-primary">前往報名</a>
      </div>
    </div>
  </div>
</div>

{{< /example >}}

#### 標題優先卡片加按鈕 Title first card with button

按鈕若與標題同時在圖片上方，用圖標按鈕呈現。

{{< example >}}

<div class="row d-flex justify-content-center">
  <div class="col-md-4">
    <div class="card">
      <div class="card-body">
        <div class="d-flex justify-content-between align-items-baseline">
        <h5 class="card-title">
          標題文字            
          </h5>
            <button class="btn text-information icon-btn">
              <i class="bi bi-arrow-right"></i>
            </button></div>
        <p class="card-text">此部分為卡片之內文。</p>
      </div>
      <img src="/docs/5.1/assets/img/bg-card.png" alt="...">  
    </div>
  </div>
</div>

{{< /example >}}

#### 一般卡片加標籤與日期 Card with tag and date

標籤與日期在標題上方。

{{< example >}}

<div class="row d-flex justify-content-center">
  <div class="col-md-5">
    <div class="card">
      <img src="/docs/5.1/assets/img/bg-card.png" class="card-img-top" alt="...">  
      <div class="card-body">
        <div class="badge-collections">
          <span class="badge bg-secondary-flat">標籤</span>
          <span class="badge bg-secondary-flat">標籤</span>
          <span class="badge bg-secondary-flat">標籤</span>
          <span class="badge bg-secondary-flat">標籤</span>
        </div>
        <p class="card-text">110-10-31</p>
        <h5 class="card-title">標題文字</h5>
        <p class="card-text">此部分為卡片之內文。</p>
        <a href="#" class="btn btn-primary">前往報名</a>
      </div>
    </div>
  </div>
  <div class="col-md-5">
    <div class="card">
      <img src="/docs/5.1/assets/img/bg-card.png" class="card-img-top" alt="...">  
      <div class="card-body">
        <div class="d-flex justify-content-between">
          <p class="card-text">110-10-31</p>
          <div>
            <span class="badge bg-secondary-flat">標籤</span>
          </div>
        </div>
        <h5 class="card-title">標題文字</h5>
        <p class="card-text">此部分為卡片之內文。</p>
        <a href="#" class="btn btn-primary">前往報名</a>
      </div>
    </div>
  </div>
</div>

{{< /example >}}

#### 標題優先卡片加標籤與日期 Title-first card with tag and date

標籤與日期在圖片上方或下方，呼籲按鈕則放在圖片對面。

{{< example >}}

<div class="row d-flex justify-content-center">
  <div class="col-md-6">
    <div class="card">
      <div class="card-body">
        <div class="d-flex justify-content-between">
          <p class="card-text">110-10-31</p>
          <div class="badge-collections">
            <span class="badge bg-secondary-flat">標籤</span>
            <span class="badge bg-secondary-flat">標籤</span>
            <span class="badge bg-secondary-flat">標籤</span>
          </div>
        </div>
        <h5 class="card-title">標題文字</h5>
      </div>
      <img src="/docs/5.1/assets/img/bg-card.png" class="card-img-top" alt="...">  
      <div class="card-body">
        <p class="card-text">此部分為卡片之內文。</p>
        <a href="#" class="btn btn-primary float-end">前往報名</a>
      </div>
    </div>
  </div>
  <div class="col-md-6">
    <div class="card">
      <div class="card-body">
        <div class="d-flex justify-content-between align-items-baseline">
        <h5 class="card-title">
          標題文字            
        </h5>
        <button class="btn text-information icon-btn">
          <i class="bi bi-arrow-right"></i>
        </button></div>
        <p class="card-text">此部分為卡片之內文。</p>
      </div>
      <img src="/docs/5.1/assets/img/bg-card.png" class="card-img-top" alt="...">  
      <div class="card-body">
        <div class="d-flex justify-content-between">
          <p class="card-text">110-10-31</p>
          <div>
            <span class="badge bg-secondary-flat">標籤</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

{{< /example >}}

#### 橫式卡片 Landscape card

圖片在內文左邊。

{{< example >}}

<div class="row d-flex justify-content-center">
  <div class="col">
    <div class="card">
      <div class="row g-0 align-items-center">
        <div class="col-md-4">
          <div class="image rounded-start" style="background: url('/docs/5.1/assets/img/bg-card.png')"></div>  
        </div>
        <div class="col-md-8">
          <div class="card-body">
            <h5 class="card-title">標題文字</h5>
            <p class="card-text">此部分為卡片之內文。</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

{{< /example >}}

#### 橫式卡片加按鈕 Landscape card with buttons

圖片在內文左邊，按鈕若在上方使用圖示按鈕，若在下方則於內文對齊。日期與標籤則在按鈕的對面。

{{< example >}}

<div class="row d-flex justify-content-center">
  <div class="col">
    <div class="card">
      <div class="row g-0 align-items-center">
        <div class="col-md-4">
          <div class="image rounded-start" style="background: url('/docs/5.1/assets/img/bg-card.png')"></div>
        </div>
        <div class="col-md-8">
          <div class="card-body">
            <div class="d-flex justify-content-between">
              <p class="card-text">110-10-31</p>
              <div>
                <span class="badge bg-secondary-flat">標籤</span>
                <span class="badge bg-secondary-flat">標籤</span>
              </div>
            </div>
            <h5 class="card-title">標題文字</h5>
            <p class="card-text">此部分為卡片之內文。</p>
            <a href="#" class="btn btn-primary">前往報名</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
<br/>
<div class="row d-flex justify-content-center">
  <div class="col">
    <div class="card">
      <div class="row g-0 align-items-center">
        <div class="col-md-4">
          <div class="image rounded-start" style="background: url('/docs/5.1/assets/img/bg-card.png')"></div> 
        </div>
        <div class="col-md-8">
          <div class="card-body">
            <div class="d-flex justify-content-between align-items-baseline">
              <h5 class="card-title">
                標題文字            
              </h5>
              <button class="btn text-information icon-btn">
                <i class="bi bi-arrow-right"></i>
              </button>
            </div>
            <p class="card-text">此部分為卡片之內文。</p>
            <div class="badge-collections">
              <span class="badge bg-secondary-flat">標籤</span>
              <span class="badge bg-secondary-flat">標籤</span>
              <span class="badge bg-secondary-flat">標籤</span>
              <span class="badge bg-secondary-flat">標籤</span>
            </div>
            <p class="card-text">110-10-31</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

{{< /example >}}

#### 文字卡 Masonry card

純文字的卡片，若有圖片則為背景。若使用背景圖片時請注意色彩對比度。

{{< example >}}

<div class="row d-flex justify-content-center">
  <div class="col-6">
    <div class="card text-card">
      <div class="card-body">
        <h4 class="card-title">服務項目</h4>
        <p class="card-text">此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明。</p>
      </div>
    </div>
  </div>
</div>
<br/>
<div class="row d-flex justify-content-center">
  <div class="col-6">
    <div class="card text-card">
      <div class="card-body text-white" style='background-image: url("/docs/5.1/assets/img/bg-text-card.png")'>
        <h4 class="card-title text-white">服務項目</h4>
        <p>此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明。</p>
      </div>
    </div>
  </div>
</div>
<br/>
<div class="row d-flex justify-content-center">
  <div class="col-6">
    <div class="card text-card">
      <div class="card-header">服務項目類別</div>
      <div class="card-body">
        <h4 class="card-title">服務項目</h4>
        <p class="card-text">此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明。</p>
      </div>
    </div>
  </div>
</div>

{{< /example >}}

#### 純色文字卡 Masonry card
{{< example >}}
<div class="row d-flex justify-content-center">
  <div class="col-6">
    <div class="card bg-brand text-card border-dark">
      <div class="card-body">
        <h4 class="card-title">Brand Card</h4>
        <p>此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明。</p>
      </div>
    </div>
  </div>
</div>
<br/>
<div class="row d-flex justify-content-center">
  <div class="col-6">
    <div class="card bg-accent text-card border-dark">
      <div class="card-body">
        <h4 class="card-title">Accent Card</h4>
        <p>此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明。</p>
      </div>
    </div>
  </div>
</div>
<br/>
<div class="row d-flex justify-content-center">
  <div class="col-6">
    <div class="card bg-positive text-card border-dark">
      <div class="card-body">
        <h4 class="card-title">Positive Card</h4>
        <p>此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明。</p>
      </div>
    </div>
  </div>
</div>
<br/>
<div class="row d-flex justify-content-center">
  <div class="col-6">
    <div class="card bg-negative text-card border-dark">
      <div class="card-body">
        <h4 class="card-title">Negative Card</h4>
        <p>此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明。</p>
      </div>
    </div>
  </div>
</div>
<br>
<div class="row d-flex justify-content-center">
  <div class="col-6">
    <div class="card bg-information text-card border-dark">
      <div class="card-body">
        <h4 class="card-title">Information Card</h4>
        <p>此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明。</p>
      </div>
    </div>
  </div>
</div>
<br/>
<div class="row d-flex justify-content-center">
  <div class="col-6">
    <div class="card bg-warning text-card border-dark">
      <div class="card-body">
        <h4 class="card-title">Warning Card</h4>
        <p>此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明。</p>
      </div>
    </div>
  </div>
</div>
{{< /example >}}

#### 淡色文字卡 Masonry card
{{< example >}}
<div class="row d-flex justify-content-center">
  <div class="col-6">
    <div class="card bg-brand-container text-card border-dark">
      <div class="card-body">
        <h4 class="card-title">Brand Card</h4>
        <p>此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明。</p>
      </div>
    </div>
  </div>
</div>
<br/>
<div class="row d-flex justify-content-center">
  <div class="col-6">
    <div class="card bg-accent-container text-card border-dark">
      <div class="card-body">
        <h4 class="card-title">Accent Card</h4>
        <p>此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明。</p>
      </div>
    </div>
  </div>
</div>
<br/>
<div class="row d-flex justify-content-center">
  <div class="col-6">
    <div class="card bg-positive-container text-card border-dark">
      <div class="card-body">
        <h4 class="card-title">Positive Card</h4>
        <p>此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明。</p>
      </div>
    </div>
  </div>
</div>
<br/>
<div class="row d-flex justify-content-center">
  <div class="col-6">
    <div class="card bg-negative-container text-card border-dark">
      <div class="card-body">
        <h4 class="card-title">Negative Card</h4>
        <p>此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明。</p>
      </div>
    </div>
  </div>
</div>
<br>
<div class="row d-flex justify-content-center">
  <div class="col-6">
    <div class="card bg-information-container text-card border-dark">
      <div class="card-body">
        <h4 class="card-title">Information Card</h4>
        <p>此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明。</p>
      </div>
    </div>
  </div>
</div>
<br/>
<div class="row d-flex justify-content-center">
  <div class="col-6">
    <div class="card bg-warning-container text-card border-dark">
      <div class="card-body">
        <h4 class="card-title">Warning Card</h4>
        <p>此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明，此部分為服務項目之說明。</p>
      </div>
    </div>
  </div>
</div>
{{< /example >}}

#### 卡片加列表 Card with list group

卡片內容需要以列表呈現時，可以使用此元件。

{{< example >}}

<div class="row d-flex justify-content-center">
  <div class="col-md-5">
    <div class="card list-card">
      <div class="card-header">服務項目類別</div>
      <div class="card-body">
        <h4 class="card-title">標題</h4>
        <p class="card-text">卡片內文或補充說明。</p>
        <p class="card-text">1. 文字列表</p>
        <p class="card-text">2. 文字列表</p>
        <a href="#" class="btn btn-primary">按鈕</a>
      </div>
      <ul class="list-group list-group-flush">
        <li class="list-group-item"><i class="bi bi-award text-information icon"></i><a href="#">列表</a></li>
        <li class="list-group-item"><i class="bi bi-award text-information icon"></i><a href="#">列表</a></li>
        <li class="list-group-item"><i class="bi bi-award text-information icon"></i><a href="#">列表</a></li>
        <li class="list-group-item"><i class="bi bi-award text-information icon"></i><a href="#">列表</a></li>
      </ul>
    </div>
  </div>
  <div class="col-md-5">
    <div class="card list-card">
      <div class="card-header">服務項目類別</div>
      <div class="card-body card-bg-gary">
        <h4 class="card-title">標題</h4>
        <p class="card-text">卡片內文或補充說明。</p>
        <p class="card-text">1. 文字列表</p>
        <p class="card-text">2. 文字列表</p>
        <a href="#" class="btn btn-primary">按鈕</a>
      </div>
      <ul class="list-group border-0">
        <li class="list-group-item border-0"><i class="bi bi-award text-information icon"></i><a href="#">列表</a></li>
        <li class="list-group-item border-0"><i class="bi bi-award text-information icon"></i><a href="#">列表</a></li>
        <li class="list-group-item border-0"><i class="bi bi-award text-information icon"></i><a href="#">列表</a></li>
        <li class="list-group-item border-0"><i class="bi bi-award text-information icon"></i><a href="#">列表</a></li>
      </ul>
    </div>
  </div>
</div>
<br/>
<div class="row d-flex justify-content-center">
  <div class="col-md-5">
    <div class="card list-card">
      <div class="card-body">
        <h4 class="card-title">標題</h4>
        <p class="card-text">卡片內文或補充說明。</p>
        <p class="card-text">1. 文字列表</p>
        <p class="card-text">2. 文字列表</p>
        <a href="#" class="btn btn-primary">按鈕</a>
      </div>
      <ul class="list-group list-group-flush">
        <li class="list-group-item">列表</li>
        <li class="list-group-item">列表</li>
        <li class="list-group-item">列表</li>
        <li class="list-group-item">列表</li>
        <li class="list-group-item"><a href="#">額外連結</a><a href="#">額外連結</a><a href="#">額外連結</a></li>
      </ul>
    </div>
  </div>
  <div class="col-md-5">
    <div class="card list-card">
      <div class="card-header">服務項目類別</div>
      <img src="/docs/5.1/assets/img/bg-list-card.png" class="card-img-top" alt="...">  
      <div class="card-body card-bg-gary">
        <h4 class="card-title">標題</h4>
        <p class="card-text">卡片內文或補充說明。</p>
        <p class="card-text">1. 文字列表</p>
        <p class="card-text">2. 文字列表</p>
        <a href="#" class="btn btn-primary">按鈕</a>
      </div>
      <ul class="list-group border-0">
        <li class="list-group-item border-0"><i class="bi bi-award icon"></i><p class="d-inline">列表</p></li>
        <li class="list-group-item border-0"><i class="bi bi-award icon"></i><p class="d-inline">列表</p></li>
        <li class="list-group-item border-0"><i class="bi bi-award icon"></i><p class="d-inline">列表</p></li>
        <li class="list-group-item border-0"><i class="bi bi-award icon"></i><p class="d-inline">列表</p></li>
        <li class="list-group-item border-0"><a href="#">額外連結</a><a href="#">額外連結</a><a href="#">額外連結</a></li>
      </ul>
    </div>
  </div>
</div>

{{< /example >}}
