---
layout: components-example
---

{{< example >}}
<header>
  <nav class="navbar navbar-expand-md">
    <div class="container">
      <a class="navbar-brand" href="/" aria-label="PDIS">
        <img class="navbar-logo" src="/docs/5.1/assets/img/logo.png" alt="logo" height="100%">
<!--         <div class="d-inline-block align-top">
          <span class="navbar-brand-title">網站名稱</span>
          <span class="navbar-brand-title d-none d-md-block"></span>
        </div> -->
      </a>
      <button class="navbar-toggler collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#Navbar" aria-controls="Navbar" aria-expanded="true" aria-label="Toggle navigation">
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
          <li class="nav-item dropdown order-2 order-md-1">
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
          <li class="nav-item dropdown order-2 order-md-1">
            <a class="nav-link dropdown-toggle" href="#" id="DropdownMenu3" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              服務項目
            </a>
            <ul class="dropdown-menu" aria-labelledby="DropdownMenu3">
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
            </ul>
          </li>
          <li class="nav-item dropdown order-2 order-md-1">
            <a class="nav-link dropdown-toggle" href="#" id="DropdownMenu4" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              服務項目
            </a>
            <ul class="dropdown-menu" aria-labelledby="DropdownMenu4">
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
              <li><a class="dropdown-item" href="#">下拉選單第一層標題文字</a></li>
            </ul>
          </li>
          <li class="nav-item dropdown order-1 order-md-2">
            <a class="nav-link dropdown-toggle d-none d-md-block" href="#" id="DropdownSearch" role="button" data-bs-toggle="dropdown" aria-expanded="false">
              <i class="bi bi-search"></i>
            </a>
            <div class="dropdown-menu search-menu" aria-labelledby="DropdownSearch">
              <span class="dropdown-menu-title d-none d-md-block">使用關鍵字搜尋網站</span>
              <div class="input-group">
                <input type="text" class="form-control" id="Input1" placeholder="請輸入關鍵字">
                <div class="input-group-append">
                  <button class="btn btn-secondary" type="button"><i class="bi bi-search"></i></button>
                </div>
              </div>
              <div class="dropdown-divider d-none d-md-block"></div>
              <div class="hot-searching">
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
              <li><a class="dropdown-item dropdown-item-header">網站設定 Setting</a></li>
              <li><a class="dropdown-item dropdown-item-title">語言 Language</a></li>
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
              <li><a class="dropdown-item dropdown-item-title">文字大小</a></li>
              <li>
                <div class="btn-group" role="group" aria-label="Font size">
                  <button type="button" class="btn btn-secondary">小</button>
                  <button type="button" class="btn btn-secondary">預設</button>
                  <button type="button" class="btn btn-secondary">大</button>
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