---
layout: docs
title: 可近用性 Accessibility
description: 盡可能讓更多人使用你所做出的網站。
group: overview
toc: true
---

## 規範

政府作為政府服務的提供者，每位公民皆為政府網站的使用者，因此在設計與開發網站時，遵守數位服務的無障礙規範，成為不可或缺且必要的設計流程與重要步驟。

## 概述

無障礙（Accessibility）的意涵是盡可能讓更多人使用你所做出的網站，讓無障礙的規範融入每一個數位服務使用者的行為中，使用者包含但不限於身心障礙者，例如正在走動的使用者、不擅於閱讀長篇文字者、不擅使用行動裝置者、身處網速較慢地區者等使用手機上網或其他頻寬受限的使用者，有效率地掌握網頁內容資訊。我們認為，遵照嚴謹的無障礙規範設計與增進網頁親和力，只是開始，盡可能擴大可用性，將有助於為所有人提升政府網站的品質。



## 考慮事項

以下為參照無障礙規範時，功能是否具足的自評問題：

- 使用者能只用鍵盤瀏覽您的網站嗎？

- 使用者能否使用螢幕閱讀器訪問所有頁面內容？

- 使用者能否快速理解您內容的要點？

- 使用者能否輕鬆解讀與圖形元素相關的內容？

- 使用者能否輕鬆理解並完成關鍵任務？

- 您是否在廣泛的用戶中測試您的服務？

## 原則

本規範係基於W3C的WAI 組織在2018年6月5日公佈最新版本的WCAG 2.1(Web Content Accessibility Guidelines 2.1)訂定的無障礙網頁內容標準相關規範，2002年訂定我國的「無障礙網頁開發規範」之四原則設計而成，內含：

- 「可感知」：使用者皆可收到所有網頁上呈現的資訊

- 「可操作」：使用者一定都能操作網頁頁面的任何功能
 
- 「可理解」：使用者一定要能夠明白資訊及使用者介面的操作
 
- 「穩健性」：即便科技演進網頁建置技術與時俱進，內容仍保有身障者可用輔具工具維持可讀性

以上這四原則是任何使用者想要取用網頁內容所必要的基礎。

## 可採行的方式

- 避免低色彩對比度、小型文字或是小型圖標的視覺設計
- 將鍵盤操作最佳化、可易用性提升
- 優先採用乾淨的架構的方式，並盡量將長篇幅的文字分段處理
- 避免將太多資訊擠在單一頁面，並且頁面按邏輯序列排列
- 不過度依賴顏色區別資訊，而應使用適當的文字或圖標示意，並且內容符合顏色對比要求
- 做響應式設計，確保所設計的介面在每個螢幕尺寸上皆可識、讀
- 使用機構資源，聯繫你所在機構的無障礙團隊，並與他們建立關係
- 瞭解輔助科技，訪問網絡無障礙倡議網站，瞭解人們使用輔助科技的基本管道以及殘疾人如何使用網絡
- 透過廣泛性測試，在發現各種使用上有需要改進處，可以隨時補救、更新製作

## 實際套用作業準則

### 一、為了讓使用者能更容易地看見及聽到內容、區分前景和背景，以利辨識（指引1.4)

#### 1. 文字色彩對比度

色彩不應為唯一傳達資訊的方式使用，但是足夠的色彩對比度，包含視障者或光線強烈或不足的裝置上查看資訊時，可增進對文字和圖片更容易閱讀及理解。

對比度的範圍可以從 1:1 到 21:1，其中 21 是最高級別的對比度和最佳易讀性，例如：白底黑字的比例為 21:1。

為符合檢測等級AA，確認文字(及影像文字)與文字後面的背景間：1.小型文字 (小於 18 點的標準文字，或是小於 14 點的粗體文字)， 設定至少 4.5:1 的對比度；2. 大型文字 (大於 18 點的標準文字，或是大於 14 點的粗體文字) ，設定至少 3:1 的對比度。

為符合檢測等級AAA，確認文字(及影像文字)與文字後面的背景間：1.小型文字 (小於 18 點的標準文字，或是小於 14 點的粗體文字)， 設定至少 7:1 的對比度，2. 大型文字 (大於 18 點的標準文字，或是大於 14 點的粗體文字) ，設定至少 4.5:1 的對比度。
除了符合色彩對比度的規範以外，選定一致的色彩對比度也有助於我們在選用不同的背景和文字顏色時仍然保持一致感。

（測試時可用[對比度](https://contrast-ratio.com/)計算工具）

#### 2. 視覺呈現
為符合檢測等級AAA，文字寬度不可多於80個字元或字符，文字不可全齊(左右邊界均對齊)，且段落內的行距至少要是1.5倍行高，而段落間距則至少要是1.5倍行距。文字要能夠放大至百分之兩百，並且在全螢幕視窗中閱讀時，使用者毋須水平捲動視窗即可讀。

#### 3. 非文字對比度
為符合檢測等級AA，視覺呈現與相鄰顏色的對比度至少為3:1。比如：當使用者使用到某個介面「元件」時，得以用CSS改變原來的呈現方式；當有特別顏色表示表單時，需撰寫程式用「文字提示」註記哪些地方是不同顏色文字內容，如可使用「required」。

#### 4. 文字間距
為符合檢測等級AA，透過設置以下所有內容且在不更改其他樣式屬性下，不會喪失任何內容或功能性，並且可以達到無障礙規範：
- 行高至少為字體大小的1.5倍；
- 段落間距至少是字體大小的2倍；
- 字元間距至少為字體大小的0.12倍；中文字元0.14倍。
- 字間距至少為字體大小的0.16倍。

#### 5. 驗證碼
為確保聽障者及視障者的資訊知情權，請：

- 不使用驗證碼為首要考量。
- 次之，如使用驗證碼，請同時併陳圖形與語音驗證碼，以符合不同障別者的需求。
- 第三，如提供圖形驗證碼，請以「全英」或「全數」為驗證碼，勿以「英數混合」提供之，以免同音致使造成混淆。

### 二、讓所有的功能都能透過鍵盤使用（指引2.1）


#### 1. 鍵盤
為符合檢測等級A，一個無障礙的數位系統設計，應能滿足使用者在不需操作滑鼠的情境及不額外要求時限下，仍能順利單用鍵盤完成任務，包含鍵盤使用者、用語音輸入者、用滑鼠操作螢幕小鍵盤者等，使用鍵盤應足夠對所有提供的功能與服務進行操作。

為符合檢測等級AAA，呈上，任何事件無論是鍵盤還是滑鼠的事件皆可由鍵盤來完成，不僅沒有額外的特定按鍵計時，且無任何例外情形。

#### 2. Tab 鍵 
為符合檢測等級A，Tab 鍵又稱「製表鍵」或「表格鍵」，用以將焦點推進到下一個連結、表單輸入欄位或按鈕，或者用 Tab 鍵即可將焦點移開。使用者按 Tab 鍵，能依序瀏覽所有內容，既不會困在某一個欄位中，也不會跳到其他內容。

#### 3. 方向鍵 
為符合檢測等級A，方向鍵又稱「上下左右鍵」，通常用於上下左右在選單之間移動、調整音量大小聲等。根據介面上顯示的方向，垂直移動時使用上、下鍵，水平移動時使用左、右鍵，透過方向鍵，可做下拉列表選項的操作。

#### 4. 輸入鍵 
為符合檢測等級A，按下輸入鍵時，會啟動所焦點的連結或按鈕並執行與連結或按鈕相關的動作，通常會被帶到新的頁面或送出表單。

#### 5. 空白鍵 
為符合檢測等級A，空白鍵可被用來「選取複選框」或「取消選取復選框」中的元素。

##### 6. ESC 鍵 
為符合檢測等級A，空白鍵可以關閉現有的互動視窗、選單或下拉式選單。 

### 三、讓網頁以可預期的方式來呈現及運作（指引3.2)

#### 1. 焦點與輸入
為符合檢測等級A，除非使用者在使用元件前已被告知過相關的程式行為，否則變更任何使用者介面元件的設定時，都不會自動變更脈絡。

#### 2. 一致性風格
為符合檢測等級AA，導覽與識別，在具有相同功能性的元件，要有一致性的識別。


## 進一步閱讀

### 英文

[Checklist of Checkpoints for Web Content Accessibility Guidelines 1.0](https://www.w3.org/TR/WAI-WEBCONTENT/full-checklist)<br>
[MSU Web Accessibility](https://msu.edu/webaccess)<br>
[Techniques for Web Content Accessibility Guidelines 1.0](https://www.w3.org/TR/WAI-WEBCONTENT-TECHS/)<br>
[Web Content Accessibility Guidelines 1.0](https://www.w3.org/TR/WAI-WEBCONTENT/)<br>
[Web Content Accessibility Guidelines 2.0](https://www.w3.org/TR/2001/WD-WCAG20-20010125/)<br>
[Web Site Accessibility](https://askjan.org/links/WebpgAccess.htm)

### 中文

[Dive Into Accessibility](https://dia.z6i.org/)<br>
[平等機會委員會](https://www.eoc.org.hk/en)<br>
[無障礙全球資訊網](https://www.batol.net/)<br>
[華文視障電子圖書館](http://elib.batol.net/)