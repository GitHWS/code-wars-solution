# Square Every Digit

## Requirement

<p>Welcome. In this kata, you are asked to square every digit of a number and concatenate them.

For example, if we run `9119` through the function, `811181` will come out, because `9^2` is `81` and `1^2` is `1`.

Note: The function accepts an integer and returns an integer

</p>

  1. 주어진 숫자의 각 자리수를 제곱하여 하나로 합친 숫자를 만들어라
  2. 함수는 정수만 받고 정수만을 리턴한다.

## Example

```js
9119 => 811181 (9^2 1^2 1^2 9^2)
```

<br>

### 첫번째 나의 시도

> why? 정수로 받은 `num`을 `String()`을 통해 숫자형을 문자열로 바꾸고 `Array.from()`메서드를 통해 문자열 요소를 가진 배열을 만들고 각 요소에 숫자형으로 변환하는 `Number`함수를 사용한다. 이후 `map()` 메서드를 사용해서 각 요소를 제곱해주고 `join()`을 통해 하나의 문자열로 합친 후 `parseInt()`로 숫자형으로 변환시켜준다.

```js
function squareDigits(num){
  return parseInt(Array.from(String(num), Number).map(item => item ** 2).join(""));
}
```
- 결과

![image](https://user-images.githubusercontent.com/96808980/174018803-c7ac04d0-2b1f-4171-a210-e66d03686c8e.png)
