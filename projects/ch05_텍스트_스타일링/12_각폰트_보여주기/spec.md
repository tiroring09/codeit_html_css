# 각 폰트 보여주기

현재 `<div>` 태그가 여섯 개 있는데요. 처음 다섯 개를 보시면 우리가 배운 폰트 종류 다섯 가지가 각각 써져 있습니다. 각 `<div>` 태그를 지정된 폰트 종류에 포함되는 font-family로 설정해주세요.

그리고 마지막 `<div>` 태그에는 Google이라고 적혀 있습니다. 마지막 `<div>`는 구글 웹폰트를 사용해주세요!

styles.css 파일에 작성하면 됩니다!

## 힌트1: 폰트 5가지

serif, sans-serif, monospace, cursive, fantasy는 Generic Font Family라고 부릅니다. 이들은 쌍따옴표 없이 써야 적용이 됩니다.

반면 그 앞에 일반적으로 오는 지정 폰트들은 중간에 띄어쓰기가 있으면 무조건 "Times New Roman"처럼 쌍따옴표 안에 써야 하며, 띄어쓰기가 없으면 쌍따옴표 없이 써도 됩니다.

예를 들어, serif 아이디에서 "Times New Roman" 폰트를 쓰고 싶고, 이 폰트가 없으면 차선책으로 "Times" 폰트를, 이마저도 없다면 Generic Font Family인 serif에 속한 폰트를 사용하고 싶다면 아래와 같이 표현할 수 있습니다.
```
#serif {
  font-family: "Times New Roman", "Times", serif;
}
```

## 힌트2: 구글 웹폰트
구글 웹폰트 홈페이지에 있는 폰트를 사용하는 방법은, 구글 웹폰트 강의에 자세히 설명되어있는데요!

예를 들어 홈페이지에 있는 "Roboto" 폰트를 이용하고 싶다면 어떻게 해야 할까요?

홈페이지에서 해당 폰트를 누르면 1 Family Selected라는 메시지가 나옵니다.

해당 메시지를 클릭하면 Embed Font라는 탭 아래에 html 파일에 붙여넣을 링크가 제공됩니다.

```
<link href="https://fonts.googleapis.com/css?family=Roboto" rel="stylesheet">
```

위의 링크를 html 파일의 head 부분에 넣습니다.

마찬가지로 Specify in CSS라는 탭 아래에 css 파일에 붙여넣을 font-family가 제공됩니다.

```
font-family: 'Roboto', sans-serif;
```

해당 부분을 google 아이디가 있는 부분에 아래와 같이 붙여넣으면 됩니다.

```
#google {
  font-family: 'Roboto', sans-serif;
}
```