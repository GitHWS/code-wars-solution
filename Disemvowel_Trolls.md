# Disemvowel Trolls

## Requirement

<p>Trolls are attacking your comment section!

A common way to deal with this situation is to remove all of the vowels from the trolls' comments, neutralizing the threat.

Your task is to write a function that takes a string and return a new string with all vowels removed.

For example, the string "This website is for losers LOL!" would become "Ths wbst s fr lsrs LL!".

Note: for this kata `y` isn't considered a vowel.</p>

  1. 문자열 내 모든 모음을 제거한 상태에서 새로운 문자열을 반환하는 함수를 완성하라
  2. `y`는 모음으로 간주하지 않는다.

## Example

```js
"This website is for losers LOL!" => "Ths wbst s fr lsrs LL!".
```

<br>

### 첫번째 나의 시도

> why? 이렇게 특정 문자를 선택해서 삭제하는 것은 "정규표현식"이 쉽다고 들은 적이 있어서 정규표현식을 사용해서 a,e,i,o,u를 `replace()`로 교체했지만 앞의 `split()` 과정을 괜히 한 것 같다..

```js
function disemvowel(str) {
  return ("" + str.split()).replace(/[aeiou]/gim, "");
}
```
- 결과

> why? 내가 원하던 함수는 이것이었는데 위처럼 복잡하게 해서 다시 공부하도록 해야겠다. 그리고 하는 과정 중 정규표현식을 사용하는 곳에서 조금 헤매서 공부를 해야할 것 같다!

```js
function disemvowel(str) {
  return str.replace(/[aeiou]/gi, '');
}
```
