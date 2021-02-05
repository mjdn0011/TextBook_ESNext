# TextBook-ESNext
ESNext description &amp; example codes (for study)

# ES6: ECMAScript 6
* Arrow Function
* Enhanced Object Literal

## 1. Arrow Function: 화살표 함수
* 함수를 정의할 때 `function` 키워드를 사용하지 않고 `=>`로 대체
* 흔히 사용하는 <u>콜백 함수의 문법을 간결화</u>
```js
// ES5
var sum = function(a, b) {
  return a + b;
};

// ES6
const sum = (a, b) => {
  return a + b;
}
```
```js
// ES5
var arr = ["a", "b", "c"];
arr.forEach(function(value) {
  console.log(value);
});

// ES6
var arr = ["a", "b", "c"];
arr.forEach((value) => console.log(value));

```

## 2. Enhanced Object Literal: 향상된 객체 리터럴
* **객체의 속성을 메서드로 사용할 때** `function` 예약어를 생략하고 생성 가능

```js
var dictionary = {
  words: 100,

  // ES5
  lookup: function() {
    console.log('find words');
  },

  // ES6
  lookup() {
    console.log('find words');
  }
}
```

```js
var dictionary = {
  // ES5
  'text': 'text',
  // ES6
  text,
}
```