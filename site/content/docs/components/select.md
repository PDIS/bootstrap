---
layout: docs
title: 下拉式選單 Select
description: 讓使用者從長清單選項中做一個選擇。
group: components
toc: true
---

### 關於下拉式選單

使用下拉式選單 (Select) 時，我們一律使用原生的選擇功能表 `<select>` 作為設計的起點。我們建議採用的自定義樣式覆蓋下拉式選單按鈕 (Dropdown button) 的風格，讓整體風格更一致。此覆蓋的風格僅限於 `<select>` 的風格，下拉式選單的選單本身 (Dropdown menu) 則無法修改。這是因為瀏覽器的限制無法修改 `<option>` 的風格。

### Guidance

#### When to use the select component

在本設計系統中，當使用者需要做篩選的行為或是在表單中回答問題時，請使用下拉式選單 (Select)。

- **篩選行為。** 使用者在多個選項中做單一選擇，選擇的目的可能是用來排序看到的內容，或過濾、篩選看到的內容。
- **回答問題。** 使用者在多個選項中做出單一或多個選擇，選擇的目的是用來回答問題，系統可以從而儲存使用者所選擇的答案。

#### Usability

- **選項請勿太少。** 選項過少，例如少於三項時，請考慮在頁面上直接用 radio 或 checkbox 展開選項。
- **選項請勿太多。** 選項過多，例如多於十項時，請再度檢視資訊架構，並審查是否有可能將問題拆解。當然，若問題無法輕易拆解時，則可以忽略此提醒。例如當請使用者選擇所縣市時，選項中必定列有全台二十二縣市時，則可以忽略本易用性建議。
- **選項內容相近的放在附近。** 選項內容中，若有內容相近的選項請放在附近，或是使用 `<optgroup>` 分類。
- **提示文字。** 提示文字請使用明確且簡短可供使用者參考的指令，以動詞開頭為佳，例如：「選擇縣市」。請注意，使用提示文字而非預設選項的下拉選單，也代表著使用者被期待做一個選擇。
- **預設選項。** 當網頁內容需要依據下拉式選單的預設選項而連動時，且畫面在沒有預設選項的情況下呈現會有困難時，應給予下拉選單一個預設選項。請注意，有預設選項的下拉式選單也代表使用者沒有必須得做一個選擇的必要。

#### Accessibility

### Component

#### 基本款

基本款包含標題、按鈕與選單。使用預設的選擇功能表 `<select>` 實作。

{{< example >}}

<div class="row d-flex justify-content-center">
  <div class="col-md-4">
    <label for="example1" class="form-label h6">問題/標題</label>
    <select class="select" id="example1" aria-label="example1">
      <option class="option" selected>請選擇一個選項</option>
      <option class="option" value="1">選項一</option>
      <option class="option" value="2">選項二</option>
      <option class="option" value="3">選項三</option>
    </select>
  </div>
</div>

{{< /example >}}

#### 標題位置

標題在上或是標題在左

{{< example >}}

<div class="row d-flex justify-content-center">
  <div class="col-md-4">
    <label for="example2" class="form-label h6">問題/標題</label>
    <select class="select" id="example2" aria-label="example2">
      <option class="option" selected>請選擇一個選項</option>
      <option class="option" value="1">選項一</option>
      <option class="option" value="2">選項二</option>
      <option class="option" value="3">選項三</option>
    </select>
  </div>
</div>

{{< /example >}}
