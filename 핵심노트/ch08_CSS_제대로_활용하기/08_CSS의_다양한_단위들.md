# CSS의 다양한 단위들

[TOC]

CSS에는 px, rem, em, % 등 여러 단위가 있습니다. 폰트 크기 뿐만 아니라 padding, margin, width 등 다양한 속성들에 이 단위들을 사용할 수 있습니다.

이 단위들의 차이에 대해 알아봅시다.

## px

px는 절대적인 값입니다. 다른 요소의 값에 영향을 받지 않는다는 거죠.

<iframe height="265" style="width: 100%;" scrolling="no" title="080801" src="https://codepen.io/tiroring09/embed/VwvMJaV?height=265&theme-id=default&default-tab=css,result" frameborder="no" allowtransparency="true" allowfullscreen="true" loading="lazy">
  See the Pen <a href='https://codepen.io/tiroring09/pen/VwvMJaV'>080801</a> by tiroring09
  (<a href='https://codepen.io/tiroring09'>@tiroring09</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

## rem

rem 은 상대적인 값입니다. 하지만 오직 `<html>` 태그의 font-size에만 영향을 받습니다.

2rem은 `<html>` 태그의 font-size의 2배 크기입니다.

> rm: html태그의 사이즈에 대한 비율
> em: 자신의 사이즈에 대한 비율

<iframe height="265" style="width: 100%;" scrolling="no" title="080802" src="https://codepen.io/tiroring09/embed/jObGjrr?height=265&theme-id=default&default-tab=css,result" frameborder="no" allowtransparency="true" allowfullscreen="true" loading="lazy">
  See the Pen <a href='https://codepen.io/tiroring09/pen/jObGjrr'>080802</a> by tiroring09
  (<a href='https://codepen.io/tiroring09'>@tiroring09</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

## em

em도 rem과 마찬가지로 상대적인 값입니다. em은 자기 자신의 font-size를 기준으로 합니다.

2em은 자기 자신의 font-size의 2배 크기입니다. 자기 자신의 font-size를 따로 정해주지 않을 경우, 상위 요소에서 상속받은 값을 기준으로 합니다.

<iframe height="265" style="width: 100%;" scrolling="no" title="080803" src="https://codepen.io/tiroring09/embed/dyYVBXg?height=265&theme-id=default&default-tab=css,result" frameborder="no" allowtransparency="true" allowfullscreen="true" loading="lazy">
  See the Pen <a href='https://codepen.io/tiroring09/pen/dyYVBXg'>080803</a> by tiroring09
  (<a href='https://codepen.io/tiroring09'>@tiroring09</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>


만약 자기 자신에게 정해진 font-size가 있다면 그 값을 기준으로 em이 결정됩니다.

<iframe height="265" style="width: 100%;" scrolling="no" title="080804" src="https://codepen.io/tiroring09/embed/BaowgLa?height=265&theme-id=default&default-tab=css,result" frameborder="no" allowtransparency="true" allowfullscreen="true" loading="lazy">
  See the Pen <a href='https://codepen.io/tiroring09/pen/BaowgLa'>080804</a> by tiroring09
  (<a href='https://codepen.io/tiroring09'>@tiroring09</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

## 퍼센트 (%)

% 역시 상대적인 값이겠죠? %는 어느 항목에서 쓰이냐에 따라 다른 기준이 적용됩니다.

예를 들어 font-size에서 %가 쓰일 경우, 상위 요소의 font-size에 곱해주는 방식으로 계산합니다.

<p class="codepen" data-height="265" data-theme-id="default" data-default-tab="css,result" data-user="tiroring09" data-slug-hash="PoPJrWY" style="height: 265px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="080805">
  <span>See the Pen <a href="https://codepen.io/tiroring09/pen/PoPJrWY">
  080805</a> by tiroring09 (<a href="https://codepen.io/tiroring09">@tiroring09</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://static.codepen.io/assets/embed/ei.js"></script>


%가 margin이나 padding의 단위로 사용될 경우, 상위 요소의 width를 기준으로 계산됩니다.

<iframe height="265" style="width: 100%;" scrolling="no" title="080806" src="https://codepen.io/tiroring09/embed/yLYzdgM?height=265&theme-id=default&default-tab=css,result" frameborder="no" allowtransparency="true" allowfullscreen="true" loading="lazy">
  See the Pen <a href='https://codepen.io/tiroring09/pen/yLYzdgM'>080806</a> by tiroring09
  (<a href='https://codepen.io/tiroring09'>@tiroring09</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>


재미있는 점은 margin-top이나 padding-bottom 등 세로(상하) 속성를 조절할 때에도 상위 요소의 height가 아닌 width를 기준으로 계산된다는 것입니다.

<iframe height="265" style="width: 100%;" scrolling="no" title="080807" src="https://codepen.io/tiroring09/embed/abvLgpY?height=265&theme-id=default&default-tab=css,result" frameborder="no" allowtransparency="true" allowfullscreen="true" loading="lazy">
  See the Pen <a href='https://codepen.io/tiroring09/pen/abvLgpY'>080807</a> by tiroring09
  (<a href='https://codepen.io/tiroring09'>@tiroring09</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

## 참고

더 자세히 알아보고 싶으신 분들은 아래 링크를 참고해보세요: https://webdesign.tutsplus.com/ko/tutorials/comprehensive-guide-when-to-use-em-vs-rem--cms-23984