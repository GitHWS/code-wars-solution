# Make a function that does arithmetic!

## Requirement

<p>Given two numbers and an arithmetic operator (the name of it, as a string), return the result of the two numbers having that operator used on them.

`a` and `b` will both be positive integers, and `a` will always be the first number in the operation, and `b` always the second.

The four operators are "add", "subtract", "divide", "multiply".</p>

  1. 연산자에 따라 연산 결과를 반환하는 함수를 완성하라
  2. `a`, `b`는 항상 양수이며 `a`는 항상 첫번째 숫자, `b`는 항상 두번째 숫자이다.

## Example

```js
5, 2, "add"      --> 7
5, 2, "subtract" --> 3
5, 2, "multiply" --> 10
5, 2, "divide"   --> 2.5
```

<br>

### 첫번째 나의 시도

> why? 명확하게 연산자의 값이 정해지기 때문에 switch문을 사용하는 것이 좋을 것 같았다. 각각 연산자에 따라 연산 결과를 반환하게 하였다.
```js
function arithmetic(a, b, operator){
  switch(operator){
      case 'add':
        return a+b;
        break;
      case 'subtract':
        return a-b;
        break;
      case 'multiply':
        return a*b;
        break;
      case 'divide':
        return a/b;
        break;
  }
}
```
- 결과

![image](https://user-images.githubusercontent.com/96808980/174814008-62b8629e-4ed8-4f25-92e8-abb8ce66311b.png)
