---
layout: docs
title: 按鈕
description: 按鈕是個引人注意的可選擇區塊，引導使用者執行重要的行為。
group: components
---

## 關於按鈕

按鈕在視覺上是一個頁面上重要行為的引導，在動作是多個頁面間關鍵行為的集合。

## 使用規範

### 何時該使用按鈕

重要的行為應該用按鈕來顯示，例如「確認」、「下載」、「下一步」、「註冊」、「登出」等。

### 何時該考慮使用其他元件

- **頁面之間的連結。** 當純粹想要從一個頁面連結到另外一個頁面時，請用一般的連結即可。
- **當行為的重要性沒那麼高時。** 當某一行為的重要性在該頁面上沒那麼高時，可以使用文字連結按鈕，視覺上跟連結一樣，但操作上仍為按鈕。

### 按鈕易用性

- **避免一頁中出現太多按鈕。** 按鈕的出現應該是該頁面中比較重要的行為，且按下之後會帶領使用者到另一個頁面，因此一頁中的按鈕不宜過多。
- **按鈕文字應以動詞或動作為主。** 按鈕是引導使用者質性某重要行為的地方，因此請盡量用簡短明瞭的動作文字作為按鈕文字，如「送出」、「取消」等。
- **可以選擇使用圖標。** 某些按鈕適合用圖標作為提示，例如「開新視窗」、「下載」等，但請適度使用。
- **按鈕文字應保持在同一行。** 請勿將按鈕文字放到第二行。
- 按鈕的位階選擇可以依據主要、次要、邊框、文字的順序做搭配。詳見[角色](/docs/components/button/#角色-role)區塊

### 按鈕近用性

- **報讀軟體觸發按鈕與連結的方式不同。** 在使用報讀軟體時，按下空白鍵會觸發按鈕，按下 Enter 鍵會觸發連結。

## 元件設計

### 基本款按鈕 Basic Button

基本款的按鈕以品牌色為背景，吸引使用者注意。使用者可以依據頁面上的資訊決定是否點擊進行下一步。

{{< example >}}
<div class="row text-center">
  <div class="col">
    <button type="button" class="btn btn-primary">預設按鈕</button>
  </div>
</div>
{{< /example >}}

### 角色 Role

從基本款按鈕的樣式延伸，共六種不同角色的按鈕，由左至右分別為：主要、次要、邊框、文字、正向、負向按鈕。在做按鈕的位階選擇時，可以依據主要、次要、邊框、文字的順序做搭配。例如可以選擇主要按鈕作為預設動作的進入點，搭配文字按鈕作為其他動作的進入點，讓頁面視覺上明顯有位階順序，幫助使用者理解兩個並排按鈕的關係。

{{< example >}}
<!-- <style>
  .btn {
    margin: 0.25rem !important;
  }
</style> -->
<div class="row text-center">
  <div class="col">
    <button type="button" class="btn btn-primary">主要按鈕</button>
    <button type="button" class="btn btn-secondary">次要按鈕</button>
    <button type="button" class="btn btn-tertiary">邊框按鈕</button>
    <button type="button" class="btn btn-semi-secondary">文字按鈕</button>
    <button type="button" class="btn btn-positive">正向按鈕</button>
    <button type="button" class="btn btn-negative">負向按鈕</button>
  </div>
</div>
{{< /example >}}

### 無效 Disabled

有的時候我們會在網頁上看到無效按鈕，它們的存在有其必要性，例如在使用者填寫完註冊表單之前，先加登入按鈕設定為無效按鈕的樣式。無效按鈕用的樣式一律用透明度 60% 處理，呈現如下。

{{< example >}}
<div class="row text-center">
  <div class="col">
    <button type="button" class="btn btn-primary disabled">主要按鈕</button>
    <button type="button" class="btn btn-secondary disabled">次要按鈕</button>
    <button type="button" class="btn btn-tertiary disabled">邊框按鈕</button>
    <button type="button" class="btn btn-semi-secondary disabled">文字按鈕</button>
    <button type="button" class="btn btn-positive disabled">正向按鈕</button>
    <button type="button" class="btn btn-negative disabled">負向按鈕</button>
  </div>
</div>
{{< /example >}}

### 大小 Size
三種不同大小的按鈕，一般預設為中型 Medium 的大小。依據視覺上美感，在與比較大的元件搭配時可以用大的按鈕，與比較小的元件搭配時可以用小的按鈕。例如在本設計系統中，[頁首](/docs/components/header)導覽列手機版的選單按鈕因為與標題搭配，使用大的按鈕。

{{< example >}}

<div class="row text-center">
  <div class="col">
    <button type="button" class="btn btn-primary btn-sm">預設按鈕</button>
    <button type="button" class="btn btn-primary">預設按鈕</button>
    <button type="button" class="btn btn-primary btn-lg">預設按鈕</button>
  </div>
</div>

{{< /example >}}


### 圖示與標籤 Icon and badge

按鈕中可以使用圖示 (icon) 輔助文字說明。圖示可以在文字左邊或是右邊。有些圖示所代表的意義已經約定成俗，在某些特殊情況下則可以只留下圖示。

[標籤](/docs/components/badge)的顏色在設計上會依據按鈕的預設顏色改變，邏輯上皆用按鈕底色的 flat color，唯一例外是，當按鈕底色已經是 flat ，則用 surface color。關於顏色系統的詳細規則請見顏色。

若您需要改變標籤的[顏色](docs/style/color)，則需要自行覆寫 (overwrite)。

{{< example >}}

<div class="row text-center">
  <div class="col">
    <button type="button" class="btn btn-primary">預設按鈕</button>
    <button type="button" class="btn btn-primary"><i class="bi bi-download"></i><span>左圖標按鈕</span></button>
    <button type="button" class="btn btn-primary"><span>右圖標按鈕</span><i class="bi bi-download"></i></button>
    <button type="button" class="btn btn-primary"><i class="bi bi-download"></i></button>
    <button type="button" class="btn btn-primary"><span>預設按鈕</span><span class="badge badge-numerical">2</span></button>
  </div>
</div>

{{< /example >}}
