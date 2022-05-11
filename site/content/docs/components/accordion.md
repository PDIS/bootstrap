---
layout: docs
title: 手風琴 (Accordion)
description: 手風琴是一種可以展開與隱藏更多資訊的列表。
group: components
toc: true
---

{{< example >}}

<div class="row">
<div class="col-md-4">
<div class="accordion" id="accordionExample">
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingOne">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
        手風琴選單標題文字
      </button>
    </h2>
    <div id="collapseOne" class="accordion-collapse collapse" aria-labelledby="headingOne" data-bs-parent="#accordionExample">
      <div class="accordion-body">
        手風琴選單第一層內容文字手風琴選單第一層內容文字手風琴選單第一層內容文字
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingTwo">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
        手風琴選單標題文字
      </button>
    </h2>
    <div id="collapseTwo" class="accordion-collapse collapse" aria-labelledby="headingTwo" data-bs-parent="#accordionExample">
      <div class="accordion-body">
        手風琴選單第一層內容文字手風琴選單第一層內容文字手風琴選單第一層內容文字
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingThree">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
        手風琴選單標題文字
      </button>
    </h2>
    <div id="collapseThree" class="accordion-collapse collapse" aria-labelledby="headingThree" data-bs-parent="#accordionExample">
      <div class="accordion-body">
        手風琴選單第一層內容文字手風琴選單第一層內容文字手風琴選單第一層內容文字
      </div>
    </div>
  </div>
   <div class="accordion-item">
    <h2 class="accordion-header" id="headingFour">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseFour" aria-expanded="false" aria-controls="collapseFour">
        手風琴選單標題文字
      </button>
    </h2>
    <div id="collapseFour" class="accordion-collapse collapse" aria-labelledby="headingFour" data-bs-parent="#accordionExample">
      <div class="accordion-body">
        手風琴選單第一層內容文字手風琴選單第一層內容文字手風琴選單第一層內容文字
      </div>
    </div>
  </div>
</div>
</div>
<div class="col-md-4">
<div class="accordion" id="accordionExample3">
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingOne3">
      <button class="accordion-button accordion-button-chevron collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne3" aria-expanded="true" aria-controls="collapseOne3">
        有參加農保，以後可以領老農津貼嗎？要怎麼申請？每個月可以領多少錢？
      </button>
    </h2>
    <div id="collapseOne3" class="accordion-collapse collapse" aria-labelledby="headingOne3" data-bs-parent="#accordionExample3">
      <div class="accordion-body">
        <p>ㄧ、您如果符合下列各項申領條件就可以領取老農津貼：</p>
        <ol>
          <li>年滿65歲國民，在國內設有戶籍，且於最近3年內每年居住超過183天。</li>
          <li>申領時參加農保且年資合計15年以上者，可領取全額津貼新台幣(下同) 7,550元；103年7月17日(含當日)以前已參加農保，且持續加保，於申領時加保年資合計6個月以上未滿15年者，可領取半額津貼3,775元。</li>
          <li>申領老農津貼之同一期間未領取政府發放之生活補助或津貼。</li>
          <li>未領取社會保險老年給付，或已領取社會保險老年給付者，於87年11月12日以前已參加農保且加保年資未中斷。</li>
          <li>自102年1月1日起，始申請領取老農津貼之老年農民，財稅機關提供中央主管機關公告年度之農業所得以外之個人綜合所得稅各類所得總額合計未達50萬元，且個人所有之土地及房屋價值經扣除農業用地、「尚未徵收及補償之公共設施保留地」、農舍、「無農舍且實際居住之唯一房屋及土地(最多以扣除400萬元為限)」、「未產生經濟效益之原住民保留地」及「未產生經濟效益具公用地役關係之現有道路」後合計未達500萬元者，得領取老農津貼。</li>
        </ol>
        <p>二、如果您符合以上申領條件，請於年滿65歲當月主動檢附國民身分證、農會信用部或郵局存簿及印章，至您所屬的基層農會提出申請。</p>
        <p>三、經審查合格，每個月可以領取7,550元或3,775元。 </p>
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingTwo3">
      <button class="accordion-button accordion-button-chevron collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo3" aria-expanded="false" aria-controls="collapseTwo3">
        請領要件
      </button>
    </h2>
    <div id="collapseTwo3" class="accordion-collapse collapse" aria-labelledby="headingTwo3" data-bs-parent="#accordionExample3">
      <div class="accordion" id="accordionSecondLayer">
        <div class="accordion-item">
          <h2 class="accordion-header" id="headingSecondLayerOne">
            <button class="accordion-button accordion-button-chevron collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseSecondLayerOne" aria-expanded="true" aria-controls="collapseSecondLayerOne">
              勞保生育給付
            </button>
          </h2>
          <div id="collapseSecondLayerOne" class="accordion-collapse collapse" aria-labelledby="headingSecondLayerOne" data-bs-parent="#accordionSecondLayer">
            <div class="accordion-body">
              <p>按被保險人分娩或 ...</p>
            </div>
          </div>
        </div>
        <div class="accordion-item">
          <h2 class="accordion-header" id="headingSecondLayerTwo">
            <button class="accordion-button accordion-button-chevron collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseSecondLayerTwo" aria-expanded="true" aria-controls="collapseSecondLayerTwo">
              國保生育給付
            </button>
          </h2>
          <div id="collapseSecondLayerTwo" class="accordion-collapse collapse" aria-labelledby="headingSecondLayerTwo" data-bs-parent="#accordionSecondLayer">
            <div class="accordion-body">
              <p>按被保險人分娩或 ...</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingThree3">
      <button class="accordion-button accordion-button-chevron collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree3" aria-expanded="false" aria-controls="collapseThree3">
        Household Registration Act 戶籍法英譯本
      </button>
    </h2>
    <div id="collapseThree3" class="accordion-collapse collapse" aria-labelledby="headingThree3" data-bs-parent="#accordionExample3">
      <div class="accordion-body">
      </div>
    </div>
  </div>
   <div class="accordion-item">
    <h2 class="accordion-header" id="headingFour3">
      <button class="accordion-button accordion-button-chevron collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseFour3" aria-expanded="false" aria-controls="collapseFour3">
        戶籍法施行細則（104.07.10 修正）
      </button>
    </h2>
    <div id="collapseFour3" class="accordion-collapse collapse" aria-labelledby="headingFour3" data-bs-parent="#accordionExample3">
      <div class="accordion-body">
      </div>
    </div>
  </div>
</div>
</div>
</div>

{{</ example >}}

### 關於手風琴元件

手風琴 (accordion) 是一種可以展開與隱藏更多資訊的列表，展開後的資訊可以是純文字、另一頁面、也可以是更深層的手風琴 (layered accordion) 。

### 使用規範

#### 何時該使用手風琴

- **切換隱藏或顯示大量文字內容。** 當列表上的說明文字多到一個量，可以使用手風琴內部分文字收納隱藏起來，讓使用者自行點擊切換顯示更多文字內容或是隱藏部分文字內容。
- **以短句標題總結大量文字內容。** 當頁面上的文字內容可以用某個短句子總結時，且使用者不一定需要這些大篇幅的文字資訊時，可以使用手風琴幫助收納資訊，讓使用者僅以短句標題先初步瀏覽總結，再自行選擇是否展開以查看更多。（列如：問答集，使用者不一定需要知道每個問題的答案，但可以透過問題本身自行選擇想要觀看某條目的答案）。

#### 何時該考慮使用其他元件

- **標題過於豐富。** 當標題內容較難以文字簡單呈現時，請考慮使用其他文件，例如可以包含標題、內文、圖片、按鈕的卡片元件 (card component) 。
- **內容過於簡單。** 手風琴的互動會增加使用者的認知負荷 (cognitive load) 和互動成本 (interaction cost)，所以當內容簡短到不需要以標題做壓縮時，請考慮直接將文字排版，不需要使用手風琴收納。
- **預設使用者詳讀全文。** 當您希望使用者詳讀所有內容時，請勿假設使用者會點開所有手風琴的內容，請考慮捨棄使用手風琴而改以使用簡單乾淨的文字排版，協助使用者閱讀內容。

#### 手風琴易用性

- **圖標一致性。** 手風琴上的圖標按鈕應一致，展開按鈕應選用同一種，收納按鈕也應選用同一種。
- **風格差異。** 使用者應要能夠容易辨識出手風琴展開時與收納時的風格差異。

### 設計元件

#### 基本款手風琴 Basic accordion

基本款手風琴包含標題與可以點擊的展開按鈕 (+) ，展開後該按鈕則會被替換回另一個可以點擊的收納按鈕 (-) 。除了預設的正負圖標以外，您也可以使用展開與收納按鈕也可以選擇箭頭圖標。展開後的列表樣式與展開前的樣式應有差距，讓使用者可以迅速的辨認出展開或未展開狀態。

<!-- {{< example >}}

<div class="accordion" id="accordionExample">
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingOne">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
        有參加農保，以後可以領老農津貼嗎？要怎麼申請？每個月可以領多少錢？
      </button>
    </h2>
    <div id="collapseOne" class="accordion-collapse collapse" aria-labelledby="headingOne" data-bs-parent="#accordionExample">
      <div class="accordion-body">
        <p>ㄧ、您如果符合下列各項申領條件就可以領取老農津貼：</p>
        <ol>
          <li>年滿65歲國民，在國內設有戶籍，且於最近3年內每年居住超過183天。</li>
          <li>申領時參加農保且年資合計15年以上者，可領取全額津貼新台幣(下同) 7,550元；103年7月17日(含當日)以前已參加農保，且持續加保，於申領時加保年資合計6個月以上未滿15年者，可領取半額津貼3,775元。</li>
          <li>申領老農津貼之同一期間未領取政府發放之生活補助或津貼。</li>
          <li>未領取社會保險老年給付，或已領取社會保險老年給付者，於87年11月12日以前已參加農保且加保年資未中斷。</li>
          <li>自102年1月1日起，始申請領取老農津貼之老年農民，財稅機關提供中央主管機關公告年度之農業所得以外之個人綜合所得稅各類所得總額合計未達50萬元，且個人所有之土地及房屋價值經扣除農業用地、「尚未徵收及補償之公共設施保留地」、農舍、「無農舍且實際居住之唯一房屋及土地(最多以扣除400萬元為限)」、「未產生經濟效益之原住民保留地」及「未產生經濟效益具公用地役關係之現有道路」後合計未達500萬元者，得領取老農津貼。</li>
        </ol>
        <p>二、如果您符合以上申領條件，請於年滿65歲當月主動檢附國民身分證、農會信用部或郵局存簿及印章，至您所屬的基層農會提出申請。</p>
        <p>三、經審查合格，每個月可以領取7,550元或3,775元。 </p>
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingTwo">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
        請領要件
      </button>
    </h2>
    <div id="collapseTwo" class="accordion-collapse collapse" aria-labelledby="headingTwo" data-bs-parent="#accordionExample">
      <div class="accordion-body">
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingThree">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
        Household Registration Act 戶籍法英譯本
      </button>
    </h2>
    <div id="collapseThree" class="accordion-collapse collapse" aria-labelledby="headingThree" data-bs-parent="#accordionExample">
      <div class="accordion-body">
      </div>
    </div>
  </div>
   <div class="accordion-item">
    <h2 class="accordion-header" id="headingFour">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseFour" aria-expanded="false" aria-controls="collapseFour">
        戶籍法施行細則（104.07.10 修正）
      </button>
    </h2>
    <div id="collapseFour" class="accordion-collapse collapse" aria-labelledby="headingFour" data-bs-parent="#accordionExample">
      <div class="accordion-body">
      </div>
    </div>
  </div>
</div>
<br />
<div class="accordion" id="accordionExample2">
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingOne2">
      <button class="accordion-button accordion-button-chevron collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne2" aria-expanded="true" aria-controls="collapseOne2">
        有參加農保，以後可以領老農津貼嗎？要怎麼申請？每個月可以領多少錢？
      </button>
    </h2>
    <div id="collapseOne2" class="accordion-collapse collapse" aria-labelledby="headingOne2" data-bs-parent="#accordionExample2">
      <div class="accordion-body">
        <p>ㄧ、您如果符合下列各項申領條件就可以領取老農津貼：</p>
        <ol>
          <li>年滿65歲國民，在國內設有戶籍，且於最近3年內每年居住超過183天。</li>
          <li>申領時參加農保且年資合計15年以上者，可領取全額津貼新台幣(下同) 7,550元；103年7月17日(含當日)以前已參加農保，且持續加保，於申領時加保年資合計6個月以上未滿15年者，可領取半額津貼3,775元。</li>
          <li>申領老農津貼之同一期間未領取政府發放之生活補助或津貼。</li>
          <li>未領取社會保險老年給付，或已領取社會保險老年給付者，於87年11月12日以前已參加農保且加保年資未中斷。</li>
          <li>自102年1月1日起，始申請領取老農津貼之老年農民，財稅機關提供中央主管機關公告年度之農業所得以外之個人綜合所得稅各類所得總額合計未達50萬元，且個人所有之土地及房屋價值經扣除農業用地、「尚未徵收及補償之公共設施保留地」、農舍、「無農舍且實際居住之唯一房屋及土地(最多以扣除400萬元為限)」、「未產生經濟效益之原住民保留地」及「未產生經濟效益具公用地役關係之現有道路」後合計未達500萬元者，得領取老農津貼。</li>
        </ol>
        <p>二、如果您符合以上申領條件，請於年滿65歲當月主動檢附國民身分證、農會信用部或郵局存簿及印章，至您所屬的基層農會提出申請。</p>
        <p>三、經審查合格，每個月可以領取7,550元或3,775元。 </p>
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingTwo2">
      <button class="accordion-button accordion-button-chevron collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo2" aria-expanded="false" aria-controls="collapseTwo2">
        請領要件
      </button>
    </h2>
    <div id="collapseTwo2" class="accordion-collapse collapse" aria-labelledby="headingTwo2" data-bs-parent="#accordionExample2">
      <div class="accordion-body">
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingThree2">
      <button class="accordion-button accordion-button-chevron collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree2" aria-expanded="false" aria-controls="collapseThree2">
        Household Registration Act 戶籍法英譯本
      </button>
    </h2>
    <div id="collapseThree2" class="accordion-collapse collapse" aria-labelledby="headingThree2" data-bs-parent="#accordionExample2">
      <div class="accordion-body">
      </div>
    </div>
  </div>
   <div class="accordion-item">
    <h2 class="accordion-header" id="headingFour2">
      <button class="accordion-button accordion-button-chevron collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseFour2" aria-expanded="false" aria-controls="collapseFour2">
        戶籍法施行細則（104.07.10 修正）
      </button>
    </h2>
    <div id="collapseFour2" class="accordion-collapse collapse" aria-labelledby="headingFour2" data-bs-parent="#accordionExample2">
      <div class="accordion-body">
      </div>
    </div>
  </div>
</div>

{{</ example >}} -->

#### 多層手風琴 Layered accordion

有的時候手風琴裡面還有一層手風琴，強烈建議不同層的手風情使用不同的圖標按鈕 (icon button) 與樣式以利區分。

<!-- {{< example >}}

<div class="accordion" id="accordionExample3">
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingOne3">
      <button class="accordion-button accordion-button-chevron collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne3" aria-expanded="true" aria-controls="collapseOne3">
        有參加農保，以後可以領老農津貼嗎？要怎麼申請？每個月可以領多少錢？
      </button>
    </h2>
    <div id="collapseOne3" class="accordion-collapse collapse" aria-labelledby="headingOne3" data-bs-parent="#accordionExample3">
      <div class="accordion-body">
        <p>ㄧ、您如果符合下列各項申領條件就可以領取老農津貼：</p>
        <ol>
          <li>年滿65歲國民，在國內設有戶籍，且於最近3年內每年居住超過183天。</li>
          <li>申領時參加農保且年資合計15年以上者，可領取全額津貼新台幣(下同) 7,550元；103年7月17日(含當日)以前已參加農保，且持續加保，於申領時加保年資合計6個月以上未滿15年者，可領取半額津貼3,775元。</li>
          <li>申領老農津貼之同一期間未領取政府發放之生活補助或津貼。</li>
          <li>未領取社會保險老年給付，或已領取社會保險老年給付者，於87年11月12日以前已參加農保且加保年資未中斷。</li>
          <li>自102年1月1日起，始申請領取老農津貼之老年農民，財稅機關提供中央主管機關公告年度之農業所得以外之個人綜合所得稅各類所得總額合計未達50萬元，且個人所有之土地及房屋價值經扣除農業用地、「尚未徵收及補償之公共設施保留地」、農舍、「無農舍且實際居住之唯一房屋及土地(最多以扣除400萬元為限)」、「未產生經濟效益之原住民保留地」及「未產生經濟效益具公用地役關係之現有道路」後合計未達500萬元者，得領取老農津貼。</li>
        </ol>
        <p>二、如果您符合以上申領條件，請於年滿65歲當月主動檢附國民身分證、農會信用部或郵局存簿及印章，至您所屬的基層農會提出申請。</p>
        <p>三、經審查合格，每個月可以領取7,550元或3,775元。 </p>
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingTwo3">
      <button class="accordion-button accordion-button-chevron collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo3" aria-expanded="false" aria-controls="collapseTwo3">
        請領要件
      </button>
    </h2>
    <div id="collapseTwo3" class="accordion-collapse collapse" aria-labelledby="headingTwo3" data-bs-parent="#accordionExample3">
      <div class="accordion" id="accordionSecondLayer">
        <div class="accordion-item">
          <h2 class="accordion-header" id="headingSecondLayerOne">
            <button class="accordion-button accordion-button-chevron collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseSecondLayerOne" aria-expanded="true" aria-controls="collapseSecondLayerOne">
              勞保生育給付
            </button>
          </h2>
          <div id="collapseSecondLayerOne" class="accordion-collapse collapse" aria-labelledby="headingSecondLayerOne" data-bs-parent="#accordionSecondLayer">
            <div class="accordion-body">
              <p>按被保險人分娩或 ...</p>
            </div>
          </div>
        </div>
        <div class="accordion-item">
          <h2 class="accordion-header" id="headingSecondLayerTwo">
            <button class="accordion-button accordion-button-chevron collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseSecondLayerTwo" aria-expanded="true" aria-controls="collapseSecondLayerTwo">
              國保生育給付
            </button>
          </h2>
          <div id="collapseSecondLayerTwo" class="accordion-collapse collapse" aria-labelledby="headingSecondLayerTwo" data-bs-parent="#accordionSecondLayer">
            <div class="accordion-body">
              <p>按被保險人分娩或 ...</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingThree3">
      <button class="accordion-button accordion-button-chevron collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree3" aria-expanded="false" aria-controls="collapseThree3">
        Household Registration Act 戶籍法英譯本
      </button>
    </h2>
    <div id="collapseThree3" class="accordion-collapse collapse" aria-labelledby="headingThree3" data-bs-parent="#accordionExample3">
      <div class="accordion-body">
      </div>
    </div>
  </div>
   <div class="accordion-item">
    <h2 class="accordion-header" id="headingFour3">
      <button class="accordion-button accordion-button-chevron collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseFour3" aria-expanded="false" aria-controls="collapseFour3">
        戶籍法施行細則（104.07.10 修正）
      </button>
    </h2>
    <div id="collapseFour3" class="accordion-collapse collapse" aria-labelledby="headingFour3" data-bs-parent="#accordionExample3">
      <div class="accordion-body">
      </div>
    </div>
  </div>
</div>
<br />
<div class="accordion" id="accordionExample4">
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingOne4">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne4" aria-expanded="true" aria-controls="collapseOne4">
        有參加農保，以後可以領老農津貼嗎？要怎麼申請？每個月可以領多少錢？
      </button>
    </h2>
    <div id="collapseOne4" class="accordion-collapse collapse" aria-labelledby="headingOne4" data-bs-parent="#accordionExample4">
      <div class="accordion-body">
        <p>ㄧ、您如果符合下列各項申領條件就可以領取老農津貼：</p>
        <ol>
          <li>年滿65歲國民，在國內設有戶籍，且於最近3年內每年居住超過183天。</li>
          <li>申領時參加農保且年資合計15年以上者，可領取全額津貼新台幣(下同) 7,550元；103年7月17日(含當日)以前已參加農保，且持續加保，於申領時加保年資合計6個月以上未滿15年者，可領取半額津貼3,775元。</li>
          <li>申領老農津貼之同一期間未領取政府發放之生活補助或津貼。</li>
          <li>未領取社會保險老年給付，或已領取社會保險老年給付者，於87年11月12日以前已參加農保且加保年資未中斷。</li>
          <li>自102年1月1日起，始申請領取老農津貼之老年農民，財稅機關提供中央主管機關公告年度之農業所得以外之個人綜合所得稅各類所得總額合計未達50萬元，且個人所有之土地及房屋價值經扣除農業用地、「尚未徵收及補償之公共設施保留地」、農舍、「無農舍且實際居住之唯一房屋及土地(最多以扣除400萬元為限)」、「未產生經濟效益之原住民保留地」及「未產生經濟效益具公用地役關係之現有道路」後合計未達500萬元者，得領取老農津貼。</li>
        </ol>
        <p>二、如果您符合以上申領條件，請於年滿65歲當月主動檢附國民身分證、農會信用部或郵局存簿及印章，至您所屬的基層農會提出申請。</p>
        <p>三、經審查合格，每個月可以領取7,550元或3,775元。 </p>
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingTwo4">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo4" aria-expanded="false" aria-controls="collapseTwo4">
        請領要件
      </button>
    </h2>
    <div id="collapseTwo4" class="accordion-collapse collapse" aria-labelledby="headingTwo4" data-bs-parent="#accordionExample4">
      <div class="accordion second-layer" id="accordionSecondLayer2">
        <div class="accordion-item">
          <h2 class="accordion-header" id="headingSecondLayerOne2">
            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseSecondLayerOne2" aria-expanded="true" aria-controls="collapseSecondLayerOne2">
              勞保生育給付
            </button>
          </h2>
          <div id="collapseSecondLayerOne2" class="accordion-collapse collapse" aria-labelledby="headingSecondLayerOne2" data-bs-parent="#accordionSecondLayer2">
            <div class="accordion-body">
              <p>按被保險人分娩或 ...</p>
            </div>
          </div>
        </div>
        <div class="accordion-item">
          <h2 class="accordion-header" id="headingSecondLayerTwo2">
            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseSecondLayerTwo2" aria-expanded="true" aria-controls="collapseSecondLayerTwo2">
              國保生育給付
            </button>
          </h2>
          <div id="collapseSecondLayerTwo2" class="accordion-collapse collapse" aria-labelledby="headingSecondLayerTw2o" data-bs-parent="#accordionSecondLayer2">
            <div class="accordion-body">
              <p>按被保險人分娩或 ...</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <div class="accordion-item">
    <h2 class="accordion-header" id="headingThree4">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree4" aria-expanded="false" aria-controls="collapseThree4">
        Household Registration Act 戶籍法英譯本
      </button>
    </h2>
    <div id="collapseThree4" class="accordion-collapse collapse" aria-labelledby="headingThree4" data-bs-parent="#accordionExample4">
      <div class="accordion-body">
      </div>
    </div>
  </div>
   <div class="accordion-item">
    <h2 class="accordion-header" id="headingFour4">
      <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseFour4" aria-expanded="false" aria-controls="collapseFour4">
        戶籍法施行細則（104.07.10 修正）
      </button>
    </h2>
    <div id="collapseFour4" class="accordion-collapse collapse" aria-labelledby="headingFour4" data-bs-parent="#accordionExample4">
      <div class="accordion-body">
      </div>
    </div>
  </div>
</div>

{{</ example >}}
 -->