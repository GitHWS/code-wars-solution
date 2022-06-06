# Square(n) Sum

## Requirement

<p>Complete the square sum function so that it squares each number passed into it and then sums the results together.</p>

  1. 전달된 각 숫자를 제곱한 후 모든 요소의 합을 구한다.

## Example

```js
[1, 2, 2] => 1^2 + 2^2 + 2^2 = 9
```

<br>

### 첫번째 나의 시도

> why? 제곱한 요소의 전체 합을 구하기 때문에 합계를 위한 변수 `result`를 선언하고 `forEach()`를 통해 모든 요소에 제곱을 하고 `result`에 누적해주고 반환한다.

```js
function squareSum(numbers){
  let result = 0;
  numbers.forEach((element, index, array) => {
    array[index] = element ** 2;
    result += array[index];
  })
  return result;
}
```
- 결과

> why? `forEach()`를 사용해서 결과를 반환했지만 다른 사람들의 답이 더 간결하고 좋아보인다.. 🤔

![image](https://user-images.githubusercontent.com/96808980/172267592-4e4d084a-9277-498b-8aaa-6a20ad51f063.png)


### 가장 많이 사용한 답안

> why? `reduce()` 메서드에 콜백함수를 사용해서 합계를 즉시 구하는 것 같다. 코드에 답은 없지만 다른 분들 정말 대단..👍

```js
function squareSum(numbers){
  return numbers.reduce(function(sum, n){
    return (n*n) + sum;
  }, 0)
}
```
