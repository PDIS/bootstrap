---
layout: docs
title: 版面配置 (Layout)
description: 做版面配置時，若參考同一套基準，可以幫助我們設計具有一致性的視覺體驗的介面。以下為此設計系統關於版面配置的建議，作為數位系統製作與設計時的參考。
group: style
toc: true
---

## 概述

在做版面配置時，建議採用以 4 為倍數的網格與間距系統。在各種螢幕尺寸上，採用同樣以 4 為倍數的參考基準，可以幫助我們設計具有一致性的視覺體驗的介面。

### 基本配置

配置版面時，物件彼此之間的間距可以採用 4 像素 (4px) 或是 8 像素 (8px) 為倍數的間距系統。當在決定比較大規模的版面配置時，建議以 8 像素為基礎的間距系統來思考，而在決定較為細緻的物件內的版面配置時（例如製作按鈕 Button、圖標 Icon 時），建議以 4 像素為基礎思考。

### 容器 (Containers)

在介面設計上，容器指的是一個可以容納一定範圍所有元件的概念。容器大致上可以分類為兩種：固定容器 (fixed container) 和 流動容器 (fluid container)。若使用固定容器，通常內容物會在延展到一個最大值之後停止延展，而通常這個最大寬度為 1280 px。若使用流動容器，隨著對不同視窗斷點 (break point) 拉伸，容器內的所有物件會延展並且佔滿整個視窗寬度。容器的選用通常會與斷點搭配。一般建議在設計大螢幕的介面使用固定容器，小螢幕則使用流動容器。

#### 固定容器 & 流動容器 (Fixed & Fluid container)

- [x] Fixed Container
      <img class="img-fluid" src="https://i.imgur.com/pIUHJed.png" >

- [x] Fluid Container
      <img class="img-fluid" src="https://i.imgur.com/3zLdXcQ.png" >

## 響應式排版 (Responsive layout)

### 欄位, 間隙, 外邊距 (Columns, Gutters, Margins)

- [x] Columns, Gutters, Margins
      <img class="img-fluid" src="https://i.imgur.com/3ktORVm.png" >

### 斷點 (Breakpoints)

斷點用於控制版面配置，在不同的設備或視窗大小進行響應式變化。我們列出以下的斷點作為使用本設計系統時的設計參考。斷點是響應式開發的基礎，一般實作上，我們會使用斷點來控制在特定尺寸視窗或設備上的版面配置。

- [x] 斷點 (Breakpoints)
      <img class="img-fluid" src="https://i.imgur.com/RTdYjkJ.png" >

```
之後表格再更新，先使用bootstrap的截圖版
```
