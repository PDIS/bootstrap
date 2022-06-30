---
layout: docs
title: 手風琴 Accordion
description: 手風琴是一種可以展開與隱藏更多資訊的列表。
group: components
toc: true
---

## 關於手風琴

手風琴 (accordion) 是一種可以展開與隱藏更多資訊的列表，展開後的資訊可以是純文字，也可以是更深層的手風琴 (layered accordion) 。

## 使用規範

### 何時該使用手風琴

- **切換隱藏或顯示大量文字內容。** 當列表上的說明文字多到一個量，可以使用手風琴內部分文字收納隱藏起來，讓使用者自行點擊切換顯示更多文字內容或是隱藏部分文字內容。
- **以短句標題總結大量文字內容。** 當頁面上的文字內容可以用某個短句子總結時，且使用者不一定需要這些大篇幅的文字資訊時，可以使用手風琴幫助收納資訊，讓使用者僅以短句標題先初步瀏覽總結，再自行選擇是否展開以查看更多。（列如：問答集，使用者不一定需要知道每個問題的答案，但可以透過問題本身自行選擇想要觀看某條目的答案）。

### 何時該考慮使用其他元件

- **標題過於豐富。** 當標題內容較難以文字簡單呈現時，請考慮使用其他文件，例如可以包含標題、內文、圖片、按鈕的卡片元件 (card component) 。
- **內容過於簡單。** 手風琴的互動會增加使用者的認知負荷 (cognitive load) 和互動成本 (interaction cost)，所以當內容簡短到不需要以標題做壓縮時，請考慮直接將文字排版，不需要使用手風琴收納。
- **預設使用者詳讀全文。** 當您希望使用者詳讀所有內容時，請勿假設使用者會點開所有手風琴的內容，請考慮捨棄使用手風琴而改以使用簡單乾淨的文字排版，協助使用者閱讀內容。

### 手風琴易用性

- **圖標一致性。** 手風琴上的圖標按鈕應一致，展開按鈕應選用同一種，收納按鈕也應選用同一種。
- **風格差異。** 使用者應要能夠容易辨識出手風琴展開時與收納時的風格差異。

## 元件設計

### 基本手風琴 Basic accordion

基本款的手風琴預設將內容收起。打開後有文字內容。

{{< example >}}

<div class="row d-flex justify-content-center">
  <div class="col-lg-4">
    <div class="accordion" id="accordionExample">
      <div class="accordion-item">
        <span class="accordion-header" id="headingOne">
          <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
            手風琴選單標題文字
          </button>
        </span>
        <div id="collapseOne" class="accordion-collapse collapse" aria-labelledby="headingOne" data-bs-parent="#accordionExample">
          <div class="accordion-body">
            手風琴選單第一層內容文字手風琴選單第一層內容文字手風琴選單第一層內容文字
          </div>
        </div>
      </div>
      <div class="accordion-item">
        <span class="accordion-header" id="headingTwo">
          <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
            手風琴選單標題文字
          </button>
        </span>
        <div id="collapseTwo" class="accordion-collapse collapse" aria-labelledby="headingTwo" data-bs-parent="#accordionExample">
          <div class="accordion-body">
            手風琴選單第一層內容文字手風琴選單第一層內容文字手風琴選單第一層內容文字
          </div>
        </div>
      </div>
      <div class="accordion-item">
        <span class="accordion-header" id="headingThree">
          <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
            手風琴選單標題文字
          </button>
        </span>
        <div id="collapseThree" class="accordion-collapse collapse" aria-labelledby="headingThree" data-bs-parent="#accordionExample">
          <div class="accordion-body">
            手風琴選單第一層內容文字手風琴選單第一層內容文字手風琴選單第一層內容文字
          </div>
        </div>
      </div>
        <div class="accordion-item">
        <span class="accordion-header" id="headingFour">
          <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseFour" aria-expanded="false" aria-controls="collapseFour">
            手風琴選單標題文字
          </button>
        </span>
        <div id="collapseFour" class="accordion-collapse collapse" aria-labelledby="headingFour" data-bs-parent="#accordionExample">
          <div class="accordion-body">
            手風琴選單第一層內容文字手風琴選單第一層內容文字手風琴選單第一層內容文字
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

{{</ example >}}

## 多層 Multilevel

打開有另一層可展開的內容。

{{< example >}}
<div class="row d-flex justify-content-center">
  <div class="col-lg-4">
    <div class="accordion" id="accordionExample3">
      <div class="accordion-item">
        <span class="accordion-header" id="headingOne3">
          <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne3" aria-expanded="true" aria-controls="collapseOne3">
            手風琴選單標題文字
          </button>
        </span>
        <div id="collapseOne3" class="accordion-collapse collapse" aria-labelledby="headingOne3" data-bs-parent="#accordionExample3">
          <div class="accordion-body">
            手風琴選單第一層內容文字手風琴選單第一層內容文字手風琴選單第一層內容文字
          </div>
        </div>
      </div>
      <div class="accordion-item">
        <span class="accordion-header" id="headingTwo3">
          <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo3" aria-expanded="false" aria-controls="collapseTwo3">
            手風琴選單標題文字
          </button>
        </span>
        <div id="collapseTwo3" class="accordion-collapse collapse" aria-labelledby="headingTwo3" data-bs-parent="#accordionExample3">
          <div class="accordion" id="accordionSecondLayer">
            <div class="accordion-item">
              <span class="accordion-header" id="headingSecondLayerOne">
                <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseSecondLayerOne" aria-expanded="true" aria-controls="collapseSecondLayerOne">
                  內層標題文字
                </button>
              </span>
              <div id="collapseSecondLayerOne" class="accordion-collapse collapse" aria-labelledby="headingSecondLayerOne" data-bs-parent="#accordionSecondLayer">
                <div class="accordion-body">
                  手風琴選單第二層內容文字手風琴選單第二層內容文字手風琴選單第二層內容文字
                </div>
              </div>
            </div>
            <div class="accordion-item">
              <span class="accordion-header" id="headingSecondLayerTwo">
                <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseSecondLayerTwo" aria-expanded="true" aria-controls="collapseSecondLayerTwo">
                  內層標題文字
                </button>
              </span>
              <div id="collapseSecondLayerTwo" class="accordion-collapse collapse" aria-labelledby="headingSecondLayerTwo" data-bs-parent="#accordionSecondLayer">
                <div class="accordion-body">
                  手風琴選單第二層內容文字手風琴選單第二層內容文字手風琴選單第二層內容文字
                </div>
              </div>
            </div>
            <div class="accordion-item">
              <span class="accordion-header" id="headingSecondLayerThree">
                <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseSecondLayerThree" aria-expanded="true" aria-controls="collapseSecondLayerThree">
                  內層標題文字
                </button>
              </span>
              <div id="collapseSecondLayerThree" class="accordion-collapse collapse" aria-labelledby="headingSecondLayerThree" data-bs-parent="#accordionSecondLayer">
                <div class="accordion-body">
                  手風琴選單第二層內容文字手風琴選單第二層內容文字手風琴選單第二層內容文字
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="accordion-item">
        <span class="accordion-header" id="headingThree3">
          <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree3" aria-expanded="false" aria-controls="collapseThree3">
            手風琴選單標題文字
          </button>
        </span>
        <div id="collapseThree3" class="accordion-collapse collapse" aria-labelledby="headingThree3" data-bs-parent="#accordionExample3">
          <div class="accordion-body">
          手風琴選單第一層內容文字手風琴選單第一層內容文字手風琴選單第一層內容文字
          </div>
        </div>
      </div>
        <div class="accordion-item">
        <span class="accordion-header" id="headingFour3">
          <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseFour3" aria-expanded="false" aria-controls="collapseFour3">
            手風琴選單標題文字
          </button>
        </span>
        <div id="collapseFour3" class="accordion-collapse collapse" aria-labelledby="headingFour3" data-bs-parent="#accordionExample3">
          <div class="accordion-body">
          手風琴選單第一層內容文字手風琴選單第一層內容文字手風琴選單第一層內容文字
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

{{</ example >}}

## 禁用 Disabled

將某些內容設為禁用，不可以按。

{{< example >}}

<div class="row d-flex justify-content-center">
  <div class="col-lg-4">
    <div class="accordion" id="accordionExample2">
      <div class="accordion-item">
        <span class="accordion-header" id="headingOne2">
          <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne2" aria-expanded="true" aria-controls="collapseOne2">
            手風琴選單標題文字
          </button>
        </span>
        <div id="collapseOne2" class="accordion-collapse collapse" aria-labelledby="headingOne2" data-bs-parent="#accordionExample2">
          <div class="accordion-body">
            手風琴選單第一層內容文字手風琴選單第一層內容文字手風琴選單第一層內容文字
          </div>
        </div>
      </div>
      <div class="accordion-item">
        <span class="accordion-header" id="headingTwo2">
          <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo2" aria-expanded="false" aria-controls="collapseTwo2">
            手風琴選單標題文字
          </button>
        </span>
        <div id="collapseTwo2" class="accordion-collapse collapse" aria-labelledby="headingTwo2" data-bs-parent="#accordionExample2">
          <div class="accordion-body">
            手風琴選單第一層內容文字手風琴選單第一層內容文字手風琴選單第一層內容文字
          </div>
        </div>
      </div>
      <div class="accordion-item">
        <span class="accordion-header" id="headingThree2">
          <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree2" aria-expanded="false" aria-controls="collapseThree2" disabled>
            手風琴選單標題文字
          </button>
        </span>
        <div id="collapseThree2" class="accordion-collapse collapse" aria-labelledby="headingThree2" data-bs-parent="#accordionExample2">
          <div class="accordion-body">
            手風琴選單第一層內容文字手風琴選單第一層內容文字手風琴選單第一層內容文字
          </div>
        </div>
      </div>
        <div class="accordion-item">
        <span class="accordion-header" id="headingFour2">
          <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseFour2" aria-expanded="false" aria-controls="collapseFour2" disabled>
            手風琴選單標題文字
          </button>
        </span>
        <div id="collapseFour2" class="accordion-collapse collapse" aria-labelledby="headingFour2" data-bs-parent="#accordionExample2">
          <div class="accordion-body">
            手風琴選單第一層內容文字手風琴選單第一層內容文字手風琴選單第一層內容文字
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

{{</ example >}}

## 總是開啟 Always open

在打開選單中另一個選項時，保持開啟狀態。

{{< example >}}

<div class="row d-flex justify-content-center">
  <div class="col-lg-4">
    <div class="accordion" id="accordionExample4">
      <div class="accordion-item">
        <span class="accordion-header" id="headingOne4">
          <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne4" aria-expanded="true" aria-controls="collapseOne4">
            手風琴選單標題文字
          </button>
        </span>
        <div id="collapseOne4" class="accordion-collapse collapse" aria-labelledby="headingOne4">
          <div class="accordion-body">
            手風琴選單第一層內容文字手風琴選單第一層內容文字手風琴選單第一層內容文字
          </div>
        </div>
      </div>
      <div class="accordion-item">
        <span class="accordion-header" id="headingTwo4">
          <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo4" aria-expanded="false" aria-controls="collapseTwo4">
            手風琴選單標題文字
          </button>
        </span>
        <div id="collapseTwo4" class="accordion-collapse collapse show" aria-labelledby="headingTwo4">
          <div class="accordion-body">
            手風琴選單第一層內容文字手風琴選單第一層內容文字手風琴選單第一層內容文字
          </div>
        </div>
      </div>
      <div class="accordion-item">
        <span class="accordion-header" id="headingThree4">
          <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree4" aria-expanded="false" aria-controls="collapseThree4">
            手風琴選單標題文字
          </button>
        </span>
        <div id="collapseThree4" class="accordion-collapse collapse" aria-labelledby="headingThree4">
          <div class="accordion-body">
            手風琴選單第一層內容文字手風琴選單第一層內容文字手風琴選單第一層內容文字
          </div>
        </div>
      </div>
        <div class="accordion-item">
        <span class="accordion-header" id="headingFour4">
          <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseFour4" aria-expanded="false" aria-controls="collapseFour4">
            手風琴選單標題文字
          </button>
        </span>
        <div id="collapseFour4" class="accordion-collapse collapse" aria-labelledby="headingFour4">
          <div class="accordion-body">
            手風琴選單第一層內容文字手風琴選單第一層內容文字手風琴選單第一層內容文字
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="col-lg-4">
    <div class="accordion" id="accordionExample5">
      <div class="accordion-item">
        <span class="accordion-header" id="headingOne5">
          <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne5" aria-expanded="true" aria-controls="collapseOne5">
            手風琴選單標題文字
          </button>
        </span>
        <div id="collapseOne5" class="accordion-collapse collapse" aria-labelledby="headingOne5">
          <div class="accordion-body">
            手風琴選單第一層內容文字手風琴選單第一層內容文字手風琴選單第一層內容文字
          </div>
        </div>
      </div>
      <div class="accordion-item">
        <span class="accordion-header" id="headingTwo5">
          <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo5" aria-expanded="false" aria-controls="collapseTwo5">
            手風琴選單標題文字
          </button>
        </span>
        <div id="collapseTwo5" class="accordion-collapse collapse show" aria-labelledby="headingTwo5" data-bs-parent="#accordionExample5">
          <div class="accordion" id="accordionSecondLayer">
            <div class="accordion-item">
              <span class="accordion-header" id="headingSecondLayerOne">
                <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseSecondLayerOne" aria-expanded="true" aria-controls="collapseSecondLayerOne">
                  內層標題文字
                </button>
              </span>
              <div id="collapseSecondLayerOne" class="accordion-collapse collapse show" aria-labelledby="headingSecondLayerOne">
                <div class="accordion-body">
                  手風琴選單第二層內容文字手風琴選單第二層內容文字手風琴選單第二層內容文字
                </div>
              </div>
            </div>
            <div class="accordion-item">
              <span class="accordion-header" id="headingSecondLayerTwo">
                <button class="accordion-button accordion-button-chevron collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseSecondLayerTwo" aria-expanded="true" aria-controls="collapseSecondLayerTwo">
                  內層標題文字
                </button>
              </span>
              <div id="collapseSecondLayerTwo" class="accordion-collapse collapse" aria-labelledby="headingSecondLayerTwo">
                <div class="accordion-body">
                  手風琴選單第二層內容文字手風琴選單第二層內容文字手風琴選單第二層內容文字
                </div>
              </div>
            </div>
            <div class="accordion-item">
              <span class="accordion-header" id="headingSecondLayerThree">
                <button class="accordion-button accordion-button-chevron collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseSecondLayerThree" aria-expanded="true" aria-controls="collapseSecondLayerThree">
                  內層標題文字
                </button>
              </span>
              <div id="collapseSecondLayerThree" class="accordion-collapse collapse" aria-labelledby="headingSecondLayerThree">
                <div class="accordion-body">
                  手風琴選單第二層內容文字手風琴選單第二層內容文字手風琴選單第二層內容文字
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="accordion-item">
        <span class="accordion-header" id="headingThree5">
          <button class="accordion-button accordion-button-chevron collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree5" aria-expanded="false" aria-controls="collapseThree5">
            手風琴選單標題文字
          </button>
        </span>
        <div id="collapseThree5" class="accordion-collapse collapse" aria-labelledby="headingThree5">
          <div class="accordion-body">
          手風琴選單第一層內容文字手風琴選單第一層內容文字手風琴選單第一層內容文字
          </div>
        </div>
      </div>
        <div class="accordion-item">
        <span class="accordion-header" id="headingFour5">
          <button class="accordion-button accordion-button-chevron collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseFour5" aria-expanded="false" aria-controls="collapseFour5">
            手風琴選單標題文字
          </button>
        </span>
        <div id="collapseFour5" class="accordion-collapse collapse" aria-labelledby="headingFour5">
          <div class="accordion-body">
          手風琴選單第一層內容文字手風琴選單第一層內容文字手風琴選單第一層內容文字
          </div>
        </div>
      </div>
    </div>
  </div>
</div>

{{</ example >}}