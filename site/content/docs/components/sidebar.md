---
layout: docs
title: 側邊欄
description: 放置頁面一邊的具層級性、垂直排列的導覽。
group: components
toc: true
---

## 關於側邊欄元件

側邊欄為導覽用的元件，通常與頂部導覽搭配使用，適合當網站資訊架構較為複雜、層級較多時使用。側邊欄可以呈現一到三層級的選項，第一層級的選項最少五項。根據米勒定律 (Miller’s law) 一般人短期記憶中能容納的物體數量為七加減二，所以第一層級的選項也請儘量維持在九項以下。第二層級沒有特別規定，但若超過九項時，請審慎考慮網站的架構規劃。第三層級因為已到達直接呈現後點擊的用途，連結數量上並沒有一定限制。

## 使用規範

### 何時該使用側邊欄

- **呈現一到三層級的導覽架構。** 側邊欄至少一層且第一層級至少五項，層級數目則至多三層。
- **呈現網站分區中的次層級導覽。** 當網站有明顯分區且次層級較多時，善用側邊欄輔助頂部導覽列。
- **有層級的常用服務之快速導覽。** 當網站有明顯較常用的服務存在且多於五項又有層級架構時，利用側邊欄作為整個網站的快速導覽。

### 何時該考慮使用其他元件

- **小網站。** 當網站架構簡單、層級數少時，不需用到側邊欄。
- **已有導覽存在。** 當網站架構簡單，頂部導覽即可有效的引導使用者時，不需用到側邊欄。
- **需要用文字標題以外的元素描述時。** 當文字標題不足以描述使用者即將前往的頁面時，請考慮用其他元件，例如卡片。
- **數量少的常用服務之快速導覽。** 當有替常用服務做快速導覽的需求時，若層級簡單則不需用到側邊欄，可以考慮使用其他元件如卡片，橫向呈列常見服務。
- **選項為僅供瀏覽但不可以點擊的資訊。** 當列出的選項僅為瀏覽用但不為導覽用時，請勿使用導覽列。

### 側邊欄易用性

- **文字標題簡短。** 請保持文字標題簡短易懂，且在單行呈現文字標題。
- **用狀態呈現目前選擇。** 利用風格區別已選擇或未選擇的選項，通常使用狀態 (actvie state) 來區別。
- **側邊欄內比較不常用的選擇放在比較下方。** 使用者的注意力會從側邊欄的選項中從上至下瀏覽，因此為了幫助使用者方便且迅速的到達對的頁面，請將比較不常見的選擇放在欄位較為下方的位置。
- **請勿用過於華麗的特效展開、收納導覽列。** 導覽的用除在於幫助使用者找到對的頁面與內容，請勿將導覽列的風格或視覺做得過於花俏反而喧賓奪主，影響使用者的注意力。
- **請勿在側邊欄呈現跟其他導覽列完全一樣的內容。** 當側邊欄與頂部導覽列同時存在時，側邊欄的存在目的為輔助頂部導覽列，完全將頂部導覽列的內容全部複製到側邊欄。
- **請勿為了填滿空間而使用側邊欄。** 側邊欄的存在目的為導覽，當頁面很簡單乾淨時，切勿為了填滿空間而執意製作一個側邊導覽列。空白空間的存在可以幫助使用者將注意力放在對的地方。
- **請勿只以圖標 (icon) 呈現側邊欄。** 側邊欄的存在目的為導覽，且應能幫助使用者迅速地看到欲點擊選項。勿為省略文字標題，而只以圖標暗示。請勿讓使用者花額外時間猜測圖標背後代表的意義。

## 元件設計

### 基本側邊欄 Basic Sidebar

基本側邊欄由垂直排列的選單所構成，至多可以展開到第三層。

{{< example >}}
<div class="row d-flex justify-content-center">
  <div class="col-lg-6">
    <nav class="sidebar">
      <ul class="sidebar-body">
        <li>
          <button class="sidebar-button collapsed" data-bs-toggle="collapse" data-bs-target="#first-collapse" aria-expanded="true">
            可展開第一層標題
          </button>
          <div class="collapse" id="first-collapse">
            <ul class="sidebar-menu">
              <li>
                <button class="sidebar-button collapsed" data-bs-toggle="collapse" data-bs-target="#second-collapse" aria-expanded="true">可展開第二層標題
                </button>
                <div class="collapse" id="second-collapse">
                  <ul class="sidebar-menu">
                    <li><a href="#" class="sidebar-link">第三層連結內容</a></li>
                    <li><a href="#" class="sidebar-link">第三層連結內容</a></li>
                    <li><a href="#" class="sidebar-link">第三層連結內容</a></li>
                  </ul>
                </div>
              </li>
            </ul>
          </div>
        </li>
        <li>
          <button class="sidebar-button collapsed" data-bs-toggle="collapse" data-bs-target="#one-collapse" aria-expanded="true">
            可展開第一層標題
          </button>
          <div class="collapse" id="one-collapse">
            <ul class="sidebar-menu">
              <li>
                <button class="sidebar-button collapsed" data-bs-toggle="collapse" data-bs-target="#two-collapse" aria-expanded="true">可展開第二層標題
                </button>
                <div class="collapse" id="two-collapse">
                  <ul class="sidebar-menu">
                    <li><a href="#" class="sidebar-link">第三層連結內容</a></li>
                    <li><a href="#" class="sidebar-link">第三層連結內容</a></li>
                    <li><a href="#" class="sidebar-link">第三層連結內容</a></li>
                  </ul>
                </div>
              </li>
              <li>
                <button class="sidebar-button collapsed" data-bs-toggle="collapse" data-bs-target="#three-collapse" aria-expanded="true">可展開第二層標題
                </button>
                <div class="collapse" id="three-collapse">
                  <ul class="sidebar-menu">
                    <li><a href="#" class="sidebar-link">第三層連結內容</a></li>
                    <li><a href="#" class="sidebar-link">第三層連結內容</a></li>
                    <li><a href="#" class="sidebar-link">第三層連結內容</a></li>
                  </ul>
                </div>
              </li>
            </ul>
          </div>
        </li>
        <li>
          <button class="sidebar-button collapsed" data-bs-toggle="collapse" data-bs-target="#four-collapse" aria-expanded="true">
            可展開第一層標題
          </button>
          <div class="collapse" id="four-collapse">
            <ul class="sidebar-menu">
              <li>
                <button class="sidebar-button collapsed" data-bs-toggle="collapse" data-bs-target="#five-collapse" aria-expanded="true">可展開第二層標題
                </button>
                <div class="collapse" id="five-collapse">
                  <ul class="sidebar-menu">
                    <li><a href="#" class="sidebar-link">第三層連結內容</a></li>
                    <li><a href="#" class="sidebar-link">第三層連結內容</a></li>
                    <li><a href="#" class="sidebar-link">第三層連結內容</a></li>
                  </ul>
                </div>
              </li>
            </ul>
          </div>
        </li>
      </ul>
    </nav>
  </div>
</div>

<script>
for (const link of document.querySelectorAll(".sidebar-link")) {
  link.addEventListener("click", () => {
    for (const a of document.querySelectorAll(".sidebar-link")) {
      a.classList.remove("active")
    }
    link.classList.add("active")
  });
}
</script>
{{< /example >}}

### 內容頁選單 Linked Items

內容頁選單右側沒有向下的箭頭，點擊後在側邊欄右側反映出相對應的頁面內容。

{{< example >}}
<div class="row d-flex justify-content-center">
  <div class="col-lg-6">
    <nav class="sidebar">
      <ul class="sidebar-body">
        <li><a href="#" class="sidebar-link">第一層連結內容</a></li>
        <li><a href="#" class="sidebar-link">第一層連結內容</a></li>
        <li><a href="#" class="sidebar-link">第一層連結內容</a></li>
        <li><a href="#" class="sidebar-link">第一層連結內容</a></li>
        <li><a href="#" class="sidebar-link">第一層連結內容</a></li>
        <li><a href="#" class="sidebar-link">第一層連結內容</a></li>
      </ul>
    </nav>
  </div>
</div>
<script>
for (const link of document.querySelectorAll(".sidebar-link")) {
  link.addEventListener("click", () => {
    for (const a of document.querySelectorAll(".sidebar-link")) {
      a.classList.remove("active")
    }
    link.classList.add("active")
  });
}
</script>
{{< /example >}}

### 多層混用 Mixed Multilevels

選單可以是單層、兩層或三層，但最多不超過三層。

{{< example >}}
<div class="row d-flex justify-content-center">
  <div class="col-md-6">
    <nav class="sidebar">
      <ul class="sidebar-body">
        <li><a href="#" class="sidebar-link">第一層連結內容</a></li>
        <li>
          <button class="sidebar-button collapsed" data-bs-toggle="collapse" data-bs-target="#multi-collapse" aria-expanded="true">
            可展開第一層標題
          </button>
          <div class="collapse" id="multi-collapse">
            <ul class="sidebar-menu">
              <li><a href="#" class="sidebar-link">第二層連結內容</a></li>
              <li><a href="#" class="sidebar-link">第二層連結內容</a></li>
              <li><a href="#" class="sidebar-link">第二層連結內容</a></li>
            </ul>
          </div>
        </li>
        <li>
          <button class="sidebar-button collapsed" data-bs-toggle="collapse" data-bs-target="#multi-collapse2" aria-expanded="true">
            可展開第一層標題
          </button>
          <div class="collapse" id="multi-collapse2">
            <ul class="sidebar-menu">
              <li><a href="#" class="sidebar-link">第二層連結內容</a></li>
              <li><a href="#" class="sidebar-link">第二層連結內容</a></li>
              <li><a href="#" class="sidebar-link">第二層連結內容</a></li>
              <li>
                <button class="sidebar-button collapsed" data-bs-toggle="collapse" data-bs-target="#multi-collapse3" aria-expanded="true">可展開第二層標題
                </button>
                <div class="collapse" id="multi-collapse3">
                  <ul class="sidebar-menu">
                    <li><a href="#" class="sidebar-link">第三層連結內容</a></li>
                    <li><a href="#" class="sidebar-link">第三層連結內容</a></li>
                  </ul>
                </div>
              </li>
            </ul>
          </div>
        </li>
        <li><a href="#" class="sidebar-link">第一層連結內容</a></li>
      </ul>
    </nav>
  </div>
</div>
<script>
for (const link of document.querySelectorAll(".sidebar-link")) {
  link.addEventListener("click", () => {
    for (const a of document.querySelectorAll(".sidebar-link")) {
      a.classList.remove("active")
    }
    link.classList.add("active")
  });
}
</script>
{{< /example >}}

### 分區 Grouping

選單可以分區顯示，以標題文字區隔。

{{< example >}}
<div class="row d-flex justify-content-center">
  <div class="col-lg-6">
    <nav class="sidebar">
      <ul class="sidebar-body">
        <li><span class="sidebar-subheader">側邊欄分區標題文字</span></li>
        <li><a href="#" class="sidebar-link">第一層連結內容</a></li>
        <li><a href="#" class="sidebar-link">第一層連結內容</a></li>
        <li><a href="#" class="sidebar-link">第一層連結內容</a></li>
        <li class="sidebar-divider"><hr></li>
        <li><span class="sidebar-subheader">側邊欄分區標題文字</span></li>
        <li><a href="#" class="sidebar-link">第一層連結內容</a></li>
        <li><a href="#" class="sidebar-link">第一層連結內容</a></li>
        <li><a href="#" class="sidebar-link">第一層連結內容</a></li>
      </ul>
    </nav>
  </div>
</div>
<script>
for (const link of document.querySelectorAll(".sidebar-link")) {
  link.addEventListener("click", () => {
    for (const a of document.querySelectorAll(".sidebar-link")) {
      a.classList.remove("active")
    }
    link.classList.add("active")
  });
}
</script>
{{< /example >}}

### 圖示  Icon

可以用純文字，不需要圖示。

{{< example >}}
<div class="row d-flex justify-content-center">
  <div class="col-lg-6">
    <nav class="sidebar">
      <ul class="sidebar-body">
        <li><a href="#" class="sidebar-link"><i class="bi bi-signpost-split icon"></i>第一層連結內容</a></li>
        <li><a href="#" class="sidebar-link"><i class="bi bi-signpost-split icon"></i>第一層連結內容</a></li>
        <li><a href="#" class="sidebar-link"><i class="bi bi-signpost-split icon"></i>第一層連結內容</a></li>
        <li><a href="#" class="sidebar-link"><i class="bi bi-signpost-split icon"></i>第一層連結內容</a></li>
        <li><a href="#" class="sidebar-link"><i class="bi bi-signpost-split icon"></i>第一層連結內容</a></li>
        <li><a href="#" class="sidebar-link"><i class="bi bi-signpost-split icon"></i>第一層連結內容</a></li>
      </ul>
    </nav>
  </div>
</div>
<script>
for (const link of document.querySelectorAll(".sidebar-link")) {
  link.addEventListener("click", () => {
    for (const a of document.querySelectorAll(".sidebar-link")) {
      a.classList.remove("active")
    }
    link.classList.add("active")
  });
}
</script>
{{< /example >}}

### 徽章  Badge

可以用 badge 顯示某一連結項目的狀態。這樣的做法可以呈現出 stepper 的樣式。

{{< example >}}
<div class="row d-flex justify-content-center">
  <div class="col-lg-6">
    <nav class="sidebar">
      <ul class="sidebar-body">
        <li><a href="#" class="sidebar-link">第一層連結內容<span class="badge bg-positive-flat">已完成</span></a></li>
        <li><a href="#" class="sidebar-link">第一層連結內容<span class="badge bg-negative-flat badge-numerical">2</span></a></li>
        <li><a href="#" class="sidebar-link">第一層連結內容</a></li>
        <li><a href="#" class="sidebar-link">第一層連結內容</a></li>
        <li><a href="#" class="sidebar-link">第一層連結內容</a></li>
        <li><a href="#" class="sidebar-link">第一層連結內容</a></li>
      </ul>
    </nav>
  </div>
</div>
<script>
for (const link of document.querySelectorAll(".sidebar-link")) {
  link.addEventListener("click", () => {
    for (const a of document.querySelectorAll(".sidebar-link")) {
      a.classList.remove("active")
    }
    link.classList.add("active")
  });
}
</script>
{{< /example >}}

### 標題  Heading

在側邊欄上面加上標題文字

{{< example >}}
<div class="row d-flex justify-content-center">
  <div class="col-lg-6">
    <nav class="sidebar">
      <div class="sidebar-header">側邊欄標題文字</div>
      <ul class="sidebar-body">
        <li><span class="sidebar-subheader">側邊欄分區標題文字</span></li>
        <li><a href="#" class="sidebar-link">第一層連結內容</a></li>
        <li><a href="#" class="sidebar-link">第一層連結內容</a></li>
        <li><a href="#" class="sidebar-link">第一層連結內容</a></li>
        <li class="sidebar-divider"><hr></li>
        <li><span class="sidebar-subheader">側邊欄分區標題文字</span></li>
        <li><a href="#" class="sidebar-link">第一層連結內容</a></li>
        <li><a href="#" class="sidebar-link">第一層連結內容</a></li>
        <li><a href="#" class="sidebar-link">第一層連結內容</a></li>
      </ul>
    </nav>
  </div>
</div>
<script>
for (const link of document.querySelectorAll(".sidebar-link")) {
  link.addEventListener("click", () => {
    for (const a of document.querySelectorAll(".sidebar-link")) {
      a.classList.remove("active")
    }
    link.classList.add("active")
  });
}
</script>
{{< /example >}}


## 範例
關於側邊欄在響應式設計中的變形，以及側邊欄與頁首搭配時的見識使用方式，請詳見[模板 (Navigation Starter)](/docs/pattern/navigation_starter)。
