# Even or Odd

## Requirement

<p>Create a function that takes an integer as an argument and returns "Even" for even numbers or "Odd" for odd numbers.</p>

  1. 정수를 짝수인지 홀수인지 비교하는 함수를 만들어라

## Example

```js
1 => "Odd"
2 => "Even"
-39 => "Odd"
-42 => "Even"
```

<br>

### 첫번째 나의 시도

> why? 파라미터로 받은 정수를 2로 나누었을 때 1이 남는 것은 "Odd", 0인 것은 "Even", 여기서 1은 "true", 0은 "false"이므로 홀수일 때 참이기 때문에 가장 첫번째 조건문이 실행이 되고 아니라면 마지막 else 조건문이 실행된다.


```js
function even_or_odd(number) {
  if(number % 2){
    return 'Odd'
  }else{
    return 'Even'
  }
}
```

```js
function even_or_odd(number) {
  return number % 2 ? "Odd" : "Even"
}
```
- 결과

![image](https://user-images.githubusercontent.com/96808980/173888525-7e5d2f28-bd70-4671-913e-3aab48780e28.png)
