---
layout: docs
title: 圖標 Icons
description: 在文字的附近，協助其溝通意涵。
group: style
toc: true
---

## 關於圖示
圖示是一種在文字附近的視覺加強，通常用來幫助重述文字的意涵。除此之外，圖示也可以用來表達目前狀態或引導使用者進行某個動作，或是給予使用者動作之後的回饋。

## 預設圖示
本設計系統元件直接沿用 [Bootstrap Icons](https://icons.getbootstrap.com)，您可自行選用其他圖示庫 (icon library) 或自製 Icon 替換。在為元件替換 Icon 時請參考元件頁面的圖示大小 (size) 設計，注意不要放過大或過小的 Icon。

## 圖示易用性
**風格一致性** 讓您製作的整個網站使用類似風格的圖示，能降低使用者的學習成本，幫助他們更順利的使用您的網站。

**站內圖示一致性** 試著注意在您的網站上不同位置、頁面所使用的圖示一致性，這能減少使用者的認知負荷，幫助他們看過幾次圖示便能記得其代表的意涵。

## 範例：圖示一致性

<div class="row d-flex justify-content-center">
  <div class="col-md-4 g-3">
    <div class="card elevated">
      <img
        src="/docs/5.1/assets/img/Icon_02.png"
        class="card-img-top"
        alt="..." style="aspect-ratio: 3/2;"
      />
      <div class="card-body">
        <div class="badge-group">
            <span class="badge bg-positive-flat"><i class="bi bi-check-lg"></i><span>Do</span></span>
        </div>
        <div class="card-text">圖示用來輔助文字的溝通。</div>
      </div>
    </div>
  </div>
  <div class="col-md-4 g-3">
    <div class="card elevated">
      <img
        src="/docs/5.1/assets/img/Icon_01.png"
        class="card-img-top"
        alt="..." style="aspect-ratio: 3/2"
      />
      <div class="card-body">
        <div class="badge-group">
            <span class="badge bg-negative-flat"><i class="bi bi-x-lg"></i><span>Don't</span></span>
        </div>
        <div class="card-text">過多的圖示變化反而容易加重認知負荷</div>
      </div>
    </div>
  </div>
</div>

<div class="row d-flex justify-content-center">
  <div class="col-md-4 g-3">
    <div class="card elevated">
      <img
        src="/docs/5.1/assets/img/Icon_04.png"
        class="card-img-top"
        alt="..." style="aspect-ratio: 4/3;"
      />
      <div class="card-body">
        <div class="badge-group">
            <span class="badge bg-positive-flat"><i class="bi bi-check-lg"></i><span>Do</span></span>
        </div>
        <div class="card-text">類似意涵的地方用一樣的圖示有助於引導使用者迅速判斷。</div>
      </div>
    </div>
  </div>
    <div class="col-md-4 g-3">
    <div class="card elevated">
      <img
        src="/docs/5.1/assets/img/Icon_03.png"
        class="card-img-top"
        alt="..." style="aspect-ratio: 4/3"
      />
      <div class="card-body">
        <div class="badge-group">
            <span class="badge bg-negative-flat"><i class="bi bi-x-lg"></i><span>Don't</span></span>
        </div>
        <div class="card-text">用有些許差別的圖示表示類似的意涵容易加重認知負荷。</div>
      </div>
    </div>
  </div>
</div>

## 範例：圖示風格一致性

<div class="row d-flex justify-content-center">
  <div class="col-md-6 g-3">
    <div class="card elevated">
      <img
        src="/docs/5.1/assets/img/Icon_05.png"
        class="card-img-top"
        alt="..." style="aspect-ratio: 3/1;"
      />
      <div class="card-body">
        <div class="badge-group">
            <span class="badge bg-positive-flat"><i class="bi bi-check-lg"></i><span>Do</span></span>
        </div>
        <div class="card-text">Icon 風格都用視覺上一致的框線風格，且四個 Icon 的留白處比例都差不多。</div>
      </div>
    </div>
  </div>
  <div class="col-md-6 g-3">
    <div class="card elevated">
      <img
        src="/docs/5.1/assets/img/Icon_06.png"
        class="card-img-top"
        alt="..." style="aspect-ratio: 3/1"
      />
      <div class="card-body">
        <div class="badge-group">
            <span class="badge bg-negative-flat"><i class="bi bi-x-lg"></i><span>Don't</span></span>
        </div>
        <div class="card-text">有的 Icon 使用黑色填滿風格，有的 Icon 使用無填滿框線風格。</div>
      </div>
    </div>
  </div>
</div>