# display

[TOC]

HTML 요소의 레이아웃을 결정하는 가장 중요한 속성 중 하나는 display입니다.

## display의 종류

모든 요소는 딱 한 개의 display 값을 갖고 있습니다. 가질 수 있는 display의 종류는

- inline
- block
- inline-block
- flex
- list-item
- none

등 여러 가지가 있는데, 대부분의 요소들은 inline과 block 중 한 가지입니다.

## inline display

inline 요소들은 다른 요소들과 같은 줄에 머무르려고 하는 성향과, 필요한 만큼의 가로 길이만 차지하는 성향이 있습니다.

다음 요소들은 기본 display 값이 inline입니다.

- `<span>`
- `<a>`
- `<b>`
- `<i>`
- `<img>`
- `<button>`

<iframe height="265" style="width: 100%;" scrolling="no" title="090201" src="https://codepen.io/tiroring09/embed/dyYVBBx?height=265&theme-id=default&default-tab=css,result" frameborder="no" allowtransparency="true" allowfullscreen="true" loading="lazy">
  See the Pen <a href='https://codepen.io/tiroring09/pen/dyYVBBx'>090201</a> by tiroring09
  (<a href='https://codepen.io/tiroring09'>@tiroring09</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

`<i>` 태그는 기본적으로 inline이기 때문에 앞, 뒤의 텍스트와 같은 줄에 머무르고 있고, 가로 길이는 필요한 만큼만 차지하고 있습니다.

## block display

block 요소들은 다른 요소들과 독단적인 줄에 가려고 하는 성향과, 최대한 많은 가로 길이를 차지하는 성향이 있습니다.

다음 요소들은 기본 display 값이 block입니다.

- `<div>`
- `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>`, `<h6>`
- `<p>`
- `<nav>`
- `<ul>`
- `<li>`

<iframe height="265" style="width: 100%;" scrolling="no" title="090202" src="https://codepen.io/tiroring09/embed/BaowgXQ?height=265&theme-id=default&default-tab=css,result" frameborder="no" allowtransparency="true" allowfullscreen="true" loading="lazy">
  See the Pen <a href='https://codepen.io/tiroring09/pen/BaowgXQ'>090202</a> by tiroring09
  (<a href='https://codepen.io/tiroring09'>@tiroring09</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

`<div>` 태그는 기본적으로 block이기 때문에 새로운 줄에 가버립니다. 그리고 가로 길이는 최대한 많이, 100%를 차지하고 있죠?

## display 바꾸기

모든 요소는 기본적으로 정해진 display 값이 있는데요. CSS를 통해서 이를 바꿀 수 있습니다!

### inline 요소를 block으로 바꾸기

<iframe height="265" style="width: 100%;" scrolling="no" title="090203" src="https://codepen.io/tiroring09/embed/JjYrQgz?height=265&theme-id=default&default-tab=css,result" frameborder="no" allowtransparency="true" allowfullscreen="true" loading="lazy">
  See the Pen <a href='https://codepen.io/tiroring09/pen/JjYrQgz'>090203</a> by tiroring09
  (<a href='https://codepen.io/tiroring09'>@tiroring09</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

### block 요소를 inline으로 바꾸기

<iframe height="265" style="width: 100%;" scrolling="no" title="090204" src="https://codepen.io/tiroring09/embed/gOaGVYr?height=265&theme-id=default&default-tab=css,result" frameborder="no" allowtransparency="true" allowfullscreen="true" loading="lazy">
  See the Pen <a href='https://codepen.io/tiroring09/pen/gOaGVYr'>090204</a> by tiroring09
  (<a href='https://codepen.io/tiroring09'>@tiroring09</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>