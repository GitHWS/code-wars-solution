# Ones and Zeros

## Requirement

<p>Given an array of ones and zeroes, convert the equivalent binary value to an integer.</p>

  1. 주어진 배열은 `1`과 `0`으로 이루어져 있는데 이것을 "이진 수" 값을 "정수"로 변환해라

## Example

```js
Testing: [0, 0, 0, 1] ==> 1
Testing: [0, 0, 1, 0] ==> 2
Testing: [0, 1, 0, 1] ==> 5
Testing: [1, 0, 0, 1] ==> 9
Testing: [0, 0, 1, 0] ==> 2
Testing: [0, 1, 1, 0] ==> 6
Testing: [1, 1, 1, 1] ==> 15
Testing: [1, 0, 1, 1] ==> 11
```

<br>

### 첫번째 나의 시도

> why? 내가 받은 것은 배열인데 결과 값이 숫자라는 것은 배열을 문자열로 변경하여 숫자 타입으로 변환해야한다는 것! 그래서 주어진 배열을 `join("")` 메서드를 사용하여 배열 안의 요소를 ","없이 하나의 문자열로 만들고 `parseInt()`에 사용되는 인자 `string`, `radix`를 사용하여 이전에 만든 문자열을 `string`에, `radix`에 `2`를 넣어서 2진수를 변환한다.

```js
const binaryArrayToNumber = arr => {
  return parseInt(arr.join(""), 2)
};
```
- 결과

> why? 성공! 변환/진수라는 것에 반사적으로 `join()`과 `parseInt()` 메서드가 떠올랐다! 공부한 노력이 조금 보이는 듯!

![image](https://user-images.githubusercontent.com/96808980/173377057-2f45d7b2-d45c-4b94-9086-36780107af5c.png)
