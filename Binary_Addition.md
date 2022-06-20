# Binary Addition

## Requirement

<p>Implement a function that adds two numbers together and returns their sum in binary. The conversion can be done before, or after the addition.

The binary number returned should be a string.</p>

  1. 매개변수로 받는 두 수의 합의 "2진수"로 변환한 결과를 구하는 함수를 완성해라
  2. 2진수는 반드시 "문자열"로 반환해야한다.
  3. 

## Example

```js
1, 1 --> "10" (1 + 1 = 2 in decimal or 10 in binary)
5, 9 --> "1110" (5 + 9 = 14 in decimal or 1110 in binary)
```

<br>

### 첫번째 나의 시도

> why? 매개변수 a+b를 구해야하기 때문에 (a+b)를 해주고 2진수를 구하기 위해 `toSting()`에 인자 2를 넣어서 2진수로 변환해준다. 

```js
function addBinary(a,b) {
  return Number(a+b).toString(2);
}
```
- 결과

![image](https://user-images.githubusercontent.com/96808980/174635474-f027aa9c-6832-4980-8aeb-83ce3782d84d.png)
