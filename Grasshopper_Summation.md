# Grasshopper - Summation

## Requirement

<p>Write a program that finds the summation of every number from 1 to num. The number will always be a positive integer greater than 0.</p>

  1. 1부터 숫자까지의 합을 구하라.
  2. `num`는 0보다 큰 양의 정수이다.

## Example

```js
summation(2) -> 3
1 + 2

summation(8) -> 36
1 + 2 + 3 + 4 + 5 + 6 + 7 + 8
```

<br>

### 첫번째 나의 시도

> why? 1부터 `num`까지의 합이니 반복문 for의 `i`는 `1`로 설정하고 `num`을 포함한 합이기 때문에 `<= num`으로 설정한다. 또한 합계를 의미하는 변수인 `sum`를 만들어서 `i`가 반복될 때마다 더 해주면 될 것 같다!
```js
var summation = function (num) {
  // Code here
  let sum = 0;
  for(let i = 1; i <= num; i++){
      sum += i;
  }
  return sum;
}
```
- 결과

> why? 역시 반복문을 이용하면 `num`만큼의 합을 구할 수 있을 것 같았다. 첫번째 시도만에 성공!

![image](https://user-images.githubusercontent.com/96808980/172208446-d5e0de54-faeb-408e-a47e-9c1d1a61a99c.png)
