---
layout: docs
title: 導覽列下拉選單 Navigation Dropdowns
description: 讓使用者從多個頁面選項中做一個或選擇，並跳轉到其選擇的頁面。
group: components
toc: true
---

## 關於導覽列下拉選單元件

導覽列的下拉選單是導覽的延伸。與常駐的導覽列不同，導覽列下拉選單是短暫的存在，依據使用者的互動輸入，觸發展開選單內容，並可以再次出發收納選單內容。使用者在選單展開時，可以從多個選項中做出單一選擇，選擇的目的是用來前往別的分頁。到達新的分頁後，下拉選單則自動收納起來，整個網頁回到原導覽列的常駐狀態。

## 使用規範

### 何時該使用導覽列下拉選單

當導覽列有需要用到下拉式選單收納頁面連結，總數量不至於過多且層級（不含導覽列）不超過兩層時，請妥善利用導覽列下拉選單。

### 何時該考慮使用其他元件

- **選項過少。** 當連結數目不多，例如小於 3，且導覽列空間足夠時，建議直接將連結展開放置在導覽列上，供使用者一目了然的瀏覽並選擇想要前往的頁面。
- **選項過多。** 當選單內的項目太多，例如超過 15 項時，請先主動重新檢視網站的資訊架構。若無法更動，請參考 sidebar 搭配 header navigation 的呈現方式，避免用單一導覽列下拉選單一次收納過多資訊。否則，將過多內容收納在一處將會增加使用者的查找負擔。
- **選單數目過多。** 當導覽列上的導覽列下拉選單數量過多，甚至導覽列上每個連結都是用下拉選單呈現時，請參考 sidebar 搭配 header navigation 的呈現方式。

### 導覽列下拉選單易用性

- **導覽列與下拉選單風格應一致。** 導覽列與其下拉選單皆為導覽用，其風格應一致，幫助使用者的潛在認知，降低額外學習成本。
- **導覽列與下拉選單底色區別。** 建議在導覽列的底色與下拉選單的底色使用不同顏色以作區別。因為下拉選單是暫時出現且蓋過背後網頁內容的元件，與常駐的導覽列顏色稍作區別，能幫助使用者在瀏覽網頁時的潛在認知。
- **避免不要的特效。** 下拉選單的內容可以直接覆蓋在原網頁的內容之上，請避免另外製作非必要的特效，例如逐項展開選單，或將網頁內容下推等。
- **避免選項數量過多。** 建議不要放超過 15 個選擇。

### 導覽列下拉選單近用性

- **避免使用 hover。** 請避免用 hover 觸發展開選單，儘量使用 click 觸發，以減少視覺負擔。

## 元件設計

### 基本款下拉選單 Basic Dropdowns

基本款的下拉選單包括按鈕與選單。按鈕右側一律有向下的圖標作為引導。選單的寬度跟著文字的內容長度變化。

{{< example >}}
<header>
  <nav class="navbar navbar-expand-md">
    <div class="container">
      <a class="navbar-brand" href="/" aria-label="PDIS">
      網站名稱
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#Navbar" aria-controls="Navbar" aria-expanded="true" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="navbar-collapse collapse" id="Navbar">
        <ul class="navbar-nav">
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle" href="#" id="DropdownMenu1" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              服務項目
            </a>
            <ul class="dropdown-menu" aria-labelledby="DropdownMenu1">
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
            </ul>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</header>
{{< /example >}}

### 副標題 Sub-heading

從基本款下拉選單的樣式延伸，可以將選單內連結分類並加上副標題。

{{< example >}}
<header>
  <nav class="navbar navbar-expand-md">
    <div class="container">
      <a class="navbar-brand" href="/" aria-label="PDIS">
      網站名稱
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#Navbar" aria-controls="Navbar" aria-expanded="true" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="navbar-collapse collapse" id="Navbar">
        <ul class="navbar-nav">
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle" href="#" id="DropdownMenu1" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              服務項目
            </a>
            <ul class="dropdown-menu" aria-labelledby="DropdownMenu1">
              <li><a class="dropdown-item dropdown-item-title unclickable">副標題名稱</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li class="dropdown-divider"></li>
              <li><a class="dropdown-item dropdown-item-title unclickable">副標題名稱</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
            </ul>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</header>
{{< /example >}}

### 橫向 Horizontal

次主題的分類可以橫向排列。

{{< example >}}
<header>
  <nav class="navbar navbar-expand-md">
    <div class="container">
      <a class="navbar-brand" href="/" aria-label="PDIS">
      網站名稱
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#Navbar" aria-controls="Navbar" aria-expanded="true" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="navbar-collapse collapse" id="Navbar">
        <ul class="navbar-nav">
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle" href="#" id="DropdownMenu1" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              服務項目
            </a>
            <ul class="dropdown-menu" style="width: max-content" aria-labelledby="DropdownMenu1">
              <li class="row">
                <ul class="col-md-6">
                  <li><a class="dropdown-item dropdown-item-title unclickable">副標題名稱</a></li>
                  <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
                  <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
                  <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
                </ul>
                <ul class="col-md-6">
                  <li><a class="dropdown-item dropdown-item-title unclickable">副標題名稱</a></li>
                  <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
                  <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
                  <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
                </ul>
              </li>
            </ul>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</header>
{{< /example >}}

### 顏色 Colour

依據預設背景的顏色，下拉選單也有三種不同填色。

{{< example >}}
<header>
  <nav class="navbar navbar-expand-md">
    <div class="container">
      <a class="navbar-brand" href="/" aria-label="PDIS">
      網站名稱
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#Navbar" aria-controls="Navbar" aria-expanded="true" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="navbar-collapse collapse" id="Navbar">
        <ul class="navbar-nav">
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle" href="#" id="DropdownMenu1" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              服務項目
            </a>
            <ul class="dropdown-menu" aria-labelledby="DropdownMenu1">
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
            </ul>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</header>
<header>
  <nav class="navbar navbar-expand-md bg-surface">
    <div class="container navbar-brand-container">
      <a class="navbar-brand" href="/" aria-label="PDIS">
      網站名稱
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#Navbar" aria-controls="Navbar" aria-expanded="true" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="navbar-collapse collapse" id="Navbar">
        <ul class="navbar-nav">
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle" href="#" id="DropdownMenu1" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              服務項目
            </a>
            <ul class="dropdown-menu" aria-labelledby="DropdownMenu1">
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
            </ul>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</header>
<header>
  <nav class="navbar navbar-expand-md bg-brand-flat">
    <div class="container">
      <a class="navbar-brand" href="/" aria-label="PDIS">
      網站名稱
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#Navbar" aria-controls="Navbar" aria-expanded="true" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="navbar-collapse collapse" id="Navbar">
        <ul class="navbar-nav">
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle" href="#" id="DropdownMenu1" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              服務項目
            </a>
            <ul class="dropdown-menu" aria-labelledby="DropdownMenu1">
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
            </ul>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</header>
{{< /example >}}

### 無效 Disabled

按鈕有不同狀態，除了預設、Hover 、Pressed 以外，也可以是無效狀態。

{{< example >}}
<header>
  <nav class="navbar navbar-expand-md">
    <div class="container">
      <a class="navbar-brand" href="/" aria-label="PDIS">
      網站名稱
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#Navbar" aria-controls="Navbar" aria-expanded="true" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="navbar-collapse collapse" id="Navbar">
        <ul class="navbar-nav">
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle" href="#" id="DropdownMenu1" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              服務項目
            </a>
            <ul class="dropdown-menu" aria-labelledby="DropdownMenu1">
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
            </ul>
          </li>
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle disabled" href="#" id="DropdownMenu1" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              服務項目
            </a>
            <ul class="dropdown-menu" aria-labelledby="DropdownMenu1">
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
            </ul>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</header>
<header>
  <nav class="navbar navbar-expand-md bg-surface">
    <div class="container navbar-brand-container">
      <a class="navbar-brand" href="/" aria-label="PDIS">
      網站名稱
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#Navbar" aria-controls="Navbar" aria-expanded="true" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="navbar-collapse collapse" id="Navbar">
        <ul class="navbar-nav">
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle" href="#" id="DropdownMenu1" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              服務項目
            </a>
            <ul class="dropdown-menu" aria-labelledby="DropdownMenu1">
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
            </ul>
          </li>
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle disabled" href="#" id="DropdownMenu1" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              服務項目
            </a>
            <ul class="dropdown-menu" aria-labelledby="DropdownMenu1">
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
            </ul>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</header>
<header>
  <nav class="navbar navbar-expand-md bg-brand-flat">
    <div class="container">
      <a class="navbar-brand" href="/" aria-label="PDIS">
      網站名稱
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#Navbar" aria-controls="Navbar" aria-expanded="true" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="navbar-collapse collapse" id="Navbar">
        <ul class="navbar-nav">
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle" href="#" id="DropdownMenu1" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              服務項目
            </a>
            <ul class="dropdown-menu" aria-labelledby="DropdownMenu1">
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
            </ul>
          </li>
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle disabled" href="#" id="DropdownMenu1" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              服務項目
            </a>
            <ul class="dropdown-menu" aria-labelledby="DropdownMenu1">
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
            </ul>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</header>
{{< /example >}}

### 文字標籤 Text Label

文字標籤的變形有在左側加上圖標的標型，或是只有圖標沒有文字的變形。純文字搬遷為預設樣式，也用於大部分常見情境。文字與左側 icon 則是在有對應的 icon 可以加強使用者使用上的理解度才會放置。純 icon 則是在 icon 單獨存在就足以讓使用者完全理解時才使用。

{{< example >}}
<header>
  <nav class="navbar navbar-expand-md">
    <div class="container">
      <a class="navbar-brand" href="/" aria-label="PDIS">
      網站名稱
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#Navbar" aria-controls="Navbar" aria-expanded="true" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="navbar-collapse collapse" id="Navbar">
        <ul class="navbar-nav">
          <li class="nav-item dropdown order-2 order-md-1">
            <a class="nav-link dropdown-toggle" href="#" id="DropdownMenu1" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              服務項目
            </a>
            <ul class="dropdown-menu" aria-labelledby="DropdownMenu1">
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
            </ul>
          </li>
          <li class="nav-item dropdown order-1 order-md-2">
            <a class="nav-link dropdown-toggle dropdown-toggle-icon d-none d-md-block" href="#" id="DropdownSearch" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              <i class="bi bi-search"></i>
            </a>
            <div class="dropdown-menu search-menu" aria-labelledby="DropdownSearch">
              <span class="dropdown-menu-title d-none d-md-block">使用關鍵字搜尋網站</span>
              <div class="input-group">
                <input type="text" class="form-control" id="Input1" placeholder="請輸入關鍵字">
                <div class="input-group-append">
                  <button class="btn btn-brand" type="button"><i class="bi bi-search"></i></button>
                </div>
              </div>
              <div class="dropdown-divider d-none d-md-block"></div>
              <div style="padding: 0.75rem 0.5rem">
                <span class="d-inline d-md-block">熱門關鍵字</span>
                <a href="#">國家科學技術發展計畫</a>
                <a href="#">申辦流程</a>
                <a href="#">啟動法規鬆綁</a>
              </div>
            </div>
          </li>
          <li class="nav-item dropdown ms-md-auto order-3">
            <a class="nav-link dropdown-toggle d-none d-md-block" href="#" id="DropdownSetting" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              <i class="bi bi-gear"></i><span>網站設定 / Setting</span>
            </a>
            <ul class="dropdown-menu setting-menu" aria-labelledby="DropdownSetting">
              <li><a class="dropdown-item dropdown-item-header unclickable">網站設定 Setting</a></li>
              <li><a class="dropdown-item dropdown-item-title unclickable">語言 Language</a></li>
              <li>
                <select class="form-select" id="LanguageSelect" aria-label="LanguageSelect">
                  <option selected>請選擇一個選項</option>
                  <option value="zh-tw">繁體中文</option>
                  <option value="en-us">English (US</option>
                  <option value="en-uk">English (UK)</option>
                  <option value="jp">Japanese</option>
                  <option value="th">Thai</option>
                </select>
              </li>
              <li><a class="dropdown-item dropdown-item-title unclickable">文字大小</a></li>
              <li>
                <div class="btn-group" role="group" aria-label="Font size">
                  <button type="button" class="btn btn-brand">小</button>
                  <button type="button" class="btn btn-brand">預設</button>
                  <button type="button" class="btn btn-brand">大</button>
                </div>
              </li>
            </ul>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</header>
{{< /example >}}