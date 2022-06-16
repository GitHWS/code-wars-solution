# Count by X

## Requirement

<p>Create a function with two arguments that will return an array of the first (n) multiples of (x). Assume both the given number and the number of times to count will be positive numbers greater than 0. Return the results as an array (or list in Python, Haskell or Elixir).</p>

  1. 함수는 파라미터로 숫자인 `x`, 배수를 뜻하는 `n`을 가진다.
  2. 숫자 `x`의 배수를 `n`개 출력하는 배열을 반환하라
  3. 

## Example

```js
countBy(1,10) === [1,2,3,4,5,6,7,8,9,10]
countBy(2,5) === [2,4,6,8,10]
```

<br>

### 첫번째 나의 시도

> why? 문제를 시작할 때 `z`라는 빈 배열이 있어서 하나의 결과값이 나올 때마다 `push()`를 해야할 것이라고 생각했다. 그리고 각 요소가 배수를 나타내야하기 때문에 반복문을 통해 연산하여 배열에 `push()`한다.
 
```js
function countBy(x, n) {
  let z = [];
  for(let i = 1; i <= n; i++){
   z.push(x*i) 
  }
  return z;
}
```
- 결과

![image](https://user-images.githubusercontent.com/96808980/174021801-6a4651b7-5310-4a94-a9ed-84b83afb0d02.png)
