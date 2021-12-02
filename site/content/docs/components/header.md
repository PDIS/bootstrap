---
layout: docs
title: 頁首 Header
description: 頁首是一個網站的第一印象，一個好的頁首能提供使用者一目瞭然的整理，幫助使用者對網站的架構與規模有概念。清楚的架構能夠幫助使用者辨認出所在位置，並且被迅速地引導到達特定頁面。另一方面，頁首也扮演者當使用者迷路時可以總是找到並回到的地方。
group: components
toc: true
---

### 頁首易用性 Header usibility

列出所有網站中的重要部分，放在頁首的連結區。
若是大型網站，使用下拉選單收納較低層級的連結，輔助預覽。
如果較低層級的連結之間彼此相關，且使用者必須在這些連結之間頻繁切換，請考慮使用側邊導航。
使用簡短的文字，避免使用一般人難以理解的行話或術語。
避免組織結構導航。不要在頁首直接列出您的機構的組織結構。相反地，根據由使用者最常用服務、最常點的連結來建構您的頁首。
只將最重要的部分放在頁首。組織結構、服務一覽或是使用者較不常用但也存在的服務建議放在頁尾。
強烈建議透過使用者訪談與測試與使用者一起研究頁首區塊的內容。

此設計系統將頁首可以分為三個區塊，每一區塊應有其適合放置的元素。
**頁首主列** 最常見的頁首主列為 Logo 放置處。頁首應只放重要的服務項目，其他使用者較不常用的服務應一律放在頁尾。
**頁首副列** 當網站或是機關的服務項目較多時，建議將主列空出，並將服務項目分類、放到頁首副列。
**頁首上緣** 當需要放置操控整個網站的控制連結（例如語言切換、文字大小調整）時，可以自行加進頁首上緣。

#### 基本頁首 Base header

{{< example >}}

<nav class="navbar navbar-light bg-light">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">
      <img src="/docs/5.1/assets/brand/bootstrap-logo.svg" alt="" width="50" height="40" class="d-inline-block">
      標題
    </a>
  </div>
</nav>

{{< /example >}}

#### 變形 Variation

#### 加搜尋列 with search bar

{{< example >}}

<nav class="navbar navbar-light bg-light">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">
      <img src="/docs/5.1/assets/brand/bootstrap-logo.svg" alt="" width="50" height="40" class="d-inline-block">
      標題
    </a>
    <form class="d-flex">
      <input type="text" class="form-control" placeholder="" aria-label="Username">
      <span class="input-group-text"><i class="bi bi-search"></i></span>
    </form>
  </div>
</nav>
{{< /example >}}

#### 加連結與下拉選單 with links dropdown list

{{< example >}}

<nav class="navbar navbar-light bg-light">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">
      <img src="/docs/5.1/assets/brand/bootstrap-logo.svg" alt="" width="50" height="40" class="d-inline-block">
      標題
    </a>
  </div>
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
</nav>
{{< /example >}}
