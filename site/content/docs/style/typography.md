---
layout: docs
title: 文字屬性 Typography
description: 文字是溝通的基調，它的無所不在也承載了整個產品的基本質感。
group: style
toc: true
---

## 關於文字屬性

文字是最常出現的元素，它的無所不在也代表了整個產品的基本質感。在數位系統中，文字的出現常常代表著頁面上 80% - 90% 的資訊，其他 10% - 20% 可能是視覺引導。雖然文字所承載的的資訊量存在於文字內容而非樣式，但文字的樣式與屬性卻可以大大的影響使用者的閱讀舒適度、閱讀時的情緒。文字屬性乘載著數位產品的溝通基調，而政府網站的文字屬性應該是明確的、理性的、清晰的。

在設計數位系統時，文字內容中的每行字句（例如標題、副標題與內文）的樣式會呈現出所謂的文字情緒、文字聲音與文字氛圍。文字屬性的重要性在於給出一個架構，例如讓同樣層級的文字帶有同樣的樣式，保持整體介面的易讀性。PDIS 設計系統所採用的文字屬性著重於使用者的可讀性與介面整體的易讀性，我們注意一個頁面中標題與內文的可辨認性、段落與段落之間保持可以換氣、呼吸的空間，並注意跨頁面之間標題樣式的一致性、內文樣式的一致性。

## 預設字型家族 Font Family

市面上有許多開源的字體是適合螢幕使用的，本設計系統預設採用的中文字體是 `Noto Sans TC`，英文字體則是 `Noto Sans`。

## 修改字型家族
您可以自由選用適合的字體，方式如下：

我們沿用bootstrap variable的設定

```scss
--bs-body-font-family: var(--bs-font-sans-serif);
```

其中 `--bs-body-font-family` 為 bootstrap 定義的變數，更改此參數即可改變網站的字體設定，而由上述程式碼所知 `--bs-body-font-family` 的值為 `--bs-font-sans-serif`，因此只需在`css`裡覆蓋掉變數 `--bs-font-sans-serif` 即可。

```scss
//範例
--bs-font-sans-serif: "Noto Sans", "Noto Sans TC", sans-serif;
```

需注意的是，我們跟隨國發會的建議，避免使用標楷體，原因如下：

根據國發會網站管理規範指出：政府機關的文件習慣以標楷體編排，但小字型的標楷體在螢幕顯示往往不夠清楚，建議網頁設計者或網頁內容維護者在製作網頁時，取消原訂公文的標楷體格式，檔案或列印版本的公文則另行提供。

### 字級系統 Typescale

這個示範性的字級系統全數使用 Noto Sans TC 字體（英文則使用 Noto Sans)。

{{< bs-table "table" >}}
| Design Token | font-size | font-weight | line-height | example |
|---|---|---|---|---|
| Display/Large | 3.5625rem | 400 | 4rem | <div class="display-text-lg">人皆生而自由；在尊嚴及權利上均各平等。</div> |
| Display/Medium | 2.8125rem | 400 | 3.25rem | <div class="display-text">人皆生而自由；在尊嚴及權利上均各平等。</div> |
| Display/Small | 2.25rem | 400 | 2.75rem | <div class="display-text-sm">人皆生而自由；在尊嚴及權利上均各平等。</div> |
| Heading/Large | 2rem | 400 | 2.5rem | <div class="heading-text-lg">人皆生而自由；在尊嚴及權利上均各平等。</div> |
| Heading/Medium | 1.75rem | 400 | 2.25rem | <div class="heading-text">人皆生而自由；在尊嚴及權利上均各平等。</div> |
| Heading/Small | 1.5rem | 400 | 2rem | <div class="heading-text-sm">人皆生而自由；在尊嚴及權利上均各平等。</div> |
| Title/Large | 1.375rem | 500 | 1.75rem | <div class="title-text-lg">人皆生而自由；在尊嚴及權利上均各平等。</div> |
| Title/Medium | 1.125rem | 500 | 1.5rem | <div class="title-text">人皆生而自由；在尊嚴及權利上均各平等。</div> |
| Title/Small | 1rem | 500 | 1.25rem | <div class="title-text-sm">人皆生而自由；在尊嚴及權利上均各平等。</div> |
| Body/Large | 1.125rem | 400 | 1.6875rem | <div class="body-text-lg">人皆生而自由；在尊嚴及權利上均各平等。</div> |
| Body/Medium | 1rem | 400 | 1.5rem | <div class="body-text">人皆生而自由；在尊嚴及權利上均各平等。</div> |
| Body/Small | 0.75rem | 400 | 100% | <div class="body-text-sm">人皆生而自由；在尊嚴及權利上均各平等。</div> |
| Body/Medium(Links) | 1rem | 500 | 1.5rem | <a href="#">人皆生而自由；在尊嚴及權利上均各平等。</a> |
| Body/Medium(SecondaryLinks) | 1rem | 400 | 1.5rem | <a href="#">人皆生而自由；在尊嚴及權利上均各平等。</div> |
| Label/Large | 1rem | 500 | 1.5rem | <div class="label-text-lg">人皆生而自由；在尊嚴及權利上均各平等。</div> |
| Label/Medium | 0.875rem | 500 | 1.25rem | <div class="label-text">人皆生而自由；在尊嚴及權利上均各平等。</div> |
| Label/Small | 0.75rem | 500 | 1rem | <div class="label-text-sm">人皆生而自由；在尊嚴及權利上均各平等。</div> |
{{< /bs-table >}}