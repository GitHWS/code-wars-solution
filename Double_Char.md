# Double Char

## Requirement

<p>Given a string, you have to return a string in which each character (case-sensitive) is repeated once.</p>

  1. 주어진 문자열의 각각의 글자를 한번 더 반복하여  함수를 완성시켜라

## Example

```js
* "String"      -> "SSttrriinngg"
* "Hello World" -> "HHeelllloo  WWoorrlldd"
* "1234!_ "     -> "11223344!!__  "
```

<br>

### 첫번째 나의 시도

> why? 문자열을 각각의 글자로 나누기 위해 `split("")`을 사용하고 `map()`을 통해 요소를 반복하는데 각 요소를 `repeat()`를 통해 2번 반복하고 마지막 결과를 `join()`을 해서 한 문자열로 합쳐준다.

```js
function doubleChar(str) {
  return str.split("").map(item => item.repeat(2)).join("")
}
```
- 결과

![image](https://user-images.githubusercontent.com/96808980/174488805-9c047ca5-8dcb-48b7-957c-4a7f742e8490.png)
