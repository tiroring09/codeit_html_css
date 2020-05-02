# Padding과 Margin의 차이

[TOC]

Padding과 Margin은 쉽게 헷갈릴 수 있는 개념입니다. 차이를 정확히 집고 넘어갑시다!

요소는 내용(content), 패딩(padding), 테두리(border)로 이루어져 있습니다. Padding은 내용과 테두리 사이의 '여유 공간'입니다. 반면에 Margin은 요소 주위의 여백입니다. 즉, 테두리 밖의 공간인 셈이죠.

## Padding

Padding을 주는 방법에는 몇 가지가 있습니다.

### 가장 직관적인 방법

우선 가장 직관적인 방법입니다:
<iframe height="265" style="width: 100%;" scrolling="no" title="070301" src="https://codepen.io/tiroring09/embed/xxwXyop?height=265&theme-id=light&default-tab=html,result" frameborder="no" allowtransparency="true" allowfullscreen="true" loading="lazy">
  See the Pen <a href='https://codepen.io/tiroring09/pen/xxwXyop'>070301</a> by tiroring09
  (<a href='https://codepen.io/tiroring09'>@tiroring09</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

### 한 줄에

한 줄에 쓰고 싶으면 padding 속성을 쓰면 되는데요. 순서는 위(padding-top)부터 시계 방향으로 하나씩 쓰면 됩니다.

<iframe height="265" style="width: 100%;" scrolling="no" title="070302" src="https://codepen.io/tiroring09/embed/wvKrYVw?height=265&theme-id=light&default-tab=html,result" frameborder="no" allowtransparency="true" allowfullscreen="true" loading="lazy">
  See the Pen <a href='https://codepen.io/tiroring09/pen/wvKrYVw'>070302</a> by tiroring09
  (<a href='https://codepen.io/tiroring09'>@tiroring09</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

### 위, 아래, 왼쪽, 오른쪽이 다 같은 경우

만약 위, 아래, 왼쪽, 오른쪽에 똑같은 padding을 주고 싶으면 더 간편합니다. 모두 50px의 padding을 주려면 이렇게 하면 됩니다:
<iframe height="265" style="width: 100%;" scrolling="no" title="070303" src="https://codepen.io/tiroring09/embed/vYNeQBQ?height=265&theme-id=light&default-tab=html,result" frameborder="no" allowtransparency="true" allowfullscreen="true" loading="lazy">
  See the Pen <a href='https://codepen.io/tiroring09/pen/vYNeQBQ'>070303</a> by tiroring09
  (<a href='https://codepen.io/tiroring09'>@tiroring09</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

### 위, 아래가 같고, 왼쪽, 오른쪽이 같은 경우

위, 아래에 50px의 padding을 주고, 왼쪽, 오른쪽에 100px의 padding을 주려면 이렇게 하면 됩니다:
<iframe height="265" style="width: 100%;" scrolling="no" title="070304" src="https://codepen.io/tiroring09/embed/jObGQOW?height=265&theme-id=light&default-tab=html,result" frameborder="no" allowtransparency="true" allowfullscreen="true" loading="lazy">
  See the Pen <a href='https://codepen.io/tiroring09/pen/jObGQOW'>070304</a> by tiroring09
  (<a href='https://codepen.io/tiroring09'>@tiroring09</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

## Margin

요소에게 margin을 주는 방법은 padding을 주는 방법과 똑같습니다.


### 가장 직관적인 방법
<iframe height="265" style="width: 100%;" scrolling="no" title="070305" src="https://codepen.io/tiroring09/embed/eYpGQYW?height=265&theme-id=light&default-tab=html,result" frameborder="no" allowtransparency="true" allowfullscreen="true" loading="lazy">
  See the Pen <a href='https://codepen.io/tiroring09/pen/eYpGQYW'>070305</a> by tiroring09
  (<a href='https://codepen.io/tiroring09'>@tiroring09</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

### 한 줄에
그러니까 위의 코드와 똑같이 쓰기 위해서는 이렇게 하면 되는 거죠:
<iframe height="265" style="width: 100%;" scrolling="no" title="070306" src="https://codepen.io/tiroring09/embed/VwvMVwE?height=265&theme-id=light&default-tab=html,result" frameborder="no" allowtransparency="true" allowfullscreen="true" loading="lazy">
  See the Pen <a href='https://codepen.io/tiroring09/pen/VwvMVwE'>070306</a> by tiroring09
  (<a href='https://codepen.io/tiroring09'>@tiroring09</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

### 위, 아래, 왼쪽, 오른쪽이 다 같은 경우
```
p {
  margin: 50px;
}
```

### 위, 아래가 같고, 왼쪽, 오른쪽이 같은 경우
```
p {
  margin: 50px 70px;
}
```

## 가운데 정렬

요소를 가운데 정렬하고 싶으면 왼쪽과 오른쪽 margin 값을 auto로 설정해줘야 합니다. auto는 말 그대로 '자동으로 계산'하라는 뜻인데요. 왼쪽과 오른쪽을 auto로 설정하면 자동으로 왼쪽과 오른쪽을 똑같이 함으로써 요소는 가운데 정렬이 됩니다.
<iframe height="265" style="width: 100%;" scrolling="no" title="070307" src="https://codepen.io/tiroring09/embed/wvKrQBv?height=265&theme-id=light&default-tab=html,result" frameborder="no" allowtransparency="true" allowfullscreen="true" loading="lazy">
  See the Pen <a href='https://codepen.io/tiroring09/pen/wvKrQBv'>070307</a> by tiroring09
  (<a href='https://codepen.io/tiroring09'>@tiroring09</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>