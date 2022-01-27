---
title: 使用說明
description: a user manual
layout: post
---

## 如何開始

PDIS 設計系統的架構是使用 Bootstrap 5 為基礎，經由修改一部分 SASS 來自訂風格呈現，因此如果你也有興趣使用，可先參考如下方式安裝後，按照 [風格](/docs/style/) 及 [元件](/docs/components) 文件所演示的方法使用。

## 我該如何選擇安裝方式

端看你的網站架構，安裝方式可以有如下幾種選擇：

1. 如果你目前正在使用 Bootstrap 5，且有使用 SASS 前處理器

在 https://github.com/PDIS/design-system/tree/main/site/assets/scss/pdis/ 可找到所有我們新增的 SASS 檔案，打包下載之後，放到你的網站資料夾（如 `/site/assets/scss/` 之類的），並於你原有的自訂風格檔中（如 `style.scss`）新增一行引入 `@import "./pdis/general";` 即可。

2. 目前正在使用 Bootstrap 5，但沒有使用 SASS 前處理器

移除原本 Bootstrap 引入 CSS 的標籤，並按照 3. 的指示取代該引入。

3. 目前沒有使用任何風格框架，純 HTML/CSS/JS 的狀態

在 https://github.com/PDIS/design-system/blob/gh-pages/docs/5.1/assets/css/docs.css 可找到我們新增並經過處理器運算過的 CSS 檔案，下載之後，放到你的網站資料夾（如 `/style/`），並於你的 HTML 中 `<head> </head>` 標籤之間新增一行 `<link href="/style/docs.css" rel="stylesheet">` 即可。

4. 目前正在使用其他風格框架

由於 Bootstrap 可能會與現有框架的 class 相衝突，建議可參考 [風格](/docs/style/) 及 [元件](/docs/components) 的範例，並修改原有框架的class 相關風格。
