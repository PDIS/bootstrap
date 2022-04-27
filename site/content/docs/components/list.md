---
layout: docs
title: 列表 (List)
description: 列表將資訊整理成離散但連續的文字。
group: components
toc: true
---

### 關於列表元件

列表是連續直排的文字，將資訊組成具邏輯性及架構性離散呈現但風格的一致的模式。列表的內容所呈現的應是一些不同的候選清單（例如：透過關鍵字搜尋後所呈現出的結果）。當使用列表元件時，應輔助使用者單用視覺快速瀏覽網頁時，便迅速定位出候選清單中較為適切的選擇。

### 使用規範

#### 何時該使用列表

當您需要呈現一個清單，且裡面含有不同的候選內容時，可以選用有序列表或是無序列表：

- **有序列表 (ordered list)。** 當您需要呈現文字的排名、重要性、層級或步驟時，請使用有序列表。
- **無序列表 (unordered list)。** 當您需要呈現文字並沒有特定的排名或順序時，請使用無序列表。

#### 何時該考慮使用其他元件

1. **長篇文字。** 當您需要做較長篇幅的文字溝通時，請考慮用其他元件。
2. **豐富排版。** 當您所需要呈現的資訊可能需要圖片的輔助，或是需要將內容排版時，請考慮用卡片 (card)。

#### 列表易用性

1. 若列表內容是完整的文句，請在最後以適當的標點符號結尾，例如：句號（。）、問號（？）。
2. 圓括號有全形（）和半形 ( ) 兩種，括弧內的內容為英文或符號時用半形括弧，括弧前後與中文字之間請加半形空格；括弧內包含純中文或同時包含中文及英文和數字時，請用全形括弧，括弧前後不加空格。
3. 圖標列表中圖標的正面或負面性應於內文相符。
4. 需要用冒號（：）區別標題與內文時，請注意您使用的是全形冒號。

### 設計元件

#### 基本款列表 Basic list

基本款列表包含標題與內文。您可以選擇隱藏內文成為更單純的項目列表。

{{< example >}}

<div class="row">
  <div class="col-6">
    <label class="list-title">標題</label>
    <ul class="list-group twoline">
      <li class="list-group-item"><i class="bi bi-arrow-counterclockwise"></i><div>列表主要文字<div class="list-group-item-subheader">列表補充文字內容</div></div><i class="bi bi-arrow-counterclockwise"></i></li>
      <li class="list-group-item"><div class="d-grid"><div class="text-truncate">列表主要文字列表主要文字列表主要文字列表主要文字</div><div class="list-group-item-subheader text-truncate">列表補充文字內容列表補充文字內容列表補充文字內容列表補充文字內容列表補充文字內容列表補充文字內容</div></div></li>
      <li class="list-group-item"><span class="badge">badge</span><div>列表主要文字<div class="list-group-item-subheader">列表補充文字內容</div></div></li>
      <li class="list-group-item"><span class="badge badge-date bg-accent-flat">04-22</span><div>列表主要文字</div><div>列表主要文字</div><i class="bi bi-exclamation-triangle-fill"></i></li>
    </ul>
  </div>
</div>
<br/>
<div class="row">
  <div class="col">
   <ul class="list-group twoline">
      	<li class="list-group-item">列表主要文字<div class="list-group-item-subheader">列表補充文字內容</div></li>
      </ul>
    <ul class="list-group">
          	<li class="list-group-item"><div class="list-group-item-header">列表主要文字</div><div class="list-group-item-subheader d-inline-block text-truncate">列表補充文字內容列表補充文字內容列表補充文字內容列表補充文字內容列表補充文字內容列表補充文字內容列表補充文字內容</div></li>
      <li class="list-group-item">標題</li>
      <li class="list-group-item">標題</li>
    </ul>
  </div>
</div>
<div class="row">
  <div class="col">
    <ul class="list-group border divider">
      <a href="#" class="list-group-item"><span>標題</span><i class="bi bi-arrow-counterclockwise"></i></a>
      <a href="#" class="list-group-item"><i class="bi bi-arrow-counterclockwise"></i><span>標題</span></a>
      <li class="list-group-item"><span class="badge">badge</span><span>標題</span></li>
    </ul>
  </div>
</div>

{{< /example >}}

#### 框線 Border

可以選擇使用框線。

{{< example >}}

<div class="row">
  <div class="col">
    <ul class="list-group">
      <li class="list-group-item">標題<p class="list-group-item-subheader">副標題或內文簡單闡述</p></li>
      <li class="list-group-item">標題<p class="list-group-item-subheader">副標題或內文簡單闡述</p></li>
      <li class="list-group-item">標題<p class="list-group-item-subheader">副標題或內文簡單闡述</p></li>
    </ul>
  </div>
</div>
<br/>
<div class="row">
  <div class="col-8 col-lg-6">
    <ul class="list-group">
      <li class="list-group-item list-group-item-bottom-border">標題<p class="list-group-item-subheader">副標題或內文簡單闡述</p></li>
      <li class="list-group-item list-group-item-bottom-border">標題<p class="list-group-item-subheader">副標題或內文簡單闡述</p></li>
      <li class="list-group-item list-group-item-bottom-border">標題<p class="list-group-item-subheader">副標題或內文簡單闡述</p></li>
    </ul>
  </div>
</div>

{{< /example >}}

#### 連結 Links

當使用者可以點選列表中的文字到另一頁面時，請使用連結風格 (link style)。

{{< example >}}

<div class="row">
  <div class="col-lg-6">
    <ul class="list-group">
      <li class="list-group-item">標題<p class="list-group-item-subheader">副標題或內文簡單闡述</p></li>
    </ul>
  </div>
    <div class="col-lg-6">
    <ul class="list-group">
      <li class="list-group-item">標題<a href="#" class="list-group-item-link">副標題或內文簡單闡述</a></li>
    </ul>
  </div>
</div>
<br/>
<div class="row">
  <div class="col-lg-6">
    <ul class="list-group">
      <li class="list-group-item list-group-item-ordered">標題<p class="list-group-item-subheader">副標題或內文簡單闡述</p></li>
    </ul>
  </div>
  <div class="col-lg-6">
    <ul class="list-group">
      <li class="list-group-item list-group-item-ordered">標題<a href="#" class="list-group-item-link">副標題或內文簡單闡述</a></li>
    </ul>
  </div>
</div>
<br/>
<div class="row">
  <div class="col-lg-6">
    <ul class="list-group">
      <li class="list-group-item list-group-item-twoline">標題<p class="list-group-item-subheader">副標題或內文簡單闡述</p></li>
    </ul>
  </div>
  <div class="col-lg-6">
    <ul class="list-group">
      <li class="list-group-item list-group-item-twoline">標題<a href="#" class="list-group-item-link">副標題或內文簡單闡述</a></li>
    </ul>
  </div>
</div>

{{< /example >}}

#### 文字對齊 Text Alignment

標題與內文可以同行，也可以將內文放在標題下一行。

{{< example >}}

<div class="row">
  <div class="col">
    <ul class="list-group">
      <li class="list-group-item">標題<p class="list-group-item-subheader">副標題或內文簡單闡述</p></li>
    </ul>
  </div>
</div>
<br/>
<div class="row">
  <div class="col">
    <ul class="list-group">
      <li class="list-group-item list-group-item-twoline">標題<p class="list-group-item-subheader">副標題或內文簡單闡述</p></li>
    </ul>
  </div>
</div>

{{< /example >}}

#### 項目符號 Bullet

在標題前面，您也可以選擇加上項目符號。

{{< example >}}

<div class="row">
  <div class="col">
    <ul class="list-group">
      <li class="list-group-item">標題<p class="list-group-item-subheader">副標題或內文簡單闡述</p></li>
    </ul>
  </div>
</div>
<br/>
<div class="row">
  <div class="col">
    <ul class="list-group">
      <li class="list-group-item list-group-item-ordered">標題<p class="list-group-item-subheader">副標題或內文簡單闡述</p></li>
    </ul>
  </div>
</div>

{{< /example >}}

#### 內文長度 Content length

內文比較長時，請在句尾用省略號 （…），並將所顯示的文字放在一行內顯示，請勿顯示超過一行。

{{< example >}}

<div class="row">
  <div class="col">
    <ul class="list-group">
      <li class="list-group-item list-group-item-twoline">課程代碼<p class="list-group-item-subheader">PCENTER110100901</p></li>
    </ul>
  </div>
</div>
<br/>
<div class="row">
  <div class="col">
    <ul class="list-group">
      <li class="list-group-item list-group-item-twoline text-truncate">歡迎來部落走走 交通部觀光局邀您來當「部落客」！
        <p class="list-group-item-subheader text-truncate">交通部觀光局(以下稱觀光局)為宣傳部落特色及觀光成果，自103年起已連續8年舉辦「台灣部落觀光嘉年華」</p>
      </li>
    </ul>
  </div>
</div>

{{< /example >}}

#### 圖標列表 Icon list

項目文字前可以使用圖標 (icon) 作為開頭。列表前所用的圖標儘量用來幫助使用者分類用，並且所選用的圖標的正面性或負面性應與文字內容相符。另外，圖標列表也運用在統計圖表中的圖例 (legend) 使用。請注意，為了幫助使用者辨別列表與手風琴元件，我們強烈建議在選用圖標時，請避免使用上下方向箭頭或是正負加減符號。

{{< example >}}

<div class="row">
  <div class="col">
    <ul class="list-group">
      <li class="list-group-item"><i class="bi bi-check-circle-fill text-success icon"></i>請攜帶健保卡</li>
      <li class="list-group-item"><i class="bi bi-check-circle-fill text-success icon"></i>請配戴口罩</li>
      <li class="list-group-item"><i class="bi bi-check-circle-fill text-success icon"></i>請與工作人員保持兩公尺距離</li>
      <li class="list-group-item"><i class="bi bi-check-circle-fill text-danger icon"></i>請勿飲食</li>
    </ul>
  </div>
</div>
<br />
<div class="row">
  <div class="col">
    <ul class="list-group">
      <li class="list-group-item"><i class="bi bi-download"></i><a href="#">下載說明文件</a></li>
      <li class="list-group-item"><i class="bi bi-download"></i><a href="#">下載議程時間表</a></li>
      <li class="list-group-item"><i class="bi bi-download"></i><a href="#">下載圖檔</a></li>
      <li class="list-group-item"><i class="bi bi-download"></i><a href="#">下載報名表格</a></li>
    </ul>
  </div>
</div>
<br />
<div class="row">
  <div class="col-lg-8">
    <ul class="list d-flex justify-content-between">
      <li class="list-group-item"><i class="bi bi-square-fill text-brand"></i>15-18歲</li>
      <li class="list-group-item"><i class="bi bi-square-fill text-positive"></i>19-30歲</li>
      <li class="list-group-item"><i class="bi bi-square-fill text-negative"></i>31 歲（含）以上</li>
    </ul>
  </div>
</div>

{{< /example >}}

#### 有序列表與無序列表 Ordered list and Unordered list

當您需要呈現文字的排名、重要性、層級或步驟時，請使用有序列表。當您需要呈現文字並沒有特定的排名或順序時，請使用無序列表。

{{< example >}}

<div class="row">
  <div class="col">
    <ol class="list-group">
      <li class="list-group-item list-group-item-ordered">標題</li>
      <li class="list-group-item list-group-item-ordered">標題</li>
      <li class="list-group-item list-group-item-ordered">標題</li>
    </ol>
  </div>
</div>
<br/>
<div class="row">
  <div class="col">
    <ul class="list-group">
      <li class="list-group-item list-group-item-ordered">標題</li>
      <li class="list-group-item list-group-item-ordered">標題</li>
      <li class="list-group-item list-group-item-ordered">標題</li>
    </ul>
  </div>
</div>

{{< /example >}}

#### 有序列表 Ordered list

有序列表的預設排序方式

{{< example >}}

<div class="row">
  <div class="col-lg-4">
    <ol class="list trad-chinese-informal">
      <li class="list-group-item list-group-item-ordered">標題</li>
      <li class="list-group-item list-group-item-ordered">標題</li>
      <li class="list-group-item list-group-item-ordered">標題</li>
    </ol>
  </div>
  <div class="col-lg-4">
    <ol class="list-group" type="A">
      <li class="list-group-item list-group-item-ordered">標題</li>
      <li class="list-group-item list-group-item-ordered">標題</li>
      <li class="list-group-item list-group-item-ordered">標題</li>
    </ol>
  </div>
  <div class="col-lg-4">
    <ol class="list-group">
      <li class="list-group-item list-group-item-ordered">標題</li>
      <li class="list-group-item list-group-item-ordered">標題</li>
      <li class="list-group-item list-group-item-ordered">標題</li>
    </ol>
  </div>
</div>
<br/>
<div class="row">
  <div class="col-lg-4">
    <ol class="list trad-chinese-informal">
      <li class="list-group-item list-group-item-twoline-ordered">標題<p class="list-group-item-subheader">副標題或內文簡單闡述</p></li>
    </ol>
  </div>
  <div class="col-lg-4">
    <ol class="list-group" type="A">
      <li class="list-group-item list-group-item-twoline-ordered">標題<p class="list-group-item-subheader">副標題或內文簡單闡述</p></li>
    </ol>
  </div>
  <div class="col-lg-4">
    <ol class="list-group">
      <li class="list-group-item list-group-item-twoline-ordered">標題<p class="list-group-item-subheader">副標題或內文簡單闡述</p></li>
    </ol>
  </div>
</div>
<br/>
<div class="row">
  <div class="col-lg-4">
    <ol class="list trad-chinese-formal">
      <li class="list-group-item list-group-item-ordered">標題</li>
      <ol class="trad-chinese-informal">
        <li class="list-group-item list-group-item-ordered">標題</li>
      </ol>
    </ol>
  </div>
  <div class="col-lg-4">
    <ol class="list-group" type="A">
      <li class="list-group-item list-group-item-ordered">標題</li>
      <ol type="a" class="nested-list">
        <li class="list-group-item list-group-item-ordered">標題</li>
      </ol>
    </ol>
  </div>
  <div class="col-lg-4">
    <ol class="list-group">
      <li class="list-group-item list-group-item-ordered">標題</li>
      <ol class="nested-list">
        <li class="list-group-item list-group-item-ordered">標題</li>
      </ol>
    </ol>
  </div>
</div>

{{< /example >}}

#### 單行、雙行、多行時序列表 single-line, double-line and multi-line time ordered list

雙行的情況下，時間與標題同行。多行的情況下，時間在標題上方一行。

{{< example >}}

<div class="row">
  <div class="col">
    <ul class="list time-list">
      <li class="list-group-item">
        <div class="list-group-item-date">2021-10-25</div>
        <div class="list-group-item-content text-truncate">
          歡迎來部落走走 交通部觀光局邀您來當「部落客」！
        </div>
      </li>
    </ul>
  </div>
</div>
<br/>
<div class="row">
  <div class="col">
    <ul class="list time-list">
      <li class="list-group-item">
        <div class="list-group-item-date">2021-10-25</div>
        <div class="list-group-item-content text-truncate">
          歡迎來部落走走 交通部觀光局邀您來當「部落客」！
          <p class="list-group-item-subheader text-truncate">交通部觀光局(以下稱觀光局)為宣傳部落特色及觀光成果，自103年起已連續8年舉辦「台灣部落觀光嘉年華」</p>
        </div>
      </li>
    </ul>
  </div>
</div>
<br/>
<div class="row">
  <div class="col">
    <ul class="list time-list">
      <li class="list-group-item-multiline">
        <div class="list-group-item-date">2021-10-25</div>
        <div class="list-group-item-content text-truncate">
          歡迎來部落走走 交通部觀光局邀您來當「部落客」！
          <p class="list-group-item-subheader text-truncate">交通部觀光局(以下稱觀光局)為宣傳部落特色及觀光成果，自103年起已連續8年舉辦「台灣部落觀光嘉年華」</p>
        </div>
      </li>
    </ul>
  </div>
</div>

{{< /example >}}

#### 時序列表加分類標籤 Time ordered list with categorisation tags

時序列表加上分類標籤時，依據行數適合將標籤放在不同位置。

{{< example >}}

<div class="row">
  <div class="col">
    <ul class="list time-list">
      <li class="list-group-item">
        <div class="list-group-item-date">2021-10-25</div>
        <span class="badge bg-brand">Primary</span>
        <div class="list-group-item-content text-truncate">
          歡迎來部落走走 交通部觀光局邀您來當「部落客」！
        </div>
      </li>
    </ul>
  </div>
</div>
<br/>
<div class="row">
  <div class="col">
    <ul class="list time-list">
      <li class="list-group-item d-flex justify-content-between">
        <div class="list-group-item-date">2021-10-25</div>
        <div class="list-group-item-content text-truncate">
          歡迎來部落走走 交通部觀光局邀您來當「部落客」！
        </div>
        <span class="badge bg-brand">Primary</span>
      </li>
    </ul>
  </div>
</div>
<br/>
<div class="row">
  <div class="col">
    <ul class="list time-list">
      <li class="list-group-item-multiline">
        <div class="list-group-item-date d-inline">2021-10-25</div>
        <span class="badge bg-brand">Primary</span>
        <div class="list-group-item-content text-truncate">
          歡迎來部落走走 交通部觀光局邀您來當「部落客」！
          <p class="list-group-item-subheader">交通部觀光局(以下稱觀光局)為宣傳部落特色及觀光成果，自103年起已連續8年舉辦「台灣部落觀光嘉年華」</p>
        </div>
      </li>
    </ul>
  </div>
</div>

{{< /example >}}

#### 單行時序列表 (time ordered list) vs 列表加時間戳記 (ordered list with timestamp)

有些情況下，列表的排序方式是以時間為主的；也有些情況下，時間戳記僅作為輔助資訊。

{{< example >}}

<div class="row">
  <div class="col">
    <ul class="list time-list">
      <li class="list-group-item">
        <div class="list-group-item-date">2021-10-25</div>
        <div class="list-group-item-content text-truncate">
          歡迎來部落走走 交通部觀光局邀您來當「部落客」！
        </div>
      </li>
    </ul>
  </div>
</div>
<br/>
<div class="row">
  <div class="col">
    <ul class="list time-list">
      <li class="list-group-item d-flex justify-content-between">
        <div class="list-group-item-content text-truncate">
          歡迎來部落走走 交通部觀光局邀您來當「部落客」！
        </div>
        <div class="list-group-item-date">2021-10-25</div>
      </li>
    </ul>
  </div>
</div>

{{< /example >}}

#### 單行、多行列表加時間戳記 Single-line and multi-line ordered list with timestamp

當時間雖用於排序，但不作為使用者解讀資訊的主要依據時，時間戳記的位置依據單行或多行有所不同。單行時時間戳記放在內文後面，多行時時間戳記放在內文下面。

{{< example >}}

<div class="row">
  <div class="col">
    <ul class="list time-list">
      <li class="list-group-item d-flex justify-content-between">
        <div class="list-group-item-content text-truncate">
          歡迎來部落走走 交通部觀光局邀您來當「部落客」！
        </div>
        <div class="list-group-item-date">2021-10-25</div>
      </li>
    </ul>
  </div>
</div>
<br/>
<div class="row">
  <div class="col">
    <ul class="list time-list">
      <li class="list-group-item-multiline">
        <div class="list-group-item-content text-truncate">
          歡迎來部落走走 交通部觀光局邀您來當「部落客」！
          <p class="list-group-item-subheader text-truncate">交通部觀光局(以下稱觀光局)為宣傳部落特色及觀光成果，自103年起已連續8年舉辦「台灣部落觀光嘉年華」</p>
          2021-10-25
        </div>
      </li>
    </ul>
  </div>
</div>

{{< /example >}}
