# Mumbling

## Requirement

<p>This time no story, no theory. The examples below show you how to write function `accum`. The parameter of accum is a string which includes only letters from `a..z` and `A..Z`.

</p>

  1. 함수의 파라미터는 `a-z` 그리고 `A-Z`의 문자만 포함한다.
  2. 예시를 보고 함수를 완성해라
  3. 

## Example

```js
accum("abcd") -> "A-Bb-Ccc-Dddd"
accum("RqaEzty") -> "R-Qq-Aaa-Eeee-Zzzzz-Tttttt-Yyyyyyy"
accum("cwAt") -> "C-Ww-Aaa-Tttt"
```

<br>

### 첫번째 나의 시도

> why? 문자열을 넣었을 때 첫번째 글자는 "대문자", 이후 반복되는 모든 글자는 소문자이다. 또한 반복되는 횟수는 각 요소의 인덱스만큼 반복되는 것을 알 수 있다.

```js
function accum(s) {
  return s.split('').map((c, i) => (c.toUpperCase() + c.toLowerCase().repeat(i))).join('-');
}
```

1. 문자열을 받는 `s`를 빈문자열을 구분자로 사용하여 분리해서 배열로 만들어준다.
2. 만든 배열에 `map`메서드를 사용하는데 요소를 나타내는 c, 각 요소의 인덱스를 담고 있는 i를 설정한다.
3. 첫 번째 글자를 `toUpperCase()`를 통해 대문자로 변환하고 나머지 글자 또한 `toLowerCase()`를 통해 소문자로 변환해준다. 그리고 이 둘을 합치기 전 `repeat(i)`을 통해 각 요소의 인덱스만큼 반복해준다.
4. 구분자 "-"를 사용하여 분리하여 하나의 문자열로 형성한다.

- 결과

실패... 7 kyu는 아직 문제가 어려운가.. 생각을 해야할 것이 너무 많아서 복잡해졌다.. 그래서 7 kyu부터는 모르는 것을 잡고 있지 않고 일정시간이 지나면 답을 보고 익히는 식으로 해야할 것 같다...

> why?
