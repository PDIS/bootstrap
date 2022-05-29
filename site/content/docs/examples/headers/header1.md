---
layout: components-example
---

{{< example >}}
<header class="navbar navbar-expand-xxl">
  <nav aria-label="Main navigation">
    <div class="container navbar-brand-container">
      <a class="navbar-brand" href="/" aria-label="PDIS">
      網站名稱
      </a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#Navbar" aria-controls="Navbar" aria-expanded="true" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
    </div>
    <div class="navbar-collapse collapse" id="Navbar">
      <div class="container">
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
            <a class="nav-link dropdown-toggle" href="#" id="DropdownMenu2" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              服務項目
            </a>
            <ul class="dropdown-menu" aria-labelledby="DropdownMenu2">
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
            </ul>
          </li>
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle dropdown-toggle-iconless" href="#" id="DropdownSearch" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              <i class="bi bi-search"></i>
            </a>
            <div class="dropdown-menu search-menu" aria-labelledby="DropdownSearch">
              <span>使用關鍵字搜尋網站</span>
              <div class="input-group">
                <input type="text" class="form-control" id="Input1" placeholder="請輸入關鍵字">
                <span class="input-group-text" id="search">搜尋</span>
              </div>
              <span>熱門關鍵字</span>
              <ul><li><a href="">國家科學技術發展計畫</a></li><li>申辦流程</li></ul>
            </div>
          </li>
          <li class="nav-item dropdown ms-auto">
            <a class="nav-link dropdown-toggle dropdown-toggle-iconless bg-brand-flat" href="#" id="DropdownSetting" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              <i class="bi bi-gear"></i>網站設定 / Setting
            </a>
            <ul class="dropdown-menu" aria-labelledby="DropdownSetting">
              <li><a class="dropdown-item">下拉選單第一層標題文字<a></li>
              <li><a class="dropdown-item" href="#">繁體中文</a></li>
              <li><a class="dropdown-item" href="#">English (US)</a></li>
              <li><a class="dropdown-item" href="#">English (UK)</a></li>
              <li><a class="dropdown-item" href="#">Japanese</a></li>
              <li><a class="dropdown-item" href="#">Thai</a></li>
              <li><a class="dropdown-item">文字大小<a></li>
              <li class="text-center">
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