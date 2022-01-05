---
layout: docs
title: 頁首 Header
description: 頁首是一個網站的第一印象，一個好的頁首能提供使用者一目瞭然的整理，幫助使用者對網站的架構與規模有概念。清楚的架構能夠幫助使用者辨認出所在位置，並且被迅速地引導到達特定頁面。另一方面，頁首也扮演者當使用者迷路時可以總是找到並回到的地方。
group: components
toc: true
---

### 關於頁首元件
頁首是一個網站的第一印象，一個好的頁首能提供使用者一目瞭然的整理，幫助使用者對網站的架構與規模有概念。清楚的架構能夠幫助使用者辨認出所在位置，並且被迅速地引導到達特定頁面。另一方面，頁首也扮演者當使用者迷路時可以總是找到並回到的地方。

此設計系統將頁首可以分為三個區塊，每一區塊應有其適合放置的元素。

<img src="/img/header_navigation_illustration.png" alt="" width="50" height="40" class="d-inline-block"/>

**頁首主列** 最常見的頁首主列為 Logo 放置處。頁首應只放重要的服務項目，其他使用者較不常用的服務應一律放在頁尾。
**頁首副列** 當網站或是機關的服務項目較多時，建議將主列空出，並將服務項目分類、放到頁首副列。
**頁首上緣** 當需要放置操控整個網站的控制連結（例如語言切換、文字大小調整）時，可以自行加進頁首上緣。

### 使用規範

#### 何時該使用頁首
每個網站都應該有頁首。

#### 頁首易用性
**只將最重要的部分放在頁首。** 組織結構、服務一覽或是使用者較不常用但也存在的服務建議放在頁尾。
**避免組織結構導航。** 不要在頁首直接列出您的機構的組織結構。相反地，根據由使用者最常用服務、最常點的連結來建構您的頁首。
**使用簡短易懂的文字。** 使用簡短的文字，避免使用一般人難以理解的行話或術語。


### 設計元件

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

#### 基本加搜尋列 with search bar

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

#### 頁首加連結與下拉選單 Header with links and dropdown list

{{< example >}}

<nav class="navbar navbar-expand-lg bg-light">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">
      <img src="/docs/5.1/assets/brand/bootstrap-logo.svg" alt="" width="50" height="40" class="d-inline-block">
      標題
    </a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <i class="bi bi-list menu-icon"></i>選單
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <a class="nav-link" aria-current="page" href="#">連結</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">連結</a>
        </li>
        <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            下拉式選單
          </a>
          <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
            <li><a class="dropdown-item" href="#">連結</a></li>
            <li><a class="dropdown-item" href="#">連結</a></li>
            <li><a class="dropdown-item" href="#">連結</a></li>
          </ul>
        </li>
      </ul>
    </div>
  </div>
</nav>
{{< /example >}}

#### 頁首加許多連結 Header with many links
頁首連結多於三項時，建議放入頁首副列


### 範例 Example 

#### 簡單任務型網站

#### 大規模機關服務入口網

#### 字級操控與語言切換

#### 多國語言切換

#### 機關名稱與服務名稱

