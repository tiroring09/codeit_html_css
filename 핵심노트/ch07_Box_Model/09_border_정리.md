# border 정리

[TOC]

다른 속성들과 마찬가지로, 테두리를 설정해주는 방법도 다양합니다.

## 한 줄에 끝내기

가장 일반적인 방법은 border 속성으로 한 줄에 다 쓰는 것입니다. 이 방식을 사용하면 위, 아래, 왼쪽, 오른쪽 모두 같은 테두리가 생깁니다. 값을 쓰는 순서는 굵기, 스타일(실선, 점선 등), 색입니다.

<iframe height="265" style="width: 100%;" scrolling="no" title="070901" src="https://codepen.io/tiroring09/embed/MWaEzbm?height=265&theme-id=light&default-tab=css,result" frameborder="no" allowtransparency="true" allowfullscreen="true" loading="lazy">
  See the Pen <a href='https://codepen.io/tiroring09/pen/MWaEzbm'>070901</a> by tiroring09
  (<a href='https://codepen.io/tiroring09'>@tiroring09</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

## 명확하게 나누기

다른 방법은 border-style, border-color, border-width 속성을 써서 테두리의 스타일을 하나씩 지정해주는 것입니다.

<iframe height="265" style="width: 100%;" scrolling="no" title="070902" src="https://codepen.io/tiroring09/embed/qBOPQqy?height=265&theme-id=light&default-tab=css,result" frameborder="no" allowtransparency="true" allowfullscreen="true" loading="lazy">
  See the Pen <a href='https://codepen.io/tiroring09/pen/qBOPQqy'>070902</a> by tiroring09
  (<a href='https://codepen.io/tiroring09'>@tiroring09</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

## 다채로운 테두리

지금까지는 4면의 테두리가 모두 같았는데, 다 다르게 설정해주고 싶으면 이렇게 하면 됩니다:

<iframe height="265" style="width: 100%;" scrolling="no" title="070903" src="https://codepen.io/tiroring09/embed/RwWLqoO?height=265&theme-id=light&default-tab=css,result" frameborder="no" allowtransparency="true" allowfullscreen="true" loading="lazy">
  See the Pen <a href='https://codepen.io/tiroring09/pen/RwWLqoO'>070903</a> by tiroring09
  (<a href='https://codepen.io/tiroring09'>@tiroring09</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

## 테두리 없애기

어떤 요소들(예: `<input>` 태그)은 기본적으로 테두리가 설정되어 있습니다. 이런 요소들의 테두리를 없애고 싶으면 직접 border 속성을 설정해주면 되는데요. 두 가지 방법이 있습니다:

1. border: none;
2. border: 0;
