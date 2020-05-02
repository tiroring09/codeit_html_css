# CSS 상속

[TOC]

CSS에는 '상속'이라는 개념이 있습니다. 말 그대로 부모 요소의 속성들을 자식들한테 넘겨주는 것인데요. 예시를 한 번 봅시다.

<iframe height="265" style="width: 100%;" scrolling="no" title="080401" src="https://codepen.io/tiroring09/embed/bGVoyRz?height=265&theme-id=default&default-tab=html,result" frameborder="no" allowtransparency="true" allowfullscreen="true" loading="lazy">
  See the Pen <a href='https://codepen.io/tiroring09/pen/bGVoyRz'>080401</a> by tiroring09
  (<a href='https://codepen.io/tiroring09'>@tiroring09</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

.div1의 폰트 색을 blue로 설정해주었고, `<h1>`과 `<p>`에 대해서는 별도의 설정이 없었습니다. 그런데도 `<h1>`과 `<p>` 태그의 폰트 색이 파란색으로 설정되었죠? 그 이유는 .div1의 스타일이 자식들에게 상속되었기 때문입니다.

## 상속되는 속성들

하지만 태그와 속성에 따라 상속이 되지 않는 경우도 많이 있습니다. 예를 들어서 부모 태그에 설정한 margin이 모든 자식들에게도 적용되면 총체적 난국이 되겠죠?

웬만하면 상속되는 몇 가지 속성들입니다:

- color
- font-family
- font-size
- font-weight
- line-height
- list-style
- text-align
- visibility

이외에도 많지만 일단 자주 사용하는 몇 가지만 적어두었습니다.

위에 있는 속성들도 항상 상속되는 건 아닙니다. 대표적인 예로 `<a>` 태그에는 color 속성이 상속되지 않습니다. `<a>` 태그가 억지로 상속을 받아오기 위해서는 해당 속성에 inherit 값을 쓰면 됩니다!

<iframe height="265" style="width: 100%;" scrolling="no" title="080402" src="https://codepen.io/tiroring09/embed/NWGaVvJ?height=265&theme-id=default&default-tab=html,result" frameborder="no" allowtransparency="true" allowfullscreen="true" loading="lazy">
  See the Pen <a href='https://codepen.io/tiroring09/pen/NWGaVvJ'>080402</a> by tiroring09
  (<a href='https://codepen.io/tiroring09'>@tiroring09</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

