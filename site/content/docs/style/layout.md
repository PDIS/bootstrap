---
layout: docs
title: 排版 Layout
description: 在文字的附近，協助其溝通意涵。
group: style
toc: true
---

## HTML區塊

使用語意化來區隔功能的結構，也有利於SEO搜尋。

### 網站結構

網站結構選擇分為以下兩種，分為有aside與沒aside，排版如下

### HTML範例

#### 沒有 aside

{{< example >}}
<header>
  Header
  <nav class="container">Navbar</nav>
</header>
<div class="container">
  <main>Main</main>
</div>
<footer>Footer</footer>

<style>
.bd-example > header, .bd-example > header > nav, .bd-example > .container > main, .bd-example > section, .bd-example > aside, .bd-example > footer {
  padding: 0.5rem;
  background-color: LightGray;
  border: 0.2rem solid white;
  text-align: center;
  box-sizing: border-box;
} 
.bd-example > .container > main {
  height: 200px;
  margin: 0 -12px;
}
</style>
{{< /example >}}

#### 有 aside

{{< example >}}
<header>
  Header
  <nav class="container">nav</nav>
</header>
<div class="container">
  <div class="row">
    <aside class="col-12 col-md-4 col-lg-3">SideBar</aside>
    <main class="col-12 col-md-8 col-lg-9">Main</main>
  </div>
</div>
<footer>Footer</footer>

<style>
.bd-example > .container > div > main, .bd-example > .container > div > aside {
  height: 200px;
  padding: 0.5rem;
  background-color: LightGray;
  border: 0.2rem solid white;
  text-align: center;
  box-sizing: border-box;
}
</style>
{{< /example >}}

## 斷點 Breakpoint

斷點用於控制排版如何在不同的設備大小進行響應式的變化，本設計系統沿用 Bootstrap 在斷點的設計。

### 概念
- 斷點作為響應式開發的基礎。使用斷點來控制在特定尺寸或設備上調整佈局。
- 使用 media queries 的斷點構建 CSS。 media queries 是 CSS 的一個特性，它允許您根據瀏覽器和操作系統參數有條件地套用樣式。我們最常在 media queries 中使用 min-width.
- 在響應式開發中，主要會以行動版為優先。 Bootstrap 的 CSS 旨在使用最少的樣式來使佈局在最小的斷點處工作，然後在樣式上分層以針對較大的設備調整該設計。這樣可以優化CSS，縮短渲染時間，並為訪問者提供出色的體驗。

### 斷點選項

{{< bs-table "table" >}}
| 斷點 | Class 中綴 | 寬度 |
|---|---|---|
| X-Small  | 無  | <576px  |
| Small  | sm  |  ≥576px |
| Medium  | md  | ≥ 768px  |
| Large  | lg  | ≥ 992px  |
| Extra large  | xl  |  ≥ 1200px |
| Extra extra large  | xxl  | ≥1400px  |
{{< /bs-table >}}

## 容器 Container

容器作為基本建構區塊，在不同大小的裝置中包含、填充和對齊你的內容

### 容器選項

容器作為最基本的布局元素，可以在下表比較各段點

{{< bs-table "table" >}}
|  | &lt;576px | &ge;576px | &ge;768px | &ge;992px | &ge;1200px | &ge;1400px |
| --- | --- | --- | --- | --- | --- | --- |
| `.container` | <span class="text-muted">100%</span> | 540px | 720px | 960px | 1140px | 1320px |
| `.container-sm` | <span class="text-muted">100%</span> | 540px | 720px | 960px | 1140px | 1320px |
| `.container-md` | <span class="text-muted">100%</span> | <span class="text-muted">100%</span> | 720px | 960px | 1140px | 1320px |
| `.container-lg` | <span class="text-muted">100%</span> | <span class="text-muted">100%</span> | <span class="text-muted">100%</span> | 960px | 1140px | 1320px |
| `.container-xl` | <span class="text-muted">100%</span> | <span class="text-muted">100%</span> | <span class="text-muted">100%</span> | <span class="text-muted">100%</span> | 1140px | 1320px |
| `.container-xxl` | <span class="text-muted">100%</span> | <span class="text-muted">100%</span> | <span class="text-muted">100%</span> | <span class="text-muted">100%</span> | <span class="text-muted">100%</span> | 1320px |
| `.container-fluid` | <span class="text-muted">100%</span> | <span class="text-muted">100%</span> | <span class="text-muted">100%</span> | <span class="text-muted">100%</span> | <span class="text-muted">100%</span> | <span class="text-muted">100%</span> |
{{< /bs-table >}}

### 容器選擇
Bootstrap 提供了7種container選擇，為了統一呈現效果，我們建議使用 `.container` 與 `.container-fluid`。

#### 預設容器
預設使用 `.container`，這是一個響應式、固定寬度的容器，在每個斷點處都會改變寬度。

<!-- {{< example >}}
<div>
  <div class="container">
    .container
  </div>
</div>

<style>
.bd-example > div > .container {
  background: LightGray;
  height: 100%;
}
</style>
{{< /example >}} -->

#### 全寬容器
使用 `.container-fluid` 全寬容器，在任何裝置寬度皆採用最大寬度。

<!-- {{< example >}}
<div>
  <div class="container-fluid">
    .container-fluid
  </div>
</div>

<style>
.bd-example > div > .container-fluid {
  background: LightGray;
  height: 100%;
}
</style>
{{< /example >}} -->

## 網格 Grid

網格使用 flexbox 在各種尺寸的網頁排版，包含12個欄位、6個響應式斷點

### 如何運作

Bootstrap 的網格系統使用容器、行、列、欄來進行排版與對齊，並使用 flexbox 建構來達成響應式網站。

{{< callout info >}}
若不熟悉 flexbox，可以閱讀 [flexbox 指南](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
{{< /callout >}}

{{< example >}}
<div class="grid-example">
  <div class="container-fluid">
    <div class="row">
      <div class="col">
        <p>1/3</p>
      </div>
      <div class="col">
        <p>1/3</p>
      </div>
      <div class="col">
        <p>1/3</p>
      </div>
    </div>
  </div>
</div>

<style>
.grid-example {
  background: none;
  height: 100%;
}

.bd-example > .grid-example > .container-fluid > div > div > p {
  border-radius:10px;
  background-color: #005AA8;
  color: white;
  text-align: center;
  font-size: 2rem;
  height: 100px;
  line-height: 100px;
}
</style>
{{< /example >}}

### 網格選項
Bootstrap 的網格系統會採用以下六種斷點，各斷點欄位數量皆為12，並且欄位間距為上1.5rem、左0.75rem、右0.75rem。

<div class="table-responsive">
  <table class="table mb-4">
    <thead>
      <tr>
        <th scope="col"></th>
        <th scope="col">
          xs<br>
          <span class="fw-normal">&lt;576px</span>
        </th>
        <th scope="col">
          sm<br>
          <span class="fw-normal">&ge;576px</span>
        </th>
        <th scope="col">
          md<br>
          <span class="fw-normal">&ge;768px</span>
        </th>
        <th scope="col">
          lg<br>
          <span class="fw-normal">&ge;992px</span>
        </th>
        <th scope="col">
          xl<br>
          <span class="fw-normal">&ge;1200px</span>
        </th>
        <th scope="col">
          xxl<br>
          <span class="fw-normal">&ge;1400px</span>
        </th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <th class="text-nowrap" scope="row">容器最大寬度</th>
        <td>無(自動)</td>
        <td>540px</td>
        <td>720px</td>
        <td>960px</td>
        <td>1140px</td>
        <td>1320px</td>
      </tr>
      <tr>
        <th class="text-nowrap" scope="row">Class 前綴</th>
        <td><code>.col-</code></td>
        <td><code>.col-sm-</code></td>
        <td><code>.col-md-</code></td>
        <td><code>.col-lg-</code></td>
        <td><code>.col-xl-</code></td>
        <td><code>.col-xxl-</code></td>
      </tr>
    </tbody>
  </table>
</div>

### 使用指南

Bootstrap 提供了六個斷點，我們建議只使用以下三種斷點作為不同大小裝置的排版與設計。

<div class="table-responsive">
  <table class="table mb-4">
    <thead>
      <tr>
        <th scope="col"></th>
        <th scope="col">
          xs<br>
          <span class="fw-normal">&lt;768px</span>
        </th>
        <th scope="col">
          md<br>
          <span class="fw-normal">&ge;768px</span>
        </th>
        <th scope="col">
          lg<br>
          <span class="fw-normal">&ge;992px</span>
        </th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <th class="text-nowrap" scope="row">class 前綴</th>
        <td><code>.col-</code></td>
        <td><code>.col-md-</code></td>
        <td><code>.col-md-lg</code></td>
      </tr>
      <tr>
        <th class="text-nowrap" scope="row">裝置</th>
        <td>手機</td>
        <td>平板</td>
        <td>電腦</td>
      </tr>
    </tbody>
  </table>
</div>

在版面設計上，建議以全滿、1/2、1/3、1/4來完成排版。

<div class="table-responsive">
  <table class="table mb-4">
    <thead>
      <tr>
        <th scope="col"></th>
        <th scope="col">
          全滿</span>
        </th>
        <th scope="col">
          1/2</span>
        </th>
        <th scope="col">
          1/3</span>
        </th>
        <th scope="col">
          1/4</span>
        </th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <th class="text-nowrap" scope="row">class</th>
        <td><code>.col-</code></td>
        <td><code>.col-6</code></td>
        <td><code>.col-4</code></td>
        <td><code>.col-3</code></td>
      </tr>
    </tbody>
  </table>
</div>

### 欄位間距

預設欄位間距為：上1.5rem、左0.75rem、右0.75rem，並建議使用預設值，若要修改可參考 [Bootstrap 之 Gutters 設定](https://getbootstrap.com/docs/5.1/layout/gutters/)。

### 各種寬度

#### 全滿

{{< example >}}
<div class="grid-example">
  <div class="container-fluid">
    <div class="row">
      <div class="col">
        <p>全滿</p>
      </div>
    </div>
  </div>
</div>
{{< /example >}}

#### 二分之一

{{< example >}}
<div class="grid-example">
  <div class="container-fluid">
    <div class="row">
      <div class="col-6">
        <p>1/2</p>
      </div>
      <div class="col-6">
        <p>1/2</p>
      </div>
    </div>
  </div>
</div>
{{< /example >}}

#### 三分之一

{{< example >}}
<div class="grid-example">
  <div class="container-fluid">
    <div class="row">
      <div class="col-4">
        <p>1/3</p>
      </div>
      <div class="col-8">
        <p>2/3</p>
      </div>
    </div>
  </div>
</div>
{{< /example >}}

#### 四分之一

{{< example >}}
<div class="grid-example">
  <div class="container-fluid">
    <div class="row">
      <div class="col-3">
        <p>1/4</p>
      </div>
      <div class="col-9">
        <p>3/4</p>
      </div>
    </div>
  </div>
</div>
{{< /example >}}