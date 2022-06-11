# Return Negative

## Requirement

<p>In this simple assignment you are given a number and have to make it negative. But maybe the number is already negative?</p>
<ul>
  <li>The number can be negative already, in which case no change is required.</li>
  <li>Zero (0) is not checked for any specific sign. Negative zeros make no mathematical sense.</li>
</ul>
  

  1. 주어진 숫자를 음수로 변환하라
  2. 만약 이미 음수라면, 변경할 필요가 없다.
  3. 수학적으로 존재하지 않는 `-0`은 `0`과 똑같기 때문에 신경쓸 필요가 없다.

## Example

```js
makeNegative(1);    // return -1
makeNegative(-5);   // return -5
makeNegative(0);    // return 0
makeNegative(0.12); // return -0.12
```

<br>

### 첫번째 나의 시도

> why? 처음으로 삼항연산자를 사용해서 풀었다. `num`이 `0`보다 작을 경우(음수일 경우) `num`을 음수 그대로 리턴하고 양수(num > 0)의 경우 `-num`으로 변환하고 리턴한다.
```js
function makeNegative(num) {
  return num < 0 ? num : -num;
}
```
- 결과

> why? 성공! 절대값을 주는 `Math.abs()`를 사용한 사람도 있어서 한번 보면 재미있을 것 같다!

![image](https://user-images.githubusercontent.com/96808980/173193367-f64126d5-14cb-4004-b736-572bf70dded4.png)

```JS
function makeNegative(num) {
  return -Math.abs(num);
}
```
