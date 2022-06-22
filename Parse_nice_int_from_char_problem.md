# Parse nice int from char problem

## Requirement

<p>You ask a small girl,"How old are you?" She always says, "x years old", where x is a random number between 0 and 9.

Write a program that returns the girl's age (0-9) as an integer.

Assume the test input string is always a valid string. For example, the test input may be "1 year old" or "5 years old". The first character in the string is always a number.</p>

  1. "`x` years old"라는 문자열에서 정수를 반환하는 함수를 완성하라

## Example

```js
1 year old => 1;
5 years old => 5;
```

<br>

### 첫번째 나의 시도

> why? 문자열 속 정수를 찾아내는 문제였다. 문자열을 `parseInt()`의 인자로 사용하면 문자열에서 가장 앞에 위치한 정수만 반환해준다.
> 
```js
function getAge(inputString){
  return parseInt(inputString);
}
```
- 결과

![image](https://user-images.githubusercontent.com/96808980/175062680-c2f52e0b-2839-472e-8a48-458f257b722d.png)
