---
layout: docs
title: 顏色 (Color)
group: 風格
toc: true
---

## 規範

### 色彩對比度

在替所製作的數位系統選用色彩時，我們必須符合色彩對比度 WCAG AA 等級或更高級別。以下列出幾個可以用來檢查對比度是否足夠的工具：
[Snook.ca 顏色對比檢查](https://snook.ca/technical/colour_contrast/colour.html#fg=33FF33,bg=333333)，[Webaim 顏色對比檢查器](https://webaim.org/resources/contrastchecker/)、[TPG 顏色對比分析器](https://www.tpgi.com/color-contrast-checker/)、[對比度網站-Contrast ratio](https://contrast-ratio.com) 或 [Android 無障礙掃描工具](https://support.google.com/accessibility/android/answer/6376570?hl=en-GB)。

要注意的是，字型大小也會是影響對比度的變因。舉例來說，有時雖然文字色與背景色通過上述色彩對比度檢測，但若文字的字型縮小時，雖顏色不變，可能必須得將字重加大才能通過對比度檢測。您可以使用下列工具來檢查：[Adobe 色彩對比度分析器](https://color.adobe.com/create/color-contrast-analyzer)。

## 參考顏色

我們挑選出一組顏色作為參考，以下的顏色組合已經符合色彩對比度的規定。

### 文字 (Text)

#### 預設文字色 (Primary text color)

```graphviz
digraph hierarchy {

nodesep=1.0 // increases the separation between nodes

node [color="#121212",style=filled, shape=circle] //All nodes will this shape and colour

"#121212"
}
```

#### 次要文字色 (Secondary text color)

```graphviz
digraph hierarchy {

nodesep=1.0 // increases the separation between nodes

node [color="#5D5F60",style=filled, shape=circle] //All nodes will this shape and colour

"#5D5F60"
}
```

#### 背景色 (Background color)

```graphviz
digraph hierarchy {

nodesep=1.0 // increases the separation between nodes

node [color="#FFFFFF",style=filled, shape=circle] //All nodes will this shape and colour

"#FFFFFF"
}
```

### 連結 (Link)

#### 預設 (Default)

```graphviz
digraph hierarchy {

nodesep=1.0 // increases the separation between nodes

node [color="#005AA8",style=filled, shape=circle] //All nodes will this shape and colour

"#005AA8"
}
```

#### [hover 中文] (Hover)

```graphviz
digraph hierarchy {

nodesep=1.0 // increases the separation between nodes

node [color="#003C70",style=filled, shape=circle] //All nodes will this shape and colour

"#003C70"
}
```

#### [visited 中文] (Visited)

```graphviz
digraph hierarchy {

nodesep=1.0 // increases the separation between nodes

node [color="#E57246",style=filled, shape=circle] //All nodes will this shape and colour

"#E57246"
}
```

### 邊框 (Border)

#### [預設邊框] (Default border)

```graphviz
digraph hierarchy {

nodesep=1.0 // increases the separation between nodes

node [color="#C1C2C3",style=filled, shape=circle] //All nodes will this shape and colour

"#C1C2C3"
}
```

#### 輸入欄位框 (Input border)

```graphviz
digraph hierarchy {

nodesep=1.0 // increases the separation between nodes

node [color="#121212",style=filled, shape=circle] //All nodes will this shape and colour

"#121212"
}
```

### 聚焦狀態 (Focus state)

#### 聚焦背景 (Focused background)

```graphviz
digraph hierarchy {

nodesep=1.0 // increases the separation between nodes

node [color="#F9A602",style=filled, shape=circle] //All nodes will this shape and colour

"#F9A602"
}
```

#### 聚焦文字 (Focused text)

```graphviz
digraph hierarchy {

nodesep=1.0 // increases the separation between nodes

node [color="#3B1200",style=filled, shape=circle] //All nodes will this shape and colour

"#3B1200"
}
```

### 成功狀態 (Success state)

```graphviz
digraph hierarchy {

nodesep=1.0 // increases the separation between nodes

node [color="#4BA979",style=filled, shape=circle] //All nodes will this shape and colour

"#4BA979"
}
```

### 錯誤狀態 (Error state)

```graphviz
digraph hierarchy {

nodesep=1.0 // increases the separation between nodes

node [color="#AB361D",style=filled, shape=circle] //All nodes will this shape and colour

"#AB361D"
}
```

### 品牌顏色 (Brand color)

```graphviz
digraph hierarchy {

nodesep=1.0 // increases the separation between nodes

node [color="#005AA8",style=filled, shape=circle] //All nodes will this shape and colour

"#005AA8"
}
```
