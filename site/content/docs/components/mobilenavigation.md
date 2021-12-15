---
layout: docs
title: 行動導覽 Mobile Navigation
description: 行動裝置上的主要導覽
group: components
toc: true
---

### 關於行動導覽

在行動裝置如手機、平板上的空間較一般螢幕少，導覽元件的重要性也相對提高許多。如何在有限的空間內、有限的點擊次數內，協助使用者順利的找到相對應的服務，且不會迷航，即為行動導覽的主要功能與存在目的。

#### 以「服務」與「資訊」出發的資訊架構

在一般政府機關的網站中，常常會按照組織架構分類服務項目，例如局處 A 提供服務項目 A1, A1, A3, 局處 B 提供項目 B1, B2, B3。在我們的設計系統中，我們相信民眾應該能夠直接、快速、簡便的找到自己想要到達服務，即便是在不需要知道整體組織結構的情況下。特別是在行動裝置上的使用，通常需要提供的是更即時、更直接的服務。
因此，在我們的設計系統中，歸納出了在政府機關的行動導覽中較常出現的選單名稱：「服務」與「資訊」。「服務」為民眾可以直接進入，有直接需求的服務。這邊我們建議可以超越分組的限制，將所有以民眾的角度出發會常用到的服務列出，例如 A1, B1, A2, A3, B3。實際範例則為：「借還書」、「線上申辦借書證」等服務項目，儘管這兩項服務可能為不同分組負責。「資訊」則為提供民眾做為一般資訊查找用，且請儘量僅列出常用且可以想見會在行動中較長使用的資訊，例如：「圖書館位置」、「開館時間」等等。我們極力建議將機關所欲提供的資訊分為「服務」與「資訊」兩類，從這兩個選項出發，以利使用者能夠直接到達所需服務。

### 使用規範

#### When to use the mobile navigation component

行動導覽提供行動裝置上的主要導覽。因為行動裝置上空間較為珍貴，通常不會有太多空間讓次要導覽（如：側邊欄）出現，所以行動導覽本身就是主要的導覽，也常常是唯一的導覽方式。

#### 何時該考慮使用其他元件

**架構過於繁雜。** 當架構過於繁雜時，建議在製作網站之前先重新檢視資訊架構，刪除不必要在行動裝置上出現的資訊。
**架構過於簡單。** 當架構過於簡單時，可以省略行動導覽的使用，而直接以單頁滾動的方式呈現資訊。

### 設計元件

#### 基本款 下拉式行動導覽 vs 側欄式行動導覽

依據服務項目的多寡，基本款可以選擇下拉式行動導覽或側欄式行動導覽。下拉式行動導覽適合服務項目少的網站，包含元素有機關名稱、商標 (logo)、選單與搜尋按鈕，互動選單展開後則包含各式機關所屬服務以及語言切換。側欄式行動導覽適合服務項目多的網站，互動選單展開後則包含搜尋功能、語言切換功能以及所有服務項目。一般來說，服務項目七項以下為服務項目少，大於七項則為服務項目多。但機關可以依狀況自行決定，例如件服務項目第一層不足七項，但計算其子項目後大於七項，則仍可以使用側欄式行動導覽。

{{< example >}}

<div class="row">
  <div class="col-md-6">
    <nav class="navbar bg-light">
      <a class="navbar-brand" href="#">
        <img src="/docs/5.1/assets/brand/bootstrap-logo.svg" alt="" width="50" height="40" class="d-inline-block">
        標題
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbar1" aria-controls="navbar1" aria-expanded="false" aria-label="Toggle navigation">
        <i class="bi bi-list menu-icon"></i>選單
      </button>
      <div class="collapse navbar-collapse" id="navbar1">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">服務項目</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">服務項目</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">服務項目</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">服務項目</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">服務項目</a>
          </li>
        </ul>
        <hr>
        <div class="d-flex flex-row-reverse">
          <a class="nav-link" href="#">中文/English</a>
        </div>
      </div>
    </nav>
  </div>
  <div class="col-md-6">
    <nav class="navbar bg-light">
      <a class="navbar-brand" href="#">
        <img src="/docs/5.1/assets/brand/bootstrap-logo.svg" alt="" width="50" height="40" class="d-inline-block">
        標題
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="offcanvas" data-bs-target="#offcanvasNavbar" aria-controls="offcanvasNavbar">
        <i class="bi bi-list menu-icon"></i>選單
      </button>
      <div class="offcanvas offcanvas-end" tabindex="-1" id="offcanvasNavbar" aria-labelledby="offcanvasNavbarLabel">
        <div class="offcanvas-header">
          <a class="offcanvas-title" id="offcanvasNavbarLabel"><i class="bi bi-house-fill icon"></i>回首頁</a>
          <button type="button" class="btn-close btn-close-white  text-reset" data-bs-dismiss="offcanvas" aria-label="Close"></button>
        </div>
        <div class="offcanvas-body">
          <ul class="navbar-nav justify-content-end flex-grow-1">
            <li class="nav-item dropdown">
              <a class="nav-link dropdown-toggle" href="#" id="Dropdown1" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                服務項目(擁有子項目)
              </a>
              <ul class="dropdown-menu" aria-labelledby="Dropdown1">
                <li><a class="dropdown-item" href="#">服務子項目</a></li>
                <li><a class="dropdown-item" href="#">服務子項目</a></li>
              </ul>
            </li>
            <li class="nav-item dropdown">
              <a class="nav-link dropdown-toggle" href="#" id="Dropdown2" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                服務項目(擁有子項目)
              </a>
              <ul class="dropdown-menu" aria-labelledby="Dropdown2">
                <li><a class="dropdown-item" href="#">服務子項目</a></li>
                <li><a class="dropdown-item" href="#">服務子項目</a></li>
              </ul>
            </li>
            <li class="nav-item dropdown">
              <a class="nav-link dropdown-toggle" href="#" id="Dropdown3" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                服務項目(擁有子項目)
              </a>
              <ul class="dropdown-menu" aria-labelledby="Dropdown3">
                <li><a class="dropdown-item" href="#">服務子項目</a></li>
                <li><a class="dropdown-item" href="#">服務子項目</a></li>
              </ul>
            </li>
            <li class="nav-item dropdown">
              <a class="nav-link dropdown-toggle" href="#" id="Dropdown4" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                服務項目(擁有子項目)
              </a>
              <ul class="dropdown-menu" aria-labelledby="Dropdown4">
                <li><a class="dropdown-item" href="#">服務子項目</a></li>
                <li><a class="dropdown-item" href="#">服務子項目</a></li>
              </ul>
            </li>
            <li class="nav-item dropdown">
              <a class="nav-link dropdown-toggle" href="#" id="Dropdown5" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                服務項目(擁有子項目)
              </a>
              <ul class="dropdown-menu" aria-labelledby="Dropdown5">
                <li><a class="dropdown-item" href="#">服務子項目</a></li>
                <li><a class="dropdown-item" href="#">服務子項目</a></li>
              </ul>
            </li>
          </ul>
          <hr>
          <p>搜尋關鍵字</p>
          <div class="input-group">
            <input type="text" class="form-control" placeholder="" aria-label="Search">
            <span class="input-group-text"><i class="bi bi-search"></i></span>
          </div>
          <p>熱門搜尋：<a href="#">防疫政策</a></p>
        </div>
      </div>
    </nav>
  </div>
</div>
{{< /example >}}

{{< example >}}

<div class="row">

    <nav class="navbar navbar-expand-lg bg-light">
                <a class="navbar-brand" href="#">
        <img src="/docs/5.1/assets/brand/bootstrap-logo.svg" alt="" width="50" height="40" class="d-inline-block">
        標題
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbar1" aria-controls="navbar1" aria-expanded="false" aria-label="Toggle navigation">
        <i class="bi bi-list menu-icon"></i>選單
      </button>
      <div class="collapse navbar-collapse" id="navbar1">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">服務項目</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">服務項目</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">服務項目</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">服務項目</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="page" href="#">服務項目</a>
          </li>
        </ul>
        <hr>
        <div class="d-flex flex-row-reverse">
          <a class="nav-link" href="#">中文/English</a>
        </div>
      </div>

    </nav>

</div>

{{< /example >}}
