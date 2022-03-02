---
layout: docs
title: 間距 (Spacing)
group: style
description: 一致性的間距能建立視覺平衡，讓使用者能更容易地瀏覽網頁。使用一致性的間距能提高UI品質。
toc: true
---

## 設計原則

我們沿用了bootstrap的間距設定為設計準則。

### 間距單位

一間距單位($spacer)為1rem(16px)，以0.25rem(4px)為單位增減。

### 間距單位符號

<table class="table">
  <thead>
    <tr>
      <th scope="col">Token</th>
      <th scope="col">rem</th>
      <th scope="col">px</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th scope="row">$spacers-1</th>
      <td>0.25</td>
      <td>4</td>
    </tr>
    <tr>
      <th scope="row">$spacers-2</th>
      <td>0.5</td>
      <td>8</td>
    </tr>
    <tr>
      <th scope="row">$spacers-3</th>
      <td>1</td>
      <td>16</td>
    </tr>
    <tr>
      <th scope="row">$spacers-4</th>
      <td>1.5</td>
      <td>24</td>
    </tr>
    <tr>
      <th scope="row">$spacers-5</th>
      <td>3</td>
      <td>48</td>
    </tr>
  </tbody>
</table>

### 使用間距單位符號

- 屬性
  - m - 設定 margin 的類別
  - p - 設定 padding 的類別

- 方向
  - t - 設定 margin-top 或是 padding-top 的類別
  - b - 設定 margin-bottom 或是 padding-bottom 的類別
  - s - 在 LTR 設定 margin-left 或是 padding-left， RTL 設定 margin-right 或是 padding-right
  - e - 在 LTR 設定 margin-right 或是 padding-right， RTL 設定 margin-left 或是 padding-left
  - x - 同時設定 *-left 和 *-right
  - y - 同時設定 *-top 和 *-bottom
  - 空白 - 同時設定 margin 或 padding 在元素的四個邊緣

- 間距
  - 0 - 設定 margin 或是 padding 為 0
  - 1 - 設定 margin 或是 padding 為 $spacer * .25
  - 2 - 設定 margin 或是 padding 為 $spacer * .5
  - 3 - 設定 margin 或是 padding 為 $spacer
  - 4 - 設定 margin 或是 padding 為 $spacer * 1.5
  - 5 - 設定 margin 或是 padding 為 $spacer * 3
  - auto - 設定 margin 為 auto


詳細資料可參考[bootstrap](https://getbootstrap.com/docs/5.1/utilities/spacing/)。



<!-- ### 配置間距 (Layout spacing)

元件與元件間的間距

<img class="img-fluid" src="https://i.imgur.com/mZlBVEk.png" >

## 元件間距 (Component spacing)

元件內的間距

<img class="img-fluid" src="https://i.imgur.com/sfF0oxj.png" >

## 文字間距 (Typography spacing)

文字與文字之間的間距

<img class="img-fluid" src="https://i.imgur.com/MrUjrdq.png" >

```
Body text: 1rem (16px)
Margin-top: 0
Heading margin-botttom: .5 rem (8px)
Paragraph margin-bottom: 1rem (16px)
```

## 間距集 (Spacing)

也可以繼續往上加，但一定要是 4 或 8 的倍數。
<img class="img-fluid" src="https://i.imgur.com/EAk6Q4W.png" > -->
