# Remove exclamation marks

## Requirement

<p>Write function RemoveExclamationMarks which removes all exclamation marks from a given string.</p>

  1. 주어진 문자열에서 느낌표를 삭제하고 반환하는 함수를 완성하라

## Example

```js
"Hello world!" => "Hello world"
```

<br>

### 첫번째 나의 시도

> why? 전개구문을 이용해서 문자열을 배열로 만들어주고 `filter()`로 "!"가 아닌 요소를 골라 배열로 재구성하고 `join()`을 통해 하나의 문자열로 만들어준다. 

```js
function removeExclamationMarks(s) {
  return [...s].filter(item => item !== "!").join("")
}
```
- 결과

![image](https://user-images.githubusercontent.com/96808980/174689856-f223c29d-899c-46fd-abb5-0814ec8af289.png)
