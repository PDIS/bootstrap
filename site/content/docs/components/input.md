---
layout: docs
title: 輸入欄位 Input
description: 在表單協助使用者輸入格式正確的資訊。
group: components
toc: true
---

## 關於輸入欄位

輸入欄位通常存在於表單中，讓使用者輸入資訊到頁面中。除了表單以外，輸入欄位也可以直接存在於一般頁面上，通常用來搜尋頁面關鍵字。

## 使用規範

### 何時該使用輸入欄位

在輸入資訊到頁面上時，應該使用輸入欄位。通常會與按鈕共存。

### 何時該考慮使用其他元件

當輸入的資訊預計會超過一行，建議使用 textarea。

### 輸入欄位近用性

- **客製化任何表單控制元件時請注意近用性。** 每個表單控制元件都有其近用性規範，請務必遵守。
- **輸入欄位與驗證資訊對齊。** 視覺上對齊驗證資訊與輸入欄位，讓螢幕放大鏡的使用者可以迅速辨別輸入資訊是否正確。

## 元件設計

### 基本輸入欄位 Basic Input

基本款的輸入欄位由標題與輸入欄位組成。

{{< example >}}

<div class="row d-flex justify-content-center">
  <div class="col-lg-4">
      <label for="Input1" class="form-label">標題</label>
    <input type="text" class="form-control" id="Input1" placeholder="Placeholder">
  </div>
</div>

{{< /example >}}

### 大小 Size

三種不同大小的輸入欄位

{{< example >}}

<div class="row d-flex justify-content-center py-3">
  <div class="col-lg-4">
    <label for="Input4" class="form-label form-label-sm">標題</label>
    <input type="text" class="form-control form-control-sm" id="Input4" placeholder="Placeholder">
  </div>
</div>
<div class="row d-flex justify-content-center py-3">
  <div class="col-lg-4">
    <label for="Input2" class="form-label">標題</label>
    <input type="text" class="form-control" id="Input2" placeholder="Placeholder">
  </div>
</div>
<div class="row d-flex justify-content-center py-3">
  <div class="col-lg-4">
    <label for="Input3" class="form-label form-label-lg">標題</label>
    <input type="text" class="form-control form-control-lg" id="Input3" placeholder="Placeholder">
  </div>
</div>

{{< /example >}}

### 提示 Hint

Placeholder 可以作為輸入提示用。也可以在輸入框下顯示提示文字。提示文字可以使用圖示 (icon) 輔助說明

{{< example >}}

<div class="row d-flex justify-content-center py-3">
  <div class="col-lg-4">
    <label for="Input5" class="form-label">密碼</label>
  	<input type="text" class="form-control" id="Input5" placeholder="請輸入密碼">
  </div>
</div>
<div class="row d-flex justify-content-center py-3">
  <div class="col-lg-4">
    <label for="Input6" class="form-label">密碼</label>
    <div class="input-group input-group-icon">
      <i class="input-group-prepend-icon bi bi-key-fill"></i>
      <input type="text" class="form-control" id="Input6" placeholder="請輸入密碼" aria-label="Input6" aria-describedby="Input6">
    </div>
  </div>
</div>
<div class="row d-flex justify-content-center py-3">
  <div class="col-lg-4">
    <label for="Input7" class="form-label">密碼</label>
    <input type="text" class="form-control" id="Input7" placeholder="請輸入密碼">
    <div class="input-hint">提示文字</div>
  </div>
</div>
<div class="row d-flex justify-content-center py-3">
  <div class="col-lg-4">
    <label for="Input8" class="form-label">密碼</label>
    <input type="text" class="form-control" id="Input8" placeholder="請輸入密碼">
    <div class="input-hint"><i class="bi bi-lightbulb icon"></i>提示文字</div>
  </div>
</div>

{{< /example >}}

### 圖示 Icon

輸入框中可以使用圖示 (icon) 輔助說明。圖示可以在文字左邊或是兩邊。左邊圖示提示的作用居多， 與標題文字跟 Placeholder 配合，右邊圖示則比較功能型，必要時才出現。

{{< example >}}

<div class="row d-flex justify-content-center py-3">
  <div class="col-lg-4">
    <label for="Input9" class="form-label">密碼</label>
    <div class="input-group input-group-icon">
      <i class="input-group-prepend-icon bi bi-key-fill"></i>
      <input type="text" class="form-control" id="Input9" placeholder="請輸入密碼" aria-label="Input9" aria-describedby="Input9">
    </div>
  </div>
</div>
<div class="row mt-3 d-flex justify-content-center py-3">
  <div class="col-lg-4">
    <label for="Input10" class="form-label">密碼</label>
    <div class="input-group input-group-icon">
      <i class="input-group-prepend-icon bi bi-key-fill"></i>
      <input type="text" class="form-control" id="Input10" placeholder="請輸入密碼" aria-label="Input10" aria-describedby="Input10">
      <i class="input-group-append-icon bi bi-eye-slash-fill"></i>
    </div>
  </div>
</div>

{{< /example >}}
