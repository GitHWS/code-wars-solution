# You only need one - Beginner

## Requirement

<p>You will be given an array a and `a` value `x`. All you need to do is check whether the provided array contains the value.

Array can contain numbers or strings. X can be either.

Return `true` if the array contains the value, `false` if not.</p>

  1. 배열 `a`에 요소 중 `x`가 있는지 확인하는 함수를 완성하라
  2. 요소가 존재하면 `true`, 존재하지않으면 `false`를 반환하라

## Example

```js
[66, 101], 66 => true;
[101, 45, 75, 105, 99, 107], 107 => true;
['t', 'e', 's', 't'], 'e' => true;
['what', 'a', 'great', 'kata'], 'kat' => false;
```

<br>

### 첫번째 나의 시도

> why? 내부의 요소가 있는지 확인해서 있으면 `true`, 없으면 `false`를 반환하는 `includes()` 메서드를 사용해서 해결하였다. `include"s"` s가 붙어야한다..! 
```js
function check(a, x) {
  return a.includes(x) ? true : false;
}
```
- 결과

![image](https://user-images.githubusercontent.com/96808980/174691113-985ae82f-9781-49fa-80c2-0e3820beb584.png)
