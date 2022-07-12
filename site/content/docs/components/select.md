---
layout: docs
title: 選擇功能表
description: 讓使用者從清單選項中做一個選擇。
group: components
toc: true
---

## 關於選擇功能表

使用選擇功能表 (Select) 時，我們一律使用原生的選擇功能表 `<select>` 作為設計的起點。我們建議採用的自定義樣式覆蓋選擇功能表的起始外觀。此覆蓋的風格僅限於 `<select>` 的風格， `<option>` 則因為瀏覽器的限制無法修改。

## 使用規範

### 何時該使用選擇功能表

在本設計系統中，當使用者需要做篩選的行為或是在表單中回答問題時，請使用選擇功能表 (Select)。

- **篩選行為。** 使用者在多個選項中做單一選擇，選擇的目的可能是用來排序看到的內容，或過濾、篩選看到的內容。
- **回答問題。** 使用者在多個選項中做出單一或多個選擇，選擇的目的是用來回答問題，系統可以從而儲存使用者所選擇的答案。

### 何時該考慮使用其他元件

- **頁面導覽。** 當選擇的目的為頁面導覽時，請參考導覽的下拉式導覽選單 (Navigation Dropdowns)。
- **選單中選擇並不多。** 當下拉式選單中所陳列的選擇項目並不多，並且頁面空間足夠陳列所有選擇時，建議可以改以較容易看到所有選項的 `radio` 或 `checkbox` 陳列現有選項，讓使用者做選擇。

### 選擇功能表易用性

- **選項請勿太少。** 選項過少，例如少於三項時，請考慮在頁面上直接用 `radio` 或 `checkbox` 展開選項。
- **選項請勿太多。** 選項過多，例如多於十項時，請再度檢視資訊架構，並審查是否有可能將問題拆解。當然，若問題無法輕易拆解時，則可以忽略此提醒。例如當請使用者選擇所縣市時，選項中必定列有全台二十二縣市時，則可以忽略本易用性建議。
- **選項內容相近的放在附近。** 選項內容中，若有內容相近的選項請放在附近，或是使用 `<optgroup>` 分類。
- **提示文字。** 提示文字請使用明確且簡短可供使用者參考的指令，以動詞開頭為佳，例如：「選擇縣市」。請注意，使用提示文字而非預設選項的下拉選單，也代表著使用者被期待做一個選擇。
- **預設選項。** 當網頁內容需要依據下拉式選單的預設選項而連動時，且畫面在沒有預設選項的情況下呈現會有困難時，應給予下拉選單一個預設選項。請注意，有預設選項的下拉式選單也代表使用者沒有必須得做一個選擇的必要。

### 選擇功能表近用性

- **標題必帶。** 為搭配報讀軟題，請務必在下拉式選單前加上標題，供報讀軟題讀取選單的標題。

## 元件設計

### 基本下拉選單 Basic Select

基本款包含標題、按鈕與選單。使用預設的選擇功能表 `<select>` 實作。整個寬度跟著父層容器的寬度變化。

{{< example >}}
<div class="row d-flex justify-content-center">
  <div class="col-lg-4">
    <label for="example1" class="form-label">標題</label>
    <select class="form-select" id="example1" aria-label="example1">
      <option selected>請選擇一個選項</option>
      <option value="1">選項一</option>
      <option value="2">選項二</option>
      <option value="3">選項三</option>
    </select>
  </div>
</div>
{{< /example >}}

### 大小 Size

三種不同大小。

{{< example >}}
<div class="row d-flex justify-content-center">
  <div class="col-lg-4 py-3">
    <select class="form-select form-select-sm" id="example4" aria-label="example4">
      <option selected>請選擇一個選項</option>
      <option value="1">選項一</option>
      <option value="2">選項二</option>
      <option value="3">選項三</option>
    </select>
  </div>
    <div class="col-lg-4 py-3">
    <select class="form-select" id="example2" aria-label="example2">
      <option selected>請選擇一個選項</option>
      <option value="1">選項一</option>
      <option value="2">選項二</option>
      <option value="3">選項三</option>
    </select>
  </div>
    <div class="col-lg-4 py-3">
    <select class="form-select form-select-lg" id="example3" aria-label="example3">
      <option selected>請選擇一個選項</option>
      <option value="1">選項一</option>
      <option value="2">選項二</option>
      <option value="3">選項三</option>
    </select>
  </div>
</div>
{{< /example >}}

### 標題位置

標題在上或是標題在左。

{{< example >}}
<div class="row d-flex justify-content-center py-3">
  <div class="col-lg-6">
    <label for="example5" class="form-label">標題</label>
    <select class="form-select" id="example5" aria-label="example5">
      <option selected>請選擇一個選項</option>
      <option value="1">選項一</option>
      <option value="2">選項二</option>
      <option value="3">選項三</option>
    </select>
  </div>
</div>
<div class="row d-flex justify-content-center py-3">
  <div class="col-lg-6">
    <div class="row">
      <div class="col-3">
        <label for="example6" class="form-label align-self-center">標題</label>
      </div>
      <div class="col-9">
        <select class="form-select" id="example6" aria-label="example6">
          <option selected>請選擇一個選項</option>
          <option value="1">選項一</option>
          <option value="2">選項二</option>
          <option value="3">選項三</option>
        </select>
      </div>
    </div>
  </div>
</div>
{{< /example >}}

### 選項組 Optgroup

當選項內容有層級分類時，可以使用選項組。

{{< example >}}
<div class="row d-flex justify-content-center">
  <div class="col-lg-4">
    <label for="example7" class="form-label">標題</label>
    <select class="form-select" id="example7" aria-label="example7">
      <option  selected>請選擇一個選項</option>
      <optgroup label="分類一">
        <option value="1">選項一</option>
        <option value="2">選項二</option>
        <option value="3">選項三</option>
        <option value="4">選項四</option>
      </optgroup>
      <optgroup  label="分類二">
        <option value="5">選項一</option>
        <option value="6">選項二</option>
        <option value="7">選項三</option>
        <option value="8">選項四</option>
      </optgroup>
    </select>
  </div>
</div>
{{< /example >}}

### 下拉選單組 Select group

有序且多個下拉選單的組合，通常會需要先針對一個下拉選單做選擇，且其選擇值會影響到下一個下拉選單的內容。

{{< example >}}
<div class="row d-flex justify-content-center py-3">
  <div class="col-lg-4 py-3">
    <label for="example8" class="form-label">標題</label>
    <select class="form-select" id="example8" aria-label="example8" onchange="ShowSelect2()">
      <option  value="0" selected>請選擇一個選項</option>
      <option  value="1">選項一</option>
      <option  value="2">選項二</option>
      <option  value="3">選項三</option>
    </select>
  </div>
  <div class="col-lg-4 py-3">
    <label for="example9" class="form-label">標題</label>
    <select class="form-select" id="example9" aria-label="example9" disabled onchange="ShowSelect3()">
      <option  value="0" selected>請選擇一個選項</option>
      <option  value="1">選項一</option>
      <option  value="2">選項二</option>
      <option  value="3">選項三</option>
    </select>
  </div>
  <div class="col-lg-4 py-3">
    <label for="example10" class="form-label">標題</label>
    <select class="form-select" id="example10" aria-label="example10" disabled>
      <option  value="0" selected>請選擇一個選項</option>
      <option  value="1">選項一</option>
      <option  value="2">選項二</option>
      <option  value="3">選項三</option>
    </select>
  </div>
</div>

<script>
  const ShowSelect2 = () => {
    document.getElementById("example8").value !== '0' ? document.getElementById("example9").disabled = false : document.getElementById("example9").disabled = true; document.getElementById("example9").value = '0'; document.getElementById("example10").disabled = true; document.getElementById("example10").value = '0'
  }

  const ShowSelect3 = () => {
    document.getElementById("example9").value !== '0' ? document.getElementById("example10").disabled = false : document.getElementById("example10").disabled = true; document.getElementById("example10").value = '0'
  }
</script>
{{< /example >}}

### 下拉選單搭配輸入框 Select controlled input field

下拉選單與輸入框的組合，通常會需要先針對下拉選單做選擇，且其選擇值會影響到與其搭配的輸入框可輸入的內容。

{{< example >}}
<div class="row d-flex justify-content-center">
  <div class="col-lg-6">
    <label for="example11" class="form-label">標題</label>
    <div class="input-group">
      <select class="form-select" id="example11" aria-label="example11">
        <option selected>請選擇一個選項</option>
        <option value="1">選項一</option>
        <option value="2">選項二</option>
        <option value="3">選項三</option>
      </select>
      <input type="text" class="form-control" placeholder="placeholder" aria-label="example11">
    </div>
  </div>
</div>
{{< /example >}}