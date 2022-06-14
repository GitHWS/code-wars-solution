# String repeat

## Requirement

<p>Write a function called `repeatStr` which repeats the given string `string` exactly `n` times.</p>

  1. `string`을 `n`번 반복하여 하나의 문자열로 만들어라

## Example

```js
repeatStr(6, "I") // "IIIIII"
repeatStr(5, "Hello") // "HelloHelloHelloHelloHello"
```

<br>

### 첫번째 나의 시도

> why? 문자열 메서드인 `repeat(n)`을 사용하여 반복하면 된다.

```js
function repeatStr (n, s) {
  return s.repeat(n);
}
```
- 결과

![스크린샷 2022-06-14 오후 8 41 20](https://user-images.githubusercontent.com/96808980/173569817-abf0b9f0-14e4-48b9-bc67-9fddff56a815.png)
