---
layout: docs
title: 安裝教學 Setup
group: overview
toc: true
---

## 如何開始

PDIS 設計系統的架構是使用 Bootstrap 5 為基礎，經由修改一部分 SASS 來自訂風格呈現，因此如果你也有興趣使用，可先參考如下方式安裝後，按照 [風格](/docs/style/) 及 [元件](/docs/components) 文件所演示的方法使用。

## 我該如何選擇安裝方式

### jsDelivr CDN

使用 `jsDelivr` 依序導入 bootstrap 與 PDIS 設計系統

先導入bootstrap

```html
<!-- CSS -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">

<!-- JavaScript -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"></script>
```

導入 PDIS 設計系統

```html
<link href="https://cdn.jsdelivr.net/gh/pdis/design-system/dist/css/pdis-design-system.css" rel="stylesheet">
```

### 自行編譯

在 [Github](https://github.com/PDIS/design-system) 可找到所有我們新增的 SASS 檔案，打包下載之後，放到你的網站資料夾（如 `/site/assets/scss/` 之類的），並於你原有的自訂風格檔中（如 `style.scss`）新增一行引入 `@import "./pdis/general";` 即可。
