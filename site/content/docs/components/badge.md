---
layout: docs
title: 標籤
description: 標籤可以為其他元件新增說明文字或數字。
group: components
---

## 關於標籤

標籤內容通常較短，是一個小型元件。標籤通常不會單獨存在，而是為其他元件新增說明文字，或是以數字協助計數。

## 使用規範

### 何時該使用標籤

- **吸引目光到最新或是重要項目。** 例如在多個標題中，其中一個標題後面加上「Live 直播中」的標籤。
- **幫助篩選多個擁有不同標籤的元件。** 例如在搜尋的列表上，每個搜尋結果都附上一些分類標籤，例如「歐洲」、「美洲」以協助使用者篩選。
- **示意一個容器中有幾個新項目。** 例如在個人帳號管理區有個「個人訊息」功能，並以標籤示意還有幾則剛寄達或未讀的訊息。

### 何時該考慮使用其他元件

- **避免與按鈕混淆。** 避免將標籤與頁面上的按鈕區放太近，以防混淆。
- **定期更新內容。** 如果使用者可以預期定期更新內容，則可以考慮另闢一區專門放更新。例如「今日天氣」可以自成一區，而不是每天都用標籤新增說明。

## 元件設計

### 基本款標籤 Basic badge

基本款的標籤以打淡的品牌色 (Brand Flat) 為背景色。標籤是補充說明用的小塊資訊，通常用在提示分類、屬性或是計數。使用者常以標籤上的資訊作為依據，進行下一步動作。

{{< example >}}

<div class="row text-center">
  <div class="col">
    <span class="badge bg-brand-flat">Badge</span>
  </div>
</div>

{{< /example >}}

### 角色 Role

從基本款按鈕的樣式延伸，共六種不同角色的標籤，由左至右分別為：主要、強調、次要、正向、負向、資訊、警告。

{{< example >}}

<div class="row text-center">
  <div class="col g-3">
    <span class="badge bg-brand-flat">Brand</span>
  </div>
  <div class="col g-3">
    <span class="badge bg-accent-flat">Accent</span>
  </div>
  <div class="col g-3">
    <span class="badge bg-secondary-flat">Secondary</span>
  </div>
  <div class="col g-3">
    <span class="badge bg-positive-flat">Postive</span>
  </div>
  <div class="col g-3">
    <span class="badge bg-negative-flat">Negative</span>
  </div>
  <div class="col g-3">
    <span class="badge bg-info-flat">Info</span>
  </div>
  <div class="col g-3">
    <span class="badge bg-warning-flat">Warning</span>
  </div>
</div>

{{< /example >}}

### 計數標籤 Counter
計數標籤相對於文字標籤來說， 設計上 padding 的設定有依據數字的視覺特性微調過。這是因為計數標籤比較常與其他元件相配和，通常作為計數器，將技術標籤的 padding 做視覺調整會讓整體視覺看起來更平衡。例如在按鈕中。


{{< example >}}

<div class="row text-center" ontouchstart="">
  <div class="col-4 col-xl-2 gy-3">
    <button type="button" class="btn btn-primary"><span>報名活動</span><span class="badge badge-numerical">136</span></button>
  </div>
  <div class="col-4 col-xl-2 gy-3">
    <button type="button" class="btn btn-secondary"><span>下載</span><span class="badge badge-numerical bg-secondary-flat">251</span></button>
  </div>
  <div class="col-4 col-xl-2 gy-3">
    <button type="button" class="btn btn-tertiary"><span>登記</span><span class="badge badge-numerical">20</span></button>
  </div>
  <div class="col-4 col-xl-2 gy-3">
    <button type="button" class="btn btn-emi-secondary"><span>like</span><span class="badge badge-numerical">10</span></button>
  </div>
  <div class="col-4 col-xl-2 gy-3">
    <button type="button" class="btn btn-negative"><span>反對</span><span class="badge badge-numerical bg-negative-flat">3</span></button>
  </div>
  <div class="col-4 col-xl-2 gy-3">
    <button type="button" class="btn btn-positive"><span>贊成</span><span class="badge badge-numerical bg-positive-flat">30</span></button>
  </div>
</div>

{{< /example >}}

### 大小 Size

三種不同大小的標籤。目前本設計系統中都是用中標籤，但依據美感您可以自行搭配使用大或小標籤。在與其他元件配合時，若該元件有分大小 Size，標籤通常會配合其大小。例如在大按鈕中的標籤常用大標籤，中按鈕中的標籤常用中標籤，小按鈕中的標籤常用小標籤。

{{< example >}}

<div class="row text-center">
 <div class="col">
    <span class="badge bg-brand-flat badge-sm">Badge</span>
  </div>
  <div class="col">
    <span class="badge bg-brand-flat">Badge</span>
  </div>
  <div class="col">
    <span class="badge bg-brand-flat badge-lg">Badge</span>
  </div>
</div>
<div class="row text-center">
 <div class="col">
    <button type="button" class="btn btn-primary badge-sm"><span>小按鈕</span><span class="badge badge-numerical">2</span></button>
  </div>
  <div class="col">
    <button type="button" class="btn btn-primary"><span>中按鈕</span><span class="badge badge-numerical">2</span></button>
  </div>
  <div class="col">
    <button type="button" class="btn btn-primary badge-large"><span>大按鈕</span><span class="badge badge-numerical">2</span></button>
  </div>
</div>

{{< /example >}}


### 文字或計數 Text or Counter

標籤內容常有兩種：文字或計數。

{{< example >}}

<div class="row text-center">
  <div class="col">
    <span class="badge bg-brand-flat">Badge</span>
    <span class="badge bg-brand-flat badge-numerical">2</span>
  </div>
</div>

{{< /example >}}

## 範例

### 含有標籤的卡片 Card with badge

標籤可以出現在卡片上，常作為主題分類或屬性文字。

{{< example >}}

<div class="row d-flex justify-content-center">
  <div class="col-md-4">
    <div class="card">
      <img
        src="/docs/5.1/assets/img/bg-card.png"
        class="card-img-top"
        alt="..."
      />
      <div class="card-body">
        <div class="card-title">標題文字</div>
        <div class="badge-group">
          <span class="badge">主題標籤</span
          ><span class="badge">主題標籤</span
          ><span class="badge">主題標籤</span>
        </div>
        <div class="card-text">此部分為卡片之內文部分文字或副標題內容</div>
        <div class="card-actions">
          <button type="button" class="btn btn-primary">預設按鈕</button>
        </div>
      </div>
    </div>
  </div>
</div>

{{< /example >}}

### 含有標籤的列表 List with badge

標籤可以出現在列表上，常作為屬性文字。

{{< example >}}

<div class="row d-flex justify-content-center">
  <div class="col-md-6">
    <div class="list-group-title">最新消息</div>
    <div class="list-group border divider">
      <a href="#" class="list-group-item"><span class="badge">新聞稿</span><div>新聞稿標題範例一（有影音）</div><i class="bi bi-camera-video-fill"></i></a>
      <a href="#" class="list-group-item"><span class="badge">新聞稿</span><div>新聞稿標題範例一（有影音）</div><i class="bi bi-camera-video-fill"></i></a>
      <a href="#" class="list-group-item"><span class="badge">訊息公告</span><div>訊息公告標題範例 （示範標題較長的版本）</div></a>
    </div>
  </div>
</div>

{{< /example >}}
