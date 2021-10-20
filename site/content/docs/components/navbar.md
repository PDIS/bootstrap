---
layout: docs
title: 導覽 - 頁首與頁尾 (header & footer)
group: components
toc: true
---

## 基本概念 (Basic concept)

「只」把網站最重要的目的放在頁首。

頁首可以分為三個區塊，每一區塊應有其適合放置的元素。
<img class="img-fluid" src="https://i.imgur.com/ymHyMJb.png" >

1. 頁首主列
   最常見的頁首主列為 Logo 放置處，網站功能明確且主要服務選單少於（或等於）三項時，頁首主列上可以直接將所有服務列出。反之，若網站為多功能網站，可預見服務選單多於三項時，建議將服務選項挪至頁首副列。

2. 頁首副列
   當網站或是機關的服務項目較多時，建議將主列空出，將服務項目網頁首的第二層級（即頁首副列）放置。

3. 頁首上緣
   另外，頁首上緣留有一小條空間，放置操控整個網站的控制連結，例如語言切換、文字大小調整。您可以決定此區塊是否需要。

除了重要服務項目或分類以外的連結，應一律放在頁尾，包括網站導覽、民意信箱等不常用服務。

## 頁首與頁尾 (header & footer)

### 基本頁首 (Base header)

基本頁首是頁首的基礎，其他的頁首變形皆由基本頁首開始。一個基本的頁首內容包含：機關 Logo 、中英文語言切換與字型大小切換。

{{< example >}}

<nav class="navbar navbar-light bg-white">
   <div class="container-fluid">
      <div class="navbar-top d-flex justify-content-end">
         <a href="#" class="text-white align-baseline px-1">大</a>
         <a href="#" class="text-white align-baseline px-1">中</a>
         <a href="#" class="text-white align-baseline px-1">小</a>
         <a href="#" class="text-white align-baseline px-2">English</a>
      </div>
   </div>
   <div class="container-fluid">
      <span class="navbar-brand h2 m-3" href="#">機關名稱</span>
   </div>
   <div class="container-fluid">
      <div class="navbar-bottom"></div>
   </div>
</nav>

{{< /example >}}

### 基本頁首加搜尋框 (Base header with search bar)

搜尋框位於頁首主列

{{< example >}}

<nav class="navbar navbar-light bg-white">
   <div class="container-fluid">
      <div class="navbar-top d-flex justify-content-end">
         <a href="#" class="text-white align-baseline px-1">大</a>
         <a href="#" class="text-white align-baseline px-1">中</a>
         <a href="#" class="text-white align-baseline px-1">小</a>
         <a href="#" class="text-white align-baseline px-2">English</a>
      </div>
   </div>
   <div class="container-fluid">
      <span class="navbar-brand h2 m-3" href="#">機關名稱</span>
      <form class="d-flex">
         <input type="text" class="form-control" placeholder="搜尋" aria-label="搜尋" aria-describedby="button-addon2">
         <button class="btn btn-outline-secondary bg-custom text-white" type="button" id="button-addon2"><i class="fa fa-search"></i></button>
      </form>
   </div>
   <div class="container-fluid">
      <div class="navbar-bottom"></div>
   </div>
</nav>

{{< /example >}}

### 基本頁首加服務選單 (Base header with service menu)

服務選單少於三項時可以置於頁首主列

{{< example >}}

<nav class="navbar navbar-expand-lg navbar-light bg-white">
   <div class="container-fluid">
      <div class="navbar-top d-flex justify-content-end">
         <a href="#" class="text-white align-baseline px-1 navbar-top-item">大</a>
         <a href="#" class="text-white align-baseline px-1 navbar-top-item">中</a>
         <a href="#" class="text-white align-baseline px-1 navbar-top-item">小</a>
         <a href="#" class="text-white align-baseline px-2 navbar-top-item">English</a>
      </div>
   </div>
   <div class="container-fluid">
      <span class="navbar-brand h2 m-3" href="#">機關名稱</span>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
         <span class="navbar-toggler-icon text-white">選單</span>
      </button>
      <div class="collapse navbar-collapse navbar-menu" id="navbarNav">
         <ul class="navbar-nav">
            <li class="nav-item">
               <a class="nav-link navbar-link-item" href="#">服務項目</a>
            </li>
            <li class="nav-item">
               <a class="nav-link navbar-link-item" href="#">服務項目</a>
            </li>
         </ul>
      </div>
   </div>
   <div class="container-fluid">
      <div class="navbar-bottom"></div>
   </div>
</nav>

{{< /example >}}

依據需求可以將服務分類，用下拉式選單收納

{{< example >}}

<nav class="navbar navbar-expand-lg navbar-light bg-white">
   <div class="container-fluid">
      <div class="navbar-top d-flex justify-content-end">
         <a href="#" class="text-white align-baseline px-1">大</a>
         <a href="#" class="text-white align-baseline px-1">中</a>
         <a href="#" class="text-white align-baseline px-1">小</a>
         <a href="#" class="text-white align-baseline px-2">English</a>
      </div>
   </div>
   <div class="container-fluid">
      <span class="navbar-brand h2 m-3" href="#">機關名稱</span>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
         <span class="navbar-toggler-icon text-white">選單</span>
      </button>
      <div class="collapse navbar-collapse navbar-menu" id="navbarNav">
         <ul class="navbar-nav">
            <li class="nav-item">
               <a class="nav-link navbar-link-item" href="#">服務項目</a>
            </li>
            <li class="nav-item">
               <a class="nav-link navbar-link-item" href="#">服務項目</a>
            </li>
            <li class="nav-item dropdown">
               <a class="nav-link dropdown-toggle navbar-link-item" href="#" id="navbarDarkDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  服務分類
               </a>
               <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="navbarDarkDropdownMenuLink">
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
               </ul>
            </li>
         </ul>
      </div>
   </div>
   <div class="container-fluid">
      <div class="navbar-bottom"></div>
   </div>
</nav>

{{< /example >}}

{{< example >}}

<nav class="navbar navbar-expand-lg navbar-light bg-white">
   <div class="container-fluid">
      <div class="navbar-top d-flex justify-content-end">
         <a href="#" class="text-white align-baseline px-1">大</a>
         <a href="#" class="text-white align-baseline px-1">中</a>
         <a href="#" class="text-white align-baseline px-1">小</a>
         <a href="#" class="text-white align-baseline px-2">English</a>
      </div>
   </div>
   <div class="container-fluid">
      <span class="navbar-brand h2 m-3" href="#">機關名稱</span>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
         <span class="navbar-toggler-icon text-white">選單</span>
      </button>
      <div class="collapse navbar-collapse navbar-menu" id="navbarNav">
         <ul class="navbar-nav">
            <li class="nav-item dropdown">
               <a class="nav-link dropdown-toggle navbar-link-item" href="#" id="navbarDarkDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  服務分類
               </a>
               <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="navbarDarkDropdownMenuLink">
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
               </ul>
            </li>
            <li class="nav-item dropdown">
               <a class="nav-link dropdown-toggle navbar-link-item" href="#" id="navbarDarkDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  服務分類
               </a>
               <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="navbarDarkDropdownMenuLink">
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
               </ul>
            </li>
         </ul>
      </div>
   </div>
   <div class="container-fluid">
      <div class="navbar-bottom"></div>
   </div>
</nav>

{{< /example >}}

只要在選單總數少於獲等於三項時，都可以這樣將選單放置在頁首主列處理。

{{< example >}}

<nav class="navbar navbar-expand-lg navbar-light bg-white">
   <div class="container-fluid">
      <div class="navbar-top d-flex justify-content-end">
         <a href="#" class="text-white align-baseline px-1">大</a>
         <a href="#" class="text-white align-baseline px-1">中</a>
         <a href="#" class="text-white align-baseline px-1">小</a>
         <a href="#" class="text-white align-baseline px-2">English</a>
      </div>
   </div>
   <div class="container-fluid">
      <span class="navbar-brand h2 m-3" href="#">機關名稱</span>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
         <span class="navbar-toggler-icon text-white">選單</span>
      </button>
      <div class="collapse navbar-collapse navbar-menu" id="navbarNav">
         <ul class="navbar-nav">
            <li class="nav-item dropdown">
               <a class="nav-link dropdown-toggle navbar-link-item" href="#" id="navbarDarkDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  服務分類
               </a>
               <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="navbarDarkDropdownMenuLink">
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
               </ul>
            </li>
            <li class="nav-item dropdown">
               <a class="nav-link dropdown-toggle navbar-link-item" href="#" id="navbarDarkDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  服務分類
               </a>
               <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="navbarDarkDropdownMenuLink">
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
               </ul>
            </li>
            <li class="nav-item dropdown">
               <a class="nav-link dropdown-toggle navbar-link-item" href="#" id="navbarDarkDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  服務分類
               </a>
               <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="navbarDarkDropdownMenuLink">
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
               </ul>
            </li>
         </ul>
      </div>
   </div>
   <div class="container-fluid">
      <div class="navbar-bottom"></div>
   </div>
</nav>

{{< /example >}}

### 多服務頁首 (Multi-services header)

當服務選單多於三項時，建議將服務分類並移到頁首副列。

{{< example >}}

<nav class="navbar navbar-expand-lg navbar-light bg-white">
   <div class="container-fluid">
      <div class="navbar-top d-flex justify-content-end">
         <a href="#" class="text-white align-baseline px-1">大</a>
         <a href="#" class="text-white align-baseline px-1">中</a>
         <a href="#" class="text-white align-baseline px-1">小</a>
         <a href="#" class="text-white align-baseline px-2">English</a>
      </div>
   </div>
   <div class="container-fluid">
      <span class="navbar-brand h2 m-3" href="#">機關名稱</span>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
         <span class="navbar-toggler-icon text-white">選單</span>
      </button>
   </div>
   <div class="container-fluid">
      <div class="navbar-bottom"></div>
   </div>
   <div class="container-fluid">
      <div class="collapse navbar-collapse" id="navbarNav">
         <ul class="navbar-nav">
            <li class="nav-item">
               <a class="nav-link navbar-link-item" href="#">服務項目</a>
            </li>
            <li class="nav-item">
               <a class="nav-link navbar-link-item" href="#">服務項目</a>
            </li>
            <li class="nav-item">
               <a class="nav-link navbar-link-item" href="#">服務項目</a>
            </li>
            <li class="nav-item dropdown">
               <a class="nav-link dropdown-toggle navbar-link-item" href="#" id="navbarDarkDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  服務分類
               </a>
               <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="navbarDarkDropdownMenuLink">
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
               </ul>
            </li>
         </ul>
      </div>
   </div>
</nav>

{{< /example >}}

{{< example >}}

<nav class="navbar navbar-expand-lg navbar-light bg-white">
   <div class="container-fluid">
      <div class="navbar-top d-flex justify-content-end">
         <a href="#" class="text-white align-baseline px-1">大</a>
         <a href="#" class="text-white align-baseline px-1">中</a>
         <a href="#" class="text-white align-baseline px-1">小</a>
         <a href="#" class="text-white align-baseline px-2">English</a>
      </div>
   </div>
   <div class="container-fluid">
      <span class="navbar-brand h2 m-3" href="#">機關名稱</span>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
         <span class="navbar-toggler-icon text-white">選單</span>
      </button>
   </div>
   <div class="container-fluid">
      <div class="navbar-bottom"></div>
   </div>
   <div class="container-fluid">
      <div class="collapse navbar-collapse" id="navbarNav">
         <ul class="navbar-nav">
            <li class="nav-item dropdown">
               <a class="nav-link dropdown-toggle navbar-link-item" href="#" id="navbarDarkDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  服務分類
               </a>
               <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="navbarDarkDropdownMenuLink">
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
               </ul>
            </li>
            <li class="nav-item dropdown">
               <a class="nav-link dropdown-toggle navbar-link-item" href="#" id="navbarDarkDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  服務分類
               </a>
               <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="navbarDarkDropdownMenuLink">
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
               </ul>
            </li>
            <li class="nav-item dropdown">
               <a class="nav-link dropdown-toggle navbar-link-item" href="#" id="navbarDarkDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  服務分類
               </a>
               <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="navbarDarkDropdownMenuLink">
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
               </ul>
            </li>
            <li class="nav-item dropdown">
               <a class="nav-link dropdown-toggle navbar-link-item" href="#" id="navbarDarkDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  服務分類
               </a>
               <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="navbarDarkDropdownMenuLink">
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
               </ul>
            </li>
         </ul>
      </div>
   </div>
</nav>

{{< /example >}}

{{< example >}}

<nav class="navbar navbar-expand-lg navbar-light bg-white">
   <div class="container-fluid">
      <div class="navbar-top d-flex justify-content-end">
         <a href="#" class="text-white align-baseline px-1">大</a>
         <a href="#" class="text-white align-baseline px-1">中</a>
         <a href="#" class="text-white align-baseline px-1">小</a>
         <a href="#" class="text-white align-baseline px-2">English</a>
      </div>
   </div>
   <div class="container-fluid">
      <span class="navbar-brand h2 m-3" href="#">機關名稱</span>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
         <span class="navbar-toggler-icon text-white">選單</span>
      </button>
   </div>
   <div class="container-fluid">
      <div class="navbar-bottom"></div>
   </div>
   <div class="container-fluid">
      <div class="collapse navbar-collapse" id="navbarNav">
         <ul class="navbar-nav">
            <li class="nav-item dropdown">
               <a class="nav-link dropdown-toggle navbar-link-item" href="#" id="navbarDarkDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  服務分類
               </a>
               <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="navbarDarkDropdownMenuLink">
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
               </ul>
            </li>
            <li class="nav-item dropdown">
               <a class="nav-link dropdown-toggle navbar-link-item" href="#" id="navbarDarkDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  服務分類
               </a>
               <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="navbarDarkDropdownMenuLink">
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
               </ul>
            </li>
            <li class="nav-item dropdown">
               <a class="nav-link dropdown-toggle navbar-link-item" href="#" id="navbarDarkDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  服務分類
               </a>
               <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="navbarDarkDropdownMenuLink">
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
               </ul>
            </li>
            <li class="nav-item dropdown">
               <a class="nav-link dropdown-toggle navbar-link-item" href="#" id="navbarDarkDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  服務分類
               </a>
               <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="navbarDarkDropdownMenuLink">
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
               </ul>
            </li>
            <li class="nav-item dropdown">
               <a class="nav-link dropdown-toggle navbar-link-item" href="#" id="navbarDarkDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  服務分類
               </a>
               <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="navbarDarkDropdownMenuLink">
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
               </ul>
            </li>
            <li class="nav-item dropdown">
               <a class="nav-link dropdown-toggle navbar-link-item" href="#" id="navbarDarkDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  服務分類
               </a>
               <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="navbarDarkDropdownMenuLink">
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
               </ul>
            </li>
            <li class="nav-item dropdown">
               <a class="nav-link dropdown-toggle navbar-link-item" href="#" id="navbarDarkDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  服務分類
               </a>
               <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="navbarDarkDropdownMenuLink">
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
               </ul>
            </li>
         </ul>
      </div>
   </div>
</nav>

{{< /example >}}

### 多服務頁首加搜尋框 (Multi-services header with search bar)

搜尋框仍保持靠右，位於頁首主列。

{{< example >}}

<nav class="navbar navbar-expand-lg navbar-light bg-white">
   <div class="container-fluid">
      <div class="navbar-top d-flex justify-content-end">
         <a href="#" class="text-white align-baseline px-1">大</a>
         <a href="#" class="text-white align-baseline px-1">中</a>
         <a href="#" class="text-white align-baseline px-1">小</a>
         <a href="#" class="text-white align-baseline px-2">English</a>
      </div>
   </div>
   <div class="container-fluid">
      <span class="navbar-brand h2 m-3" href="#">機關名稱</span>
      <form class="d-flex">
         <input type="text" class="form-control" placeholder="搜尋" aria-label="搜尋" aria-describedby="button-addon2">
         <button class="btn btn-outline-secondary bg-custom text-white" type="button" id="button-addon2"><i class="fa fa-search"></i></button>
      </form>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
         <span class="navbar-toggler-icon text-white">選單</span>
      </button>
   </div>
   <div class="container-fluid">
      <div class="navbar-bottom"></div>
   </div>
   <div class="container-fluid">
      <div class="collapse navbar-collapse" id="navbarNav">
         <ul class="navbar-nav">
            <li class="nav-item dropdown">
               <a class="nav-link dropdown-toggle navbar-link-item" href="#" id="navbarDarkDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  服務分類
               </a>
               <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="navbarDarkDropdownMenuLink">
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
               </ul>
            </li>
            <li class="nav-item dropdown">
               <a class="nav-link dropdown-toggle navbar-link-item" href="#" id="navbarDarkDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  服務分類
               </a>
               <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="navbarDarkDropdownMenuLink">
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
               </ul>
            </li>
            <li class="nav-item dropdown">
               <a class="nav-link dropdown-toggle navbar-link-item" href="#" id="navbarDarkDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  服務分類
               </a>
               <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="navbarDarkDropdownMenuLink">
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
               </ul>
            </li>
            <li class="nav-item dropdown">
               <a class="nav-link dropdown-toggle navbar-link-item" href="#" id="navbarDarkDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  服務分類
               </a>
               <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="navbarDarkDropdownMenuLink">
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
               </ul>
            </li>
            <li class="nav-item dropdown">
               <a class="nav-link dropdown-toggle navbar-link-item" href="#" id="navbarDarkDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  服務分類
               </a>
               <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="navbarDarkDropdownMenuLink">
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
               </ul>
            </li>
            <li class="nav-item dropdown">
               <a class="nav-link dropdown-toggle navbar-link-item" href="#" id="navbarDarkDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  服務分類
               </a>
               <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="navbarDarkDropdownMenuLink">
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
               </ul>
            </li>
            <li class="nav-item dropdown">
               <a class="nav-link dropdown-toggle navbar-link-item" href="#" id="navbarDarkDropdownMenuLink" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                  服務分類
               </a>
               <ul class="dropdown-menu dropdown-menu-dark" aria-labelledby="navbarDarkDropdownMenuLink">
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
                  <li><a class="dropdown-item" href="#">服務項目</a></li>
               </ul>
            </li>
         </ul>
      </div>
   </div>
</nav>

{{< /example >}}

### 響應式設計

手機上的頁首應保持將機關 Logo 靠左。不論 Logo 為方形或長形，一律靠左。頁首右側放置漢堡選單 (hammburger button)。另外，依據需求，網站開發者或是機關可以自行決定是否在手機版的頁首上放入搜尋框。

<img class="img-fluid" src="https://i.imgur.com/OxDKdx2.png" >

### 頁尾

頁尾也如同頁首的概念，分成三個區塊。

<img class="img-fluid" src="https://i.imgur.com/LnTRapg.png" >

1. 返回上方

   此列可自由選保留或拿掉。

2. 頁尾副列

   這邊放的是服務選單。您可以選擇將頁尾的服務選單簡單處理，只列舉幾個常用的。或是窮舉所有服務。

3. 頁尾主列

   頁尾主列是頁尾的主要區塊，可以放置機關的 Logo 與名稱，以及必要放在頁尾的標章（如無障礙標章）、連結（如市長信箱）與文字（如機關地址電話）。這邊也可以選擇放置社群媒體的連結。

### 基本頁尾

{{< example >}}

<div class="container-fluid">
   <footer>
      <div class="row bg-light">
         <!-- <div class="navbar-menu" id="navbarNav">
            <ul class="navbar-nav">
               <li class="nav-item">
                  <a class="nav-link navbar-link-item" href="#">服務項目</a>
               </li>
               <li class="nav-item">
                  <a class="nav-link navbar-link-item" href="#">服務項目</a>
               </li>
            </ul>
         </div> -->
      </div>
      <div class="row bg-footer p-3">
         <div class="col-4 d-flex justify-content-center align-items-center">
            <div class="row" >
               <div class="col-4">
                  <img src="/docs/5.1/assets/brand/bootstrap-logo.svg" class="img-fluid" alt="">
               </div>
                <div class="col-8 align-self-center">
                  <p class="h4">機關名稱</p>
               </div>
            </div>
         </div>
         <div class="col-4">
            <div class="row">
               <p>地址 : 地址地址地址地址地址地址地址 電話 : 1234567</p>
            </div>
            <div class="row">
               <a href="#" >政府網站資料開放宣告</a>
               <a href="#" >市民信箱</a>
               <a href="#" >隱私權及資訊安全政策</a>
            </div>
         </div>
         <div class="col-4 align-self-center">
            <img src="https://accessibility.ncc.gov.tw/ImagesUploads/e367c753-b88e-4a08-a167-84d54029a88a.jpg" class="img-fluid" alt="">
         </div>
      </div>
  </footer>
</div>

{{< /example >}}

### 基本頁尾加返回上方

{{< example >}}

<div class="container-fluid">
   <footer>
      <div class="row bg-white text-center">
         <div class="col-12">
            <button class="btn">
               <i class="bi bi-arrow-up-circle-fill" style="font-size: 1.1rem; color: cornflowerblue;"></i>
               <a href="#" class="link-primary">回上方</a>
            </button>
         </div>
      </div>
      <div class="row bg-light">
         <!-- <div class="navbar-menu" id="navbarNav">
            <ul class="navbar-nav">
               <li class="nav-item">
                  <a class="nav-link navbar-link-item" href="#">服務項目</a>
               </li>
               <li class="nav-item">
                  <a class="nav-link navbar-link-item" href="#">服務項目</a>
               </li>
            </ul>
         </div> -->
      </div>
      <div class="row bg-footer p-3">
         <div class="col-4 d-flex justify-content-center align-items-center">
            <div class="row" >
               <div class="col-4">
                  <img src="/docs/5.1/assets/brand/bootstrap-logo.svg" class="img-fluid" alt="">
               </div>
                <div class="col-8 align-self-center">
                  <p class="h4">機關名稱</p>
               </div>
            </div>
         </div>
         <div class="col-4">
            <div class="row">
               <p>地址 : 地址地址地址地址地址地址地址 電話 : 1234567</p>
            </div>
            <div class="row">
               <a href="#" >政府網站資料開放宣告</a>
               <a href="#" >市民信箱</a>
               <a href="#" >隱私權及資訊安全政策</a>
            </div>
         </div>
         <div class="col-4 align-self-center">
            <img src="https://accessibility.ncc.gov.tw/ImagesUploads/e367c753-b88e-4a08-a167-84d54029a88a.jpg" class="img-fluid" alt="">
         </div>
      </div>
  </footer>
</div>

{{< /example >}}

### 頁尾含所有服務

### 常見服務與社群媒體

### 頁尾含所有服務與社群媒體
