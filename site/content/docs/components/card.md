---
layout: docs
title: 卡片 (Card)
description: 卡片是一個常用來彙整或列舉資訊的呈現方式。
group: components
toc: true
---

## About the card component

卡片是一個常用來彙整或列舉資訊的方式，一個基本的卡片可以將特定主題的內容與行動放在一個容器裡。一張卡面上通常可以有標題、圖片、文字段落、列表、按鈕與連結。卡片通常是另一個更詳細資訊頁面的入口，使用者在點擊卡片之後會被帶往更多資訊的面進行下一步動作。

{{< example >}}

<div class="card" style="width: 18rem;">
  {{< placeholder width="100%" height="180" class="card-img-top" text="圖片" >}}
  <div class="card-body">
    <h5 class="card-title">標題文字</h5>
    <p class="card-text">此部分為卡片之內文。</p>
  </div>
</div>

{{< /example >}}

{{< example >}}

<div class="row">
  <div class="col-md-4">
    <div class="card">
      {{< placeholder width="100%" height="180" class="card-img-top" text="圖片" >}}
      <div class="card-body">
        <h5 class="card-title">標題文字</h5>
        <p class="card-text">此部分為卡片之內文。</p>
      </div>
    </div>
  </div>
  <div class="col-md-4">
    <div class="card text-center">
      {{< placeholder width="100%" height="180" class="card-img-top" text="圖片" >}}
      <div class="card-body">
        <h5 class="card-title">標題文字</h5>
        <p class="card-text">此部分為卡片之內文。</p>
      </div>
    </div>
  </div>
</div>

{{< /example >}}

{{< example >}}

<div class="card" style="width: 18rem;">
  <div class="card-body">
    <h5 class="card-title">標題文字</h5>
    <p class="card-text">此部分為卡片之內文。</p>
  </div>
  {{< placeholder width="100%" height="180" class="card-img-top" text="圖片" >}}
</div>

{{< /example >}}

{{< example >}}

<div class="card" style="width: 18rem;">
  {{< placeholder width="100%" height="180" class="card-img-top" text="圖片" >}}
  <div class="card-body">
    <h5 class="card-title">標題文字</h5>
    <p class="card-text">此部分為卡片之內文。</p>
    <a href="#" class="btn btn-primary">前往報名</a>
  </div>
</div>

{{< /example >}}
