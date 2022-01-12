---
layout: docs
title: 側邊欄 Sidebar
description: 放置頁面一邊的具層級性、垂直排列的導覽
group: components
toc: true
---

### 關於側邊欄元件

側邊欄為導覽用的元件，通常與頂部導覽搭配使用，適合當網站資訊架構較為複雜、層級較多時使用。側邊欄可以呈現一到三層級的選項，第一層級的選項最少五項。根據米勒定律 (Miller’s law) 一般人短期記憶中能容納的物體數量為七加減二，所以第一層級的選項也請儘量維持在九項以下。第二層級沒有特別規定，但若超過九項時，請審慎考慮網站的架構規劃。第三層級因為已到達直接呈現後點擊的用途，連結數量上並沒有一定限制。

<img class="img-fluid" src="../docs/5.1/assets/img/sidebar_illustration.png">

### 使用規範

#### 何時該使用側邊欄

- **呈現一到三層級的導覽架構。** 側邊欄至少一層且第一層級至少五項，層級數目則至多三層。
- **呈現網站分區中的次層級導覽。** 當網站有明顯分區且次層級較多時，善用側邊欄輔助頂部導覽列。
- **有層級的常用服務之快速導覽。** 當網站有明顯較常用的服務存在且多於五項又有層級架構時，利用側邊欄作為整個網站的快速導覽。

#### 何時該考慮使用其他元件

- **小網站。** 當網站架構簡單、層級數少時，不需用到側邊欄。
- **已有導覽存在。** 當網站架構簡單，頂部導覽即可有效的引導使用者時，不需用到側邊欄。
- **需要用文字標題以外的元素描述時。** 當文字標題不足以描述使用者即將前往的頁面時，請考慮用其他元件，例如卡片。
- **數量少的常用服務之快速導覽。** 當有替常用服務做快速導覽的需求時，若層級簡單則不需用到側邊欄，可以考慮使用其他元件如卡片，橫向呈列常見服務。
- **選項為僅供瀏覽但不可以點擊的資訊。** 當列出的選項僅為瀏覽用但不為導覽用時，請勿使用導覽列。

#### 側邊欄易用性

- **文字標題簡短。** 請保持文字標題簡短易懂，且在單行呈現文字標題。
- **用狀態呈現目前選擇。** 利用風格區別已選擇或未選擇的選項，通常使用狀態 (actvie state) 來區別。
- **側邊欄內比較不常用的選擇放在比較下方。** 使用者的注意力會從側邊欄的選項中從上至下瀏覽，因此為了幫助使用者方便且迅速的到達對的頁面，請將比較不常見的選擇放在欄位較為下方的位置。
- **請勿用過於華麗的特效展開、收納導覽列。** 導覽的用除在於幫助使用者找到對的頁面與內容，請勿將導覽列的風格或視覺做得過於花俏反而喧賓奪主，影響使用者的注意力。
- **請勿在側邊欄呈現跟其他導覽列完全一樣的內容。** 當側邊欄與頂部導覽列同時存在時，側邊欄的存在目的為輔助頂部導覽列，完全將頂部導覽列的內容全部複製到側邊欄。
- **請勿為了填滿空間而使用側邊欄。** 側邊欄的存在目的為導覽，當頁面很簡單乾淨時，切勿為了填滿空間而執意製作一個側邊導覽列。空白空間的存在可以幫助使用者將注意力放在對的地方。
- **請勿只以圖標 (icon) 呈現側邊欄。** 側邊欄的存在目的為導覽，且應能幫助使用者迅速地看到欲點擊選項。勿為省略文字標題，而只以圖標暗示。請勿讓使用者花額外時間猜測圖標背後代表的意義。

### 設計元件

#### 基本款 - Default & Small

基本款的側邊欄有舒適行高 (comfortable height) 與壓縮行高 (compact height) 兩種選擇，請依據網站空間自行調配。

{{< example >}}

<div class="row">
  <div class="col-md-6">
    <div class="sidebar" id="sidebar">
      <div class="accordion-item">
        <h2 class="sidebar-header" id="headerone">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseone" aria-expanded="true" aria-controls="collapseone">
            可展開第一層標題
          </button>
        </h2>
        <div id="collapseone" class="sidebar-collapse collapse" aria-labelledby="headerone" data-bs-parent="#sidebar">
          <div class="sidebar-second-layer" id="sidebarsecondlayer">
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="secondlayerheaderone">
                <button class="accordion-button sidebar-button sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#secondlayercollapseone" aria-expanded="true" aria-controls="secondlayercollapseone">
                  可展開第二層標題
                </button>
              </h2>
              <div id="secondlayercollapseone" class="sidebar-collapse collapse" aria-labelledby="secondlayerheaderone" data-bs-parent="#sidebarsecondlayer">
              </div>
            </div>
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="secondlayerheadertwo">
                <button class="accordion-button sidebar-button sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#secondlayercollapsetwo" aria-expanded="true" aria-controls="secondlayercollapsetwo">
                  可展開第二層標題
                </button>
              </h2>
              <div id="secondlayercollapsetwo" class="sidebar-collapse collapse" aria-labelledby="secondlayerheadertwo" data-bs-parent="#sidebarsecondlayer">
                <div class="list-group">
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">
                    可點擊服務連結
                  </a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action active" aria-current="true">瀏覽中服務連結</a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">可點擊服務連結</a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">可點擊服務連結</a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="sidebar-header" id="headertwo">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapsetwo" aria-expanded="true" aria-controls="collapsetwo">
            可展開第一層標題
          </button>
        </h2>
        <div id="collapsetwo" class="sidebar-collapse collapse" aria-labelledby="headertwo" data-bs-parent="#sidebar">
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="sidebar-header" id="headerthree">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapsethree" aria-expanded="true" aria-controls="collapsethree">
            可展開第一層標題
          </button>
        </h2>
        <div id="collapsethree" class="sidebar-collapse collapse" aria-labelledby="headerthree" data-bs-parent="#sidebar">
        </div>
      </div>
    </div>
  </div>
  <div class="col-md-6">
    <div class="sidebar-dense" id="sidebardense">
      <div class="accordion-item">
        <h2 class="sidebar-header" id="headeronedense">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseonedense" aria-expanded="true" aria-controls="collapseonedense">
            可展開第一層標題
          </button>
        </h2>
        <div id="collapseonedense" class="sidebar-collapse collapse" aria-labelledby="headeronedense" data-bs-parent="#sidebardense">
          <div class="sidebar-second-layer" id="sidebarsecondlayerdense">
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="secondlayerheaderonedense">
                <button class="accordion-button sidebar-button sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#secondlayercollapseonedense" aria-expanded="true" aria-controls="secondlayercollapseonedense">
                  可展開第二層標題
                </button>
              </h2>
              <div id="secondlayercollapseonedense" class="sidebar-collapse collapse" aria-labelledby="secondlayerheaderonedense" data-bs-parent="#sidebarsecondlayerdense">
              </div>
            </div>
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="secondlayerheadertwodense">
                <button class="accordion-button sidebar-button sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#secondlayercollapsetwodense" aria-expanded="true" aria-controls="secondlayercollapsetwodense">
                  可展開第二層標題
                </button>
              </h2>
              <div id="secondlayercollapsetwodense" class="sidebar-collapse collapse" aria-labelledby="secondlayerheadertwodense" data-bs-parent="#sidebarsecondlayerdense">
                <div class="list-group">
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">
                    可點擊服務連結
                  </a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action active" aria-current="true">瀏覽中服務連結</a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">可點擊服務連結</a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">可點擊服務連結</a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="sidebar-header" id="headertwodense">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapsetwodense" aria-expanded="true" aria-controls="collapsetwodense">
            可展開第一層標題
          </button>
        </h2>
        <div id="collapsetwodense" class="sidebar-collapse collapse" aria-labelledby="headertwodense" data-bs-parent="#sidebardense">
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="sidebar-header" id="headerthreedense">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapsethreedense" aria-expanded="true" aria-controls="collapsethreedense">
            可展開第一層標題
          </button>
        </h2>
        <div id="collapsethreedense" class="sidebar-collapse collapse" aria-labelledby="headerthreedense" data-bs-parent="#sidebardense">
        </div>
      </div>
    </div>
  </div>
</div>

{{< /example >}}

#### 側欄主標題

側欄上方可以放置一行主標題文字，概述側欄內容，例如：常用服務、快速導覽。

{{< example >}}

<div class="row">
  <div class="col-md-6">
    <div class="sidebar" id="sidebar2">
      <div class="accordion-item">
        <h2 class="sidebar-header" id="headerone2">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseone2" aria-expanded="true" aria-controls="collapseone2">
            可展開第一層標題
          </button>
        </h2>
        <div id="collapseone2" class="sidebar-collapse collapse" aria-labelledby="headerone2" data-bs-parent="#sidebar2">
          <div class="sidebar-second-layer" id="sidebarsecondlayer2">
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="secondlayerheaderone2">
                <button class="accordion-button sidebar-button sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#secondlayercollapseone2" aria-expanded="true" aria-controls="secondlayercollapseone2">
                  可展開第二層標題
                </button>
              </h2>
              <div id="secondlayercollapseone2" class="sidebar-collapse collapse" aria-labelledby="secondlayerheaderone2" data-bs-parent="#sidebarsecondlayer2">
              </div>
            </div>
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="secondlayerheadertwo2">
                <button class="accordion-button sidebar-button sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#secondlayercollapsetwo2" aria-expanded="true" aria-controls="secondlayercollapsetwo2">
                  可展開第二層標題
                </button>
              </h2>
              <div id="secondlayercollapsetwo2" class="sidebar-collapse collapse" aria-labelledby="secondlayerheadertwo2" data-bs-parent="#sidebarsecondlayer2">
                <div class="list-group">
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">
                    可點擊服務連結
                  </a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action active" aria-current="true">瀏覽中服務連結</a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">可點擊服務連結</a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">可點擊服務連結</a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="sidebar-header" id="headertwo2">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapsetwo2" aria-expanded="true" aria-controls="collapsetwo2">
            可展開第一層標題
          </button>
        </h2>
        <div id="collapsetwo2" class="sidebar-collapse collapse" aria-labelledby="headertwo2" data-bs-parent="#sidebar2">
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="sidebar-header" id="headerthree2">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapsethree2" aria-expanded="true" aria-controls="collapsethree2">
            可展開第一層標題
          </button>
        </h2>
        <div id="collapsethree2" class="sidebar-collapse collapse" aria-labelledby="headerthree2" data-bs-parent="#sidebar2">
        </div>
      </div>
    </div>
  </div>
  <div class="col-md-6">
    <h4>側欄主標題</h4>
    <div class="sidebar" id="title-sidebar">
      <div class="accordion-item">
        <h2 class="sidebar-header" id="headerone3">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseone3" aria-expanded="true" aria-controls="collapseone3">
            可展開第一層標題
          </button>
        </h2>
        <div id="collapseone3" class="sidebar-collapse collapse" aria-labelledby="headerone3" data-bs-parent="#title-sidebar">
          <div class="sidebar-second-layer" id="sidebarsecondlayer3">
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="secondlayerheaderone3">
                <button class="accordion-button sidebar-button sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#secondlayercollapseone3" aria-expanded="true" aria-controls="secondlayercollapseone3">
                  可展開第二層標題
                </button>
              </h2>
              <div id="secondlayercollapseone3" class="sidebar-collapse collapse" aria-labelledby="secondlayerheaderone3" data-bs-parent="#sidebarsecondlayer3">
              </div>
            </div>
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="secondlayerheadertwo3">
                <button class="accordion-button sidebar-button sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#secondlayercollapsetwo3" aria-expanded="true" aria-controls="secondlayercollapsetwo3">
                  可展開第二層標題
                </button>
              </h2>
              <div id="secondlayercollapsetwo3" class="sidebar-collapse collapse" aria-labelledby="secondlayerheadertwo3" data-bs-parent="#sidebarsecondlayer3">
                <div class="list-group">
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">
                    可點擊服務連結
                  </a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action active" aria-current="true">瀏覽中服務連結</a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">可點擊服務連結</a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">可點擊服務連結</a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="sidebar-header" id="headertwo3">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapsetwo3" aria-expanded="true" aria-controls="collapsetwo3">
            可展開第一層標題
          </button>
        </h2>
        <div id="collapsetwo3" class="sidebar-collapse collapse" aria-labelledby="headertwo3" data-bs-parent="#title-sidebar">
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="sidebar-header" id="headerthree3">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapsethree3" aria-expanded="true" aria-controls="collapsethree3">
            可展開第一層標題
          </button>
        </h2>
        <div id="collapsethree3" class="sidebar-collapse collapse" aria-labelledby="headerthree3" data-bs-parent="#title-sidebar">
        </div>
      </div>
    </div>
  </div>
</div>

{{< /example >}}

#### 展開全部

您可以依需求選擇性加上「展開全部」的功能，以用來一次展開所有層級，方便導覽。

{{< example >}}

<div class="row">
  <div class="col-md-6">
    <div class="d-flex justify-content-between">
      <h4>側欄主標題</h4>
      <a href="#" OnClick='Collapse()'>展開全部</a>
    </div>
    <div class="sidebar" id="js-sidebar">
      <div class="accordion-item">
        <h2 class="sidebar-header" id="js-headerone">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#js-collapseone" aria-expanded="true" aria-controls="js-collapseone">
            可展開第一層標題
          </button>
        </h2>
        <div id="js-collapseone" class="sidebar-collapse collapse" aria-labelledby="js-headerone" data-bs-parent="#js-sidebar">
          <div class="sidebar-second-layer" id="js-sidebarsecondlayer">
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="js-secondlayerheaderone">
                <button class="accordion-button sidebar-button sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#js-secondlayercollapseone" aria-expanded="true" aria-controls="js-secondlayercollapseone">
                  可展開第二層標題
                </button>
              </h2>
              <div id="js-secondlayercollapseone" class="sidebar-collapse collapse" aria-labelledby="js-secondlayerheaderone" data-bs-parent="#js-sidebarsecondlayer">
              </div>
            </div>
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="js-secondlayerheadertwo">
                <button class="accordion-button sidebar-button sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#js-secondlayercollapsetwo" aria-expanded="true" aria-controls="js-secondlayercollapsetwo">
                  可展開第二層標題
                </button>
              </h2>
              <div id="js-secondlayercollapsetwo" class="sidebar-collapse collapse" aria-labelledby="js-secondlayerheadertwo" data-bs-parent="#js-sidebarsecondlayer">
                <div class="list-group">
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">
                    可點擊服務連結
                  </a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action active" aria-current="true">瀏覽中服務連結</a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">可點擊服務連結</a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">可點擊服務連結</a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="sidebar-header" id="js-headertwo">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#js-collapsetwo" aria-expanded="true" aria-controls="js-collapsetwo">
            可展開第一層標題
          </button>
        </h2>
        <div id="js-collapsetwo" class="sidebar-collapse collapse" aria-labelledby="js-headertwo" data-bs-parent="#js-sidebar">
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="sidebar-header" id="js-headerthree">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#js-collapsethree" aria-expanded="true" aria-controls="js-collapsethree">
            可展開第一層標題
          </button>
        </h2>
        <div id="js-collapsethree" class="sidebar-collapse collapse" aria-labelledby="js-headerthree" data-bs-parent="#js-sidebar">
        </div>
      </div>
    </div>
  </div>
</div>

<script>

const Collapse = () => {
  var container = document.querySelector("#js-sidebar")
  var collapseElementList = [].slice.call(container.querySelectorAll('.collapse'))
  var collapseList = collapseElementList.map(function (collapseEl) {
    return new bootstrap.Collapse(collapseEl)
  })
}

</script>

{{< /example >}}

#### 指標 (indicator) 位置

預設的箭頭指標預設為靠右對齊，文字標題左側則可以加上簡單且風格一致的圖標 (icon)。
您也可以選擇不用圖標輔助文字標題，並將箭頭指標靠左對齊。

{{< example >}}

<div class="row">
  <div class="col-md-6">
    <div class="sidebar" id="indicator-sidebar">
      <div class="accordion-item">
        <h2 class="sidebar-header" id="indicator-headerone">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#indicator-collapseone" aria-expanded="true" aria-controls="indicator-collapseone">
            <i class="bi bi-house-door-fill icon"></i>可展開第一層標題
          </button>
        </h2>
        <div id="indicator-collapseone" class="sidebar-collapse collapse" aria-labelledby="indicator-headerone" data-bs-parent="#indicator-sidebar">
          <div class="sidebar-second-layer" id="indicator-sidebarsecondlayer">
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="indicator-secondlayerheaderone">
                <button class="accordion-button sidebar-button sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#indicator-secondlayercollapseone" aria-expanded="true" aria-controls="indicator-secondlayercollapseone">
                  <i class="bi bi-credit-card-2-front icon"></i>可展開第二層標題
                </button>
              </h2>
              <div id="indicator-secondlayercollapseone" class="sidebar-collapse collapse" aria-labelledby="indicator-secondlayerheaderone" data-bs-parent="#indicator-sidebarsecondlayer">
              </div>
            </div>
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="secondlayerheadertwo">
                <button class="accordion-button sidebar-button sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#indicator-secondlayercollapsetwo" aria-expanded="true" aria-controls="indicator-secondlayercollapsetwo">
                  <i class="bi bi-clipboard icon"></i>可展開第二層標題
                </button>
              </h2>
              <div id="indicator-secondlayercollapsetwo" class="sidebar-collapse collapse" aria-labelledby="indicator-secondlayerheadertwo" data-bs-parent="#indicator-sidebarsecondlayer">
                <div class="list-group">
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">
                    可點擊服務連結
                  </a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action active" aria-current="true">瀏覽中服務連結</a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">可點擊服務連結</a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">可點擊服務連結</a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="sidebar-header" id="indicator-headertwo">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#indicator-collapsetwo" aria-expanded="true" aria-controls="indicator-collapsetwo">
            <i class="bi bi-puzzle-fill icon"></i>可展開第一層標題
          </button>
        </h2>
        <div id="indicator-collapsetwo" class="sidebar-collapse collapse" aria-labelledby="indicator-headertwo" data-bs-parent="#indicator-sidebar">
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="sidebar-header" id="indicator-headerthree">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#indicator-collapsethree" aria-expanded="true" aria-controls="indicator-collapsethree">
            <i class="bi bi-inboxes icon"></i>可展開第一層標題
          </button>
        </h2>
        <div id="indicator-collapsethree" class="sidebar-collapse collapse" aria-labelledby="indicator-headerthree" data-bs-parent="#indicator-sidebar">
        </div>
      </div>
    </div>
  </div>
  <div class="col-md-6">
    <div class="sidebar-reversed" id="sidebar-reversed">
      <div class="accordion-item">
        <h2 class="sidebar-header" id="headerone-reversed">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseone-reversed" aria-expanded="true" aria-controls="collapseone-reversed">
            可展開第一層標題
          </button>
        </h2>
        <div id="collapseone-reversed" class="sidebar-collapse collapse" aria-labelledby="headerone-reversed" data-bs-parent="#sidebar-reversed">
          <div class="sidebar-second-layer" id="sidebarsecondlayer-reversed">
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="secondlayerheaderone-reversed">
                <button class="accordion-button sidebar-button sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#secondlayercollapseone-reversed" aria-expanded="true" aria-controls="secondlayercollapseone-reversed">
                  可展開第二層標題
                </button>
              </h2>
              <div id="secondlayercollapseone-reversed" class="sidebar-collapse collapse" aria-labelledby="secondlayerheaderone-reversed" data-bs-parent="#sidebarsecondlayer-reversed">
              </div>
            </div>
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="secondlayerheadertwo-reversed">
                <button class="accordion-button sidebar-button sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#secondlayercollapsetwo" aria-expanded="true" aria-controls="secondlayercollapsetwo">
                  可展開第二層標題
                </button>
              </h2>
              <div id="secondlayercollapsetwo" class="sidebar-collapse collapse" aria-labelledby="secondlayerheadertwo-reversed" data-bs-parent="#sidebarsecondlayer-reversed">
                <div class="list-group">
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">
                    可點擊服務連結
                  </a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action active" aria-current="true">瀏覽中服務連結</a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">可點擊服務連結</a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">可點擊服務連結</a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="sidebar-header" id="headertwo-reversed">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapsetwo-reversed" aria-expanded="true" aria-controls="collapsetwo-reversed">
            可展開第一層標題
          </button>
        </h2>
        <div id="collapsetwo-reversed" class="sidebar-collapse collapse" aria-labelledby="headertwo-reversed" data-bs-parent="#sidebar-reversed">
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="sidebar-header" id="headerthree-reversed">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapsethree-reversed" aria-expanded="true" aria-controls="collapsethree-reversed">
            可展開第一層標題
          </button>
        </h2>
        <div id="collapsethree-reversed" class="sidebar-collapse collapse" aria-labelledby="headerthree-reversed" data-bs-parent="#sidebar-reversed">
        </div>
      </div>
    </div>
  </div>
</div>

{{< /example >}}

#### 圖標 (icon)

預設的箭頭指標預設為靠右對齊，文字標題左側則可以加上簡單且風格一致的圖標 (icon)。箭頭指標靠左對齊時則請勿再加圖標。

{{< example >}}

<div class="row">
  <div class="col-md-6">
    <div class="sidebar" id="icon-sidebar">
      <div class="accordion-item">
        <h2 class="sidebar-header" id="icon-headerone">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#icon-collapseone" aria-expanded="true" aria-controls="icon-collapseone">
            <i class="bi bi-house-door-fill icon"></i>可展開第一層標題
          </button>
        </h2>
        <div id="icon-collapseone" class="sidebar-collapse collapse" aria-labelledby="icon-headerone" data-bs-parent="#icon-sidebar">
          <div class="sidebar-second-layer" id="icon-sidebarsecondlayer">
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="icon-secondlayerheaderone">
                <button class="accordion-button sidebar-button sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#icon-secondlayercollapseone" aria-expanded="true" aria-controls="icon-secondlayercollapseone">
                  <i class="bi bi-credit-card-2-front icon"></i>可展開第二層標題
                </button>
              </h2>
              <div id="icon-secondlayercollapseone" class="sidebar-collapse collapse" aria-labelledby="icon-secondlayerheaderone" data-bs-parent="#icon-sidebarsecondlayer">
              </div>
            </div>
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="secondlayerheadertwo">
                <button class="accordion-button sidebar-button sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#icon-secondlayercollapsetwo" aria-expanded="true" aria-controls="icon-secondlayercollapsetwo">
                  <i class="bi bi-clipboard icon"></i>可展開第二層標題
                </button>
              </h2>
              <div id="icon-secondlayercollapsetwo" class="sidebar-collapse collapse" aria-labelledby="icon-secondlayerheadertwo" data-bs-parent="#icon-sidebarsecondlayer">
                <div class="list-group">
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">
                    可點擊服務連結
                  </a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action active" aria-current="true">瀏覽中服務連結</a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">可點擊服務連結</a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">可點擊服務連結</a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="sidebar-header" id="icon-headertwo">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#icon-collapsetwo" aria-expanded="true" aria-controls="icon-collapsetwo">
            <i class="bi bi-puzzle-fill icon"></i>可展開第一層標題
          </button>
        </h2>
        <div id="icon-collapsetwo" class="sidebar-collapse collapse" aria-labelledby="icon-headertwo" data-bs-parent="#icon-sidebar">
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="sidebar-header" id="icon-headerthree">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#icon-collapsethree" aria-expanded="true" aria-controls="icon-collapsethree">
            <i class="bi bi-inboxes icon"></i>可展開第一層標題
          </button>
        </h2>
        <div id="icon-collapsethree" class="sidebar-collapse collapse" aria-labelledby="icon-headerthree" data-bs-parent="#icon-sidebar">
        </div>
      </div>
    </div>
  </div>
</div>

{{< /example >}}

#### 指標 (indicator) 類型

預設為單線條的箭頭指標，但您也可以視情況替換為實心箭頭指標或是加減符號。非不得已請勿使用其他圖示，惟在選擇其他圖示時也請選擇可以暗示使用者「此列為可點擊展開」之圖示。

{{< example >}}

<div class="row">
  <div class="col-md-4">
    <div class="sidebar" id="base-indicator-sidebar">
      <div class="accordion-item">
        <h2 class="sidebar-header" id="base-indicator-headerone">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#base-indicator-collapseone" aria-expanded="true" aria-controls="base-indicator-collapseone">
            可展開第一層標題
          </button>
        </h2>
        <div id="base-indicator-collapseone" class="sidebar-collapse collapse" aria-labelledby="base-indicator-headerone" data-bs-parent="#base-indicator-sidebar">
          <div class="sidebar-second-layer" id="base-indicator-sidebarsecondlayer">
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="base-indicator-secondlayerheaderone">
                <button class="accordion-button sidebar-button sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#base-indicator-secondlayercollapseone" aria-expanded="true" aria-controls="base-indicator-secondlayercollapseone">
                  可展開第二層標題
                </button>
              </h2>
              <div id="base-indicator-secondlayercollapseone" class="sidebar-collapse collapse" aria-labelledby="base-indicator-secondlayerheaderone" data-bs-parent="#base-indicator-sidebarsecondlayer">
              </div>
            </div>
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="base-indicator-secondlayerheadertwo">
                <button class="accordion-button sidebar-button sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#base-indicator-secondlayercollapsetwo" aria-expanded="true" aria-controls="base-indicator-secondlayercollapsetwo">
                  可展開第二層標題
                </button>
              </h2>
              <div id="base-indicator-secondlayercollapsetwo" class="sidebar-collapse collapse" aria-labelledby="base-indicator-secondlayerheadertwo" data-bs-parent="#base-indicator-sidebarsecondlayer">
                <div class="list-group">
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">
                    可點擊服務連結
                  </a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action active" aria-current="true">瀏覽中服務連結</a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">可點擊服務連結</a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">可點擊服務連結</a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="sidebar-header" id="base-indicator-headertwo">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#base-indicator-collapsetwo" aria-expanded="true" aria-controls="base-indicator-collapsetwo">
            可展開第一層標題
          </button>
        </h2>
        <div id="base-indicator-collapsetwo" class="sidebar-collapse collapse" aria-labelledby="base-indicator-headertwo" data-bs-parent="#base-indicator-sidebar">
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="sidebar-header" id="base-indicator-headerthree">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#base-indicator-collapsethree" aria-expanded="true" aria-controls="base-indicator-collapsethree">
            可展開第一層標題
          </button>
        </h2>
        <div id="base-indicator-collapsethree" class="sidebar-collapse collapse" aria-labelledby="base-indicator-headerthree" data-bs-parent="#base-indicator-sidebar">
        </div>
      </div>
    </div>
  </div>
    <div class="col-md-4">
    <div class="sidebar-caret" id="caret-indicator-sidebar">
      <div class="accordion-item">
        <h2 class="sidebar-header" id="caret-indicator-headerone">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#caret-indicator-collapseone" aria-expanded="true" aria-controls="caret-indicator-collapseone">
            可展開第一層標題
          </button>
        </h2>
        <div id="caret-indicator-collapseone" class="sidebar-collapse collapse" aria-labelledby="caret-indicator-headerone" data-bs-parent="#caret-indicator-sidebar">
          <div class="sidebar-second-layer" id="caret-indicator-sidebarsecondlayer">
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="caret-indicator-secondlayerheaderone">
                <button class="accordion-button sidebar-button sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#caret-indicator-secondlayercollapseone" aria-expanded="true" aria-controls="caret-indicator-secondlayercollapseone">
                  可展開第二層標題
                </button>
              </h2>
              <div id="caret-indicator-secondlayercollapseone" class="sidebar-collapse collapse" aria-labelledby="caret-indicator-secondlayerheaderone" data-bs-parent="#caret-indicator-sidebarsecondlayer">
              </div>
            </div>
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="caret-indicator-secondlayerheadertwo">
                <button class="accordion-button sidebar-button sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#caret-indicator-secondlayercollapsetwo" aria-expanded="true" aria-controls="caret-indicator-secondlayercollapsetwo">
                  可展開第二層標題
                </button>
              </h2>
              <div id="caret-indicator-secondlayercollapsetwo" class="sidebar-collapse collapse" aria-labelledby="caret-indicator-secondlayerheadertwo" data-bs-parent="#caret-indicator-sidebarsecondlayer">
                <div class="list-group">
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">
                    可點擊服務連結
                  </a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action active" aria-current="true">瀏覽中服務連結</a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">可點擊服務連結</a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">可點擊服務連結</a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="sidebar-header" id="caret-indicator-headertwo">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#caret-indicator-collapsetwo" aria-expanded="true" aria-controls="caret-indicator-collapsetwo">
            可展開第一層標題
          </button>
        </h2>
        <div id="caret-indicator-collapsetwo" class="sidebar-collapse collapse" aria-labelledby="caret-indicator-headertwo" data-bs-parent="#caret-indicator-sidebar">
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="sidebar-header" id="caret-indicator-headerthree">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#caret-indicator-collapsethree" aria-expanded="true" aria-controls="caret-indicator-collapsethree">
            可展開第一層標題
          </button>
        </h2>
        <div id="caret-indicator-collapsethree" class="sidebar-collapse collapse" aria-labelledby="caret-indicator-headerthree" data-bs-parent="#caret-indicator-sidebar">
        </div>
      </div>
    </div>
  </div>
    <div class="col-md-4">
    <div class="sidebar-plus" id="plus-indicator-sidebar">
      <div class="accordion-item">
        <h2 class="sidebar-header" id="plus-indicator-headerone">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#plus-indicator-collapseone" aria-expanded="true" aria-controls="plus-indicator-collapseone">
            可展開第一層標題
          </button>
        </h2>
        <div id="plus-indicator-collapseone" class="sidebar-collapse collapse" aria-labelledby="plus-indicator-headerone" data-bs-parent="#plus-indicator-sidebar">
          <div class="sidebar-second-layer" id="plus-indicator-sidebarsecondlayer">
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="plus-indicator-secondlayerheaderone">
                <button class="accordion-button sidebar-button sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#plus-indicator-secondlayercollapseone" aria-expanded="true" aria-controls="plus-indicator-secondlayercollapseone">
                  可展開第二層標題
                </button>
              </h2>
              <div id="plus-indicator-secondlayercollapseone" class="sidebar-collapse collapse" aria-labelledby="plus-indicator-secondlayerheaderone" data-bs-parent="#plus-indicator-sidebarsecondlayer">
              </div>
            </div>
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="plus-indicator-secondlayerheadertwo">
                <button class="accordion-button sidebar-button sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#plus-indicator-secondlayercollapsetwo" aria-expanded="true" aria-controls="plus-indicator-secondlayercollapsetwo">
                  可展開第二層標題
                </button>
              </h2>
              <div id="plus-indicator-secondlayercollapsetwo" class="sidebar-collapse collapse" aria-labelledby="plus-indicator-secondlayerheadertwo" data-bs-parent="#plus-indicator-sidebarsecondlayer">
                <div class="list-group">
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">
                    可點擊服務連結
                  </a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action active" aria-current="true">瀏覽中服務連結</a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">可點擊服務連結</a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">可點擊服務連結</a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="sidebar-header" id="plus-indicator-headertwo">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#plus-indicator-collapsetwo" aria-expanded="true" aria-controls="plus-indicator-collapsetwo">
            可展開第一層標題
          </button>
        </h2>
        <div id="plus-indicator-collapsetwo" class="sidebar-collapse collapse" aria-labelledby="plus-indicator-headertwo" data-bs-parent="#plus-indicator-sidebar">
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="sidebar-header" id="plus-indicator-headerthree">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#plus-indicator-collapsethree" aria-expanded="true" aria-controls="plus-indicator-collapsethree">
            可展開第一層標題
          </button>
        </h2>
        <div id="plus-indicator-collapsethree" class="sidebar-collapse collapse" aria-labelledby="plus-indicator-headerthree" data-bs-parent="#plus-indicator-sidebar">
        </div>
      </div>
    </div>
  </div>
</div>

{{< /example >}}

#### 標籤 (Label)

側邊欄為導覽用，其目的為讓使用者將注意力方在對的頁面內容上，而不是側邊欄本身。請謹慎評估使用者注意力的負擔，確認標籤的使用可以大幅度輔助導流，並謹慎使用標籤。

{{< example >}}

<div class="row">
  <div class="col-md-6">
    <div class="sidebar-icon-label" id="icon-label-sidebar">
      <div class="accordion-item">
        <h2 class="sidebar-header" id="icon-headerone">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#icon-label-collapseone" aria-expanded="true" aria-controls="icon-label-collapseone">
            <div class="sidebar-button-container d-flex">
              <i class="bi bi-house-door-fill icon"></i><p class="sidebar-button-text flex-grow-1 align-self-center">可展開第一層標題</p><span class="sidebar-button-badge bg-secondary text-dark">文字標籤</span>
            </div>
          </button>
        </h2>
        <div id="icon-label-collapseone" class="sidebar-collapse collapse" aria-labelledby="icon-label-headerone" data-bs-parent="#icon-label-sidebar">
          <div class="sidebar-second-layer" id="icon-label-sidebarsecondlayer">
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="icon-label-secondlayerheaderone">
                <button class="accordion-button sidebar-button sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#icon-label-secondlayercollapseone" aria-expanded="true" aria-controls="icon-label-secondlayercollapseone">
                  <i class="bi bi-credit-card-2-front icon"></i>可展開第二層標題
                </button>
              </h2>
              <div id="icon-label-secondlayercollapseone" class="sidebar-collapse collapse" aria-labelledby="icon-label-secondlayerheaderone" data-bs-parent="#icon-label-sidebarsecondlayer">
              </div>
            </div>
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="secondlayerheadertwo">
                <button class="accordion-button sidebar-button sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#icon-label-secondlayercollapsetwo" aria-expanded="true" aria-controls="icon-label-secondlayercollapsetwo">
                 <div class="sidebar-button-container d-flex">
                  <i class="bi bi-clipboard icon"></i><p class="sidebar-button-text flex-grow-1 align-self-center">可展開第二層標題</p><span class="sidebar-button-badge-round rounded-pill">12</span>
                </div>
              </h2>
              <div id="icon-label-secondlayercollapsetwo" class="sidebar-collapse collapse" aria-labelledby="icon-label-secondlayerheadertwo" data-bs-parent="#icon-label-sidebarsecondlayer">
                <div class="list-group">
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">
                    可點擊服務連結
                  </a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action active" aria-current="true">瀏覽中服務連結</a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">可點擊服務連結</a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">可點擊服務連結</a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="sidebar-header" id="icon-label-headertwo">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#icon-label-collapsetwo" aria-expanded="true" aria-controls="icon-label-collapsetwo">
            <div class="sidebar-button-container d-flex">
              <i class="bi bi-puzzle-fill icon"></i><p class="sidebar-button-text flex-grow-1 align-self-center">可展開第一層標題</p><span class="sidebar-button-badge bg-secondary text-dark">文字標籤</span>
            </div>
          </button>
        </h2>
        <div id="icon-label-collapsetwo" class="sidebar-collapse collapse" aria-labelledby="icon-label-headertwo" data-bs-parent="#icon-label-sidebar">
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="sidebar-header" id="icon-label-headerthree">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#icon-label-collapsethree" aria-expanded="true" aria-controls="icon-label-collapsethree">
            <i class="bi bi-inboxes icon"></i>可展開第一層標題
          </button>
        </h2>
        <div id="icon-label-collapsethree" class="sidebar-collapse collapse" aria-labelledby="icon-label-headerthree" data-bs-parent="#icon-label-sidebar">
        </div>
      </div>
    </div>
  </div>
  <div class="col-md-6">
    <div class="sidebar-reversed" id="sidebar-reversed-label">
      <div class="accordion-item">
        <h2 class="sidebar-header" id="headerone-reversed-label">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseone-reversed-label" aria-expanded="true" aria-controls="collapseone-reversed-label">
            <div class="sidebar-button-container d-flex">
             <p class="sidebar-button-text flex-grow-1 align-self-center">可展開第一層標題</p><span class="sidebar-button-badge-round rounded-pill">12</span>
            </div>
          </button>
        </h2>
        <div id="collapseone-reversed-label" class="sidebar-collapse collapse" aria-labelledby="headerone-reversed-label" data-bs-parent="#sidebar-reversed-label">
          <div class="sidebar-second-layer" id="sidebarsecondlayer-reversed-label">
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="secondlayerheaderone-reversed-label">
                <button class="accordion-button sidebar-button sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#secondlayercollapseone-reversed-label" aria-expanded="true" aria-controls="secondlayercollapseone-reversed-label">
                  可展開第二層標題
                </button>
              </h2>
              <div id="secondlayercollapseone-reversed-label" class="sidebar-collapse collapse" aria-labelledby="secondlayerheaderone-reversed-label" data-bs-parent="#sidebarsecondlayer-reversed-label">
              </div>
            </div>
            <div class="sidebar-second-layer-item">
              <h2 class="sidebar-header" id="secondlayerheadertwo-reversed-label">
                <button class="accordion-button sidebar-button sidebar-second-layer-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#secondlayercollapsetwo" aria-expanded="true" aria-controls="secondlayercollapsetwo">
                  <div class="sidebar-button-container d-flex">
                    <p class="sidebar-button-text flex-grow-1 align-self-center">可展開第二層標題</p><span class="sidebar-button-badge-round rounded-pill">12</span>
                  </div>
                </button>
              </h2>
              <div id="secondlayercollapsetwo" class="sidebar-collapse collapse" aria-labelledby="secondlayerheadertwo-reversed-label" data-bs-parent="#sidebarsecondlayer-reversed-label">
                <div class="list-group">
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">
                    可點擊服務連結
                  </a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action active" aria-current="true">瀏覽中服務連結</a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">可點擊服務連結</a>
                  <a href="#" class="sidebar-link list-group-item list-group-item-action">可點擊服務連結</a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="sidebar-header" id="headertwo-reversed-label">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapsetwo-reversed-label" aria-expanded="true" aria-controls="collapsetwo-reversed-label">
            <div class="sidebar-button-container d-flex">
             <p class="sidebar-button-text flex-grow-1 align-self-center">可展開第一層標題</p><span class="sidebar-button-badge-round rounded-pill">12</span>
            </div>
          </button>
        </h2>
        <div id="collapsetwo-reversed-label" class="sidebar-collapse collapse" aria-labelledby="headertwo-reversed-label" data-bs-parent="#sidebar-reversed-label">
        </div>
      </div>
      <div class="accordion-item">
        <h2 class="sidebar-header" id="headerthree-reversed-label">
          <button class="accordion-button sidebar-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapsethree-reversed-label" aria-expanded="true" aria-controls="collapsethree-reversed-label">
            可展開第一層標題
          </button>
        </h2>
        <div id="collapsethree-reversed-label" class="sidebar-collapse collapse" aria-labelledby="headerthree-reversed-label" data-bs-parent="#sidebar-reversed-label">
        </div>
      </div>
    </div>
  </div>
</div>

{{< /example >}}
