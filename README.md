# 📦 @kwange/textexpander

[![License](https://img.shields.io/npm/l/oclif.svg)](https://github.com/oclif/oclif/blob/main/package.json)
<br><br>
Text expander preview.
<br>
![avatar](https://github.com/skayi/textexpander/blob/main/textexpander.gif)

<br />

# 🗒 Description

- This is a pure CSS "Web Components" that automatically displays ellipsis and an expand button when text overflows.
- 这是一个文本溢出时自动展示省略号以及展开按钮的纯属 CSS 组件 —— Web Components。 通过 width 属性可控制整体宽度，省略时继承父级宽度。line-height 属性控制文本行高，默认值为 22px。line-clamp 属性用来控制文本换行数的最大值，默认值为 1。想默认展开显示全部内容，可设置 expanded="true"。

<br />
`Chrome: 105+` `Edge: 105+` `Firefox: 110+`

<br />

# ✨ Features

1、Automatically omit text based on width, and display expand button when text overflows
2、Custom expand and collapse button
3、Custom text width, line height and line clamp
4、Custom text default expansion

<br />

# 🔨 Installation

```
npm install @kwange/textexpander --save
or
yarn add @kwange/textexpander
```

<br/>

# 🏗 Usage

import :

```javascript
JavaScript: import '@kwange/textexpander' or require('@kwange/textexpander')
DOM: <text-expander></text-expander>
```

default :

```javascript
<text-expander>your text</text-expander>
```

custom :

```javascript
<text-expander
  width="200px"
  line-height="22px"
  line-clamp="2"
  expanded="true|false"
>
  This is a pure CSS "Web Components" that automatically displays ellipsis and
  an expand button when text overflows.
  <span slot="expand" style="color: blue">
    Expand
  </span>
  <span slot="collapse" style="color: blue">
    Collapse
  </span>
</text-expander>
```
