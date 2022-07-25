---
layout: docs
title: 列表
description: 列表將資訊整理成離散但連續的文字。
group: components
toc: true
---

## 關於列表

列表是連續直排的文字，將資訊組成具邏輯性及架構性離散呈現但風格的一致的模式。列表的內容所呈現的應是一些不同的候選清單（例如：透過關鍵字搜尋後所呈現出的結果）。當使用列表元件時，應輔助使用者迅速定位出候選清單中較為適切的選擇。

## 使用規範

### 何時該使用列表

當您需要呈現一個清單，且裡面含有不同的候選內容時，可以選用有序列表或是無序列表：

- **有序列表 (ordered list)。** 當您需要呈現文字的排名、重要性、層級或步驟時，請使用有序列表。
- **無序列表 (unordered list)。** 當您需要呈現文字並沒有特定的排名或順序時，請使用無序列表。

### 何時該考慮使用其他元件

1. **長篇文字。** 當您需要做較長篇幅的文字溝通時，請考慮用其他元件。
2. **豐富排版。** 當您所需要呈現的資訊可能需要圖片的輔助，或是需要將內容排版時，請考慮用卡片 (card)。

### 列表易用性

1. 若列表內容是完整的文句，請在最後以適當的標點符號結尾，例如：句號（。）、問號（？）。
2. 圓括號有全形（）和半形 ( ) 兩種，括弧內的內容為英文或符號時用半形括弧，括弧前後與中文字之間請加半形空格；括弧內包含純中文或同時包含中文及英文和數字時，請用全形括弧，括弧前後不加空格。
3. 圖標列表中圖標的正面或負面性應於內文相符。
4. 需要用冒號（：）區別標題與內文時，請注意您使用的是全形冒號。

## 元件設計

### 基本款列表 Basic list

基本款列表由數個文字項目構成。

{{< example >}}

<div class="row d-flex justify-content-center">
  <div class="col-6">
    <div class="list-group">
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
    </div>
  </div>
</div>

{{< /example >}}

### 分隔線 Divider

可以選擇使用分隔線區分列表中的每個項目。

{{< example >}}

<div class="row d-flex justify-content-center">
  <div class="col-6">
    <div class="list-group divider">
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
    </div>
  </div>
</div>

{{< /example >}}

### 補充文字位置 Supporting text placement
依據主要文字與補充文字的擺放位置可以分成：

- inline：補充文字與主要文字放在同行。
- block：補充文字在主要文字的下一行。

{{< example >}}

<div class="row d-flex justify-content-center">
  <div class="col-lg-6">
    <div class="list-group">
      <a href="#" class="list-group-item">
        列表主要文字
        <div class="list-group-item-subheader">列表補充文字內容</div>
      </a>
    </div>
  </div>
</div>
<div class="row d-flex justify-content-center py-3">
  <div class="col-lg-6">
    <div class="list-group twoline">
      <a href="#" class="list-group-item">
        <div>
          列表主要文字
          <div class="list-group-item-subheader">列表補充文字內容</div>
        </div>
      </a>
    </div>
  </div>
</div>

{{< /example >}}

### 文字截斷 Text truncation

對於較長的內容，可以透過刪節號截斷文字。

{{< example >}}

<div class="row d-flex justify-content-center py-3">
  <div class="col-lg-6">
    <div class="list-group">
      <a href="#" class="list-group-item d-inline-block text-truncate">列表主要文字列表主要文字列表主要文字列表主要文字</a>
    </div>
  </div>
</div>
<div class="row d-flex justify-content-center py-3">
  <div class="col-lg-6">
    <div class="list-group">
      <a href="#" class="list-group-item"><div class="list-group-item-header">列表主要文字</div><div class="list-group-item-subheader d-inline-block text-truncate">列表補充文字內容列表補充文字內容列表補充文字內容列表補充文字內容列表補充文字內容列表補充文字內容列表補充文字內容</div></a>
    </div>
  </div>
</div>
<div class="row d-flex justify-content-center py-3">
  <div class="col-lg-6">
    <div class="list-group twoline">
        <a href="#" class="list-group-item"><div class="d-grid"><div class="text-truncate">列表主要文字列表主要文字列表主要文字列表主要文字</div><div class="list-group-item-subheader text-truncate">列表補充文字內容列表補充文字內容列表補充文字內容列表補充文字內容列表補充文字內容列表補充文字內容</div></div></a>
    </div>
  </div>
</div>

{{< /example >}}

### 列表帶圖示或標籤 List with icon and badge

文字前可以使用圖示 (icon) 作為開頭。列表前所用的圖示儘量用來幫助使用者了解文字意涵，或用來分類。用圖示分類時，所選用的圖示的正面性或負面性應與文字內容相符。標籤 (badge) 可以用來輔助分類。

{{< example >}}

<div class="row d-flex justify-content-center">
  <div class="col-lg-6">
    <div class="list-group py-3">
      <a href="#" class="list-group-item"><span class="badge">Brand</span><div>列表主要文字</div></a>
    </div>
    <div class="list-group py-3">
      <a href="#" class="list-group-item"><div>列表主要文字</div><span class="badge">Brand</span></a>
    </div>
    <div class="list-group py-3">
      <a href="#" class="list-group-item"><span class="badge">Brand</span><div>列表主要文字</div><i class="bi bi-exclamation-triangle-fill"></i></a>
    </div>
    <div class="list-group py-3">
      <a href="#" class="list-group-item"><i class="bi bi-bell-fill"></i><div>列表主要文字</div><span class="badge">Brand</span></a>
    </div>
  </div>
    <div class="col-lg-6">
    <div class="list-group py-3">
      <a href="#" class="list-group-item"><i class="bi bi-bell-fill"></i><div>列表主要文字</div></a>
    </div>
    <div class="list-group py-3">
      <a href="#" class="list-group-item"><div>列表主要文字</div><i class="bi bi-exclamation-triangle-fill"></i></a>
    </div>
    <div class="list-group py-3">
      <a href="#" class="list-group-item"><i class="bi bi-bell-fill"></i><div>列表主要文字</div><i class="bi bi-exclamation-triangle-fill"></i></a>
    </div>
  </div>
</div>

{{< /example >}}

### 列表帶日期 List with date

當列表帶有日期時，我們示範的設計元件總是將日期放在前面作為開頭。文字後面可以加上圖示、標籤，或是不加任何東西。

{{< example >}}

<div class="row d-flex justify-content-center py-3">
  <div class="col-lg-6">
    <div class="list-group">
      <a href="#" class="list-group-item"><span class="badge badge-date bg-accent-flat">02-22</span><div>列表主要文字</div></a>
    </div>
  </div>
</div>
<div class="row d-flex justify-content-center py-3">
  <div class="col-lg-6">
    <div class="list-group twoline">
      <a href="#" class="list-group-item"><span class="badge badge-date bg-accent-flat">02-22</span><div>列表主要文字<div class="list-group-item-subheader">列表補充文字內容</div></div><span class="badge">Brand</span></a>
    </div>
  </div>
</div>
<div class="row d-flex justify-content-center">
  <div class="col-lg-6">
    <div class="list-group twoline">
      <a href="#" class="list-group-item"><span class="badge badge-date bg-accent-flat">02-22</span><div>列表主要文字<div class="list-group-item-subheader">列表補充文字內容</div></div><i class="bi bi-exclamation-triangle-fill"></i></a>
    </div>
  </div>
</div>

{{< /example >}}

### 框線風格 Border style

- Outlined：用框線將列表與背景區隔開。
- Elevated：將列表視覺上做提升浮起的效果，以與背景區隔。

{{< example >}}

<div class="row gy-5">
  <div class="col-lg-4">
    <div class="list-group divider">
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
    </div>
  </div>
  <div class="col-lg-4">
    <div class="list-group divider border">
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
    </div>
  </div>
  <div class="col-lg-4">
    <div class="list-group divider elevation">
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
    </div>
  </div>
  <div class="col-lg-4">
    <div class="list-group">
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
    </div>
  </div>
  <div class="col-lg-4">
    <div class="list-group border">
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
    </div>
  </div>
  <div class="col-lg-4">
    <div class="list-group border elevation">
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
    </div>
  </div>
</div>

{{< /example >}}

### 標題 Title

用標題概述這是什麼的列表

{{< example >}}

<div class="row gy-5">
  <div class="col-lg-6">
    <div class="list-group-title">標題</div>
    <div class="list-group divider">
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
    </div>
  </div>
  <div class="col-lg-6">
    <div class="list-group-title">標題</div>
    <div class="list-group">
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
      <a href="#" class="list-group-item">列表主要文字</a>
    </div>
  </div>
</div>

{{< /example >}}