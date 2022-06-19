# Reverse words

## Requirement

<p>Complete the function that accepts a string parameter, and reverses each word in the string. All spaces in the string should be retained.</p>

  1. 주어진 문자열의 띄어쓰기는 유지하며 단어를 모두 반전시키는 함수를 완성시켜라

## Example

```js
"This is an example!" ==> "sihT si na !elpmaxe"
"double  spaces"      ==> "elbuod  secaps"
```

<br>

### 첫번째 나의 시도

> why? 우선 문자열을 `split(" ")`으로 단어별로 나누어 배열로 만들고 `map()` 메서드를 사용하여 모든 요소를 순회하도록 하고 콜백으로 각 아이템(문자열)을 스프레드 연산자를 통해 한 글자로 전개해주고 `reverse()`로 역순으로 만들고 `join()`으로 합쳐주고 결과가 배열이니 한번 더 `join()`을 통해 문자열로 만들어준다. 

```js
function reverseWords(str) {
  return str.split(" ").map(item => [...item].reverse().join("")).join(" ")
}
```
- 결과

![스크린샷 2022-06-20 오전 12 22 09](https://user-images.githubusercontent.com/96808980/174488407-653d969f-ac24-4330-b80a-9939d2a19015.png)
