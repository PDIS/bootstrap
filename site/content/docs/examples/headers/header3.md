---
layout: components-example
---

{{< example >}}
<nav class="navbar navbar-expand-lg navbar-light bg-light">
  <div class="container">
    <a class="navbar-brand d-flex align-items-center" href="#">
      <img src="/img/pdis-logo-final-inverse.png" width="32" height="32" alt="logo" class="rounded">
      <span class="navbar-title h3">標題</span>
    </a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
    </button>
		<div class="collapse navbar-collapse align-items-end" id="navbarSupportedContent">
      <ul class="navbar-nav ms-auto">
        <li class="nav-item dropdown">
          <button type="button" class="btn btn-primary dropdown-toggle" data-bs-toggle="dropdown" aria-expanded="false">服務項目</button>
          <div class="dropdown-menu">
          <ul aria-labelledby="navbarDropdown1">
            <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
            <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
            <li><a class="dropdown-item disabled">下拉選單第一層標題文字</a></li>
          </ul>
                 <ul aria-labelledby="navbarDropdown1">
            <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
            <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
            <li><a class="dropdown-item disabled">下拉選單第一層標題文字</a></li>
          </ul>
        </li>
				<li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown2" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            下拉式選單
          </a>
          <ul class="dropdown-menu" aria-labelledby="navbarDropdown2">
            <li><a class="dropdown-item" href="#">子項目</a></li>
            <li><a class="dropdown-item" href="#">子項目</a></li>
            <li><a class="dropdown-item" href="#">子項目</a></li>
          </ul>
        </li>
				<li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown3" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            下拉式選單
          </a>
          <ul class="dropdown-menu" aria-labelledby="navbarDropdown3">
            <li><a class="dropdown-item" href="#">子項目</a></li>
            <li><a class="dropdown-item" href="#">子項目</a></li>
            <li><a class="dropdown-item" href="#">子項目</a></li>
          </ul>
        </li>
      </ul>
    </div>
  </div>
</nav>
{{< /example >}}