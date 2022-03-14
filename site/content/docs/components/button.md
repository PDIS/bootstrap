---
layout: docs
title: 按鈕 Button
description: 按鈕是個引人注意的可選擇區塊，引導使用者執行重要的行為。
group: components
---

### 關於按鈕元件

按鈕在視覺上是一個頁面上重要行為的引導，在動作是多個頁面間關鍵行為的集合。

### 使用規範

#### 何時該使用按鈕

重要的行為應該用按鈕來顯示，例如「確認」、「下載」、「下一步」、「註冊」、「登出」等。

#### 何時該考慮使用其他元件
- 頁面之間的連結。當純粹想要從一個頁面連結到另外一個頁面時，請用一般的連結即可。
- 當行為的重要性沒那麼高時。當某一行為的重要性在該頁面上沒那麼高時，可以使用文字連結按鈕，視覺上跟連結一樣，但操作上仍為按鈕。

#### 按鈕易用性
- 避免一頁中出現太多按鈕。按鈕的出現應該是該頁面中比較重要的行為，且按下之後會帶領使用者到另一個頁面，因此一頁中的按鈕不宜過多。
- 按鈕文字應以動詞或動作為主。按鈕是引導使用者質性某重要行為的地方，因此請盡量用簡短明瞭的動作文字作為按鈕文字，如「送出」、「取消」等。
- 可以選擇使用圖標。某些按鈕適合用圖標作為提示，例如「開新視窗」、「下載」等，但請適度使用。
- 按鈕文字應保持在同一行。請勿將按鈕文字放到第二行。

#### 按鈕近用性
- 報讀軟體觸發按鈕與連結的方式不同。在使用報讀軟體時，按下空白鍵會觸發按鈕，按下 Enter 鍵會觸發連結。

### 設計元件

#### 方角按鈕 vs 圓角按鈕

可以自行選用符合網站風格的按鈕樣式。

{{< example >}}
<div class="row text-center">
  <div class="col">
    <button type="button" class="btn btn-brand">圓角按鈕</button>
    <button type="button" class="btn rounded-0 btn-brand">方角按鈕</button>
  </div>
</div>
{{< /example >}}

#### 按鈕大小

我們提供大、中、小三種不同尺寸的按鈕。

{{< example >}}
<div class="row text-center">
  <div class="col">
    <button type="button" class="btn btn-brand btn-sm">預設按鈕 小</button>
    <button type="button" class="btn btn-brand">預設按鈕 預設</button>
    <button type="button" class="btn btn-brand btn-lg">預設按鈕 大</button>
  </div>
</div>
{{< /example >}}


#### 功能性按鈕
我們提供兩種功能性按鈕：正向與危險按鈕。

{{< example >}}
<div class="row text-center">
  <div class="col">
    <button type="button" class="btn btn-brand">主色按鈕</button>
    <button type="button" class="btn btn-positive">正面按鈕</button>
    <button type="button" class="btn btn-negative">負面按鈕</button>
  </div>
</div>
{{< /example >}}

#### 淺色功能性按鈕

我們提供兩種功能性按鈕：正向與危險按鈕。

{{< example >}}
<div class="row text-center">
  <div class="col">
    <button type="button" class="btn btn-brand-container">主色按鈕</button>
    <button type="button" class="btn btn-positive-container">正面按鈕</button>
    <button type="button" class="btn btn-negative-container">負面按鈕</button>
  </div>
</div>
{{< /example >}}


#### 框線樣式按鈕  vs 連結字按鈕

同個頁面中，可以選用框線樣式的按鈕，與預設填滿顏色的按鈕作為區隔。當按鈕的行為重要性沒那麼高時，可以將樣式視覺上做得跟連結一樣。

{{< example >}}
<div class="row text-center">
  <div class="col">
    <button type="button" class="btn btn-outline-brand">主色按鈕</button>
    <button type="button" class="btn btn-outline-positive">正面按鈕</button>
    <button type="button" class="btn btn-outline-negative">負面按鈕</button>
    <button type="button" class="btn btn-link">連結字</button>
  </div>
</div>
{{< /example >}}


#### 文字按鈕加圖標

按鈕中放有圖標時，可以選用圖標在左或是圖標在右的按鈕樣式。

{{< example >}}
<div class="row text-center">
  <div class="col">
    <button type="button" class="btn btn-brand">圖標在右<i class="bi bi-arrow-counterclockwise"></i></button>
    <button type="button" class="btn btn-brand"><i class="bi bi-arrow-counterclockwise"></i>圖標在左</button>
  </div>
</div>
{{< /example >}}
