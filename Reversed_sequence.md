# Reversed sequence

## Requirement

<p>Build a function that returns an array of integers from n to 1 where `n>0`.</p>

  1. n부터 1까지의 정수를 배열에 저장하는 함수를 완성시켜라.
  2. n은 0보다 크다.

## Example

```js
n=5 --> [5,4,3,2,1]
```

<br>

### 첫번째 나의 시도

> why? 일단 빈 배열 안에 요소를 넣는 `push()`를 사용해야 한다고 우선 생각했고 반복문으로 루프될 때마다 `-1`을 해주면서 빈 배열에 하나씩 요소를 넣고 리턴한다고 생각했다!

```js
const reverseSeq = n => {
  let arr = [];
  for(let i = n; i > 0; i--){
    arr.push(i);
  }
  return arr;
};
```
- 결과

> why? 성공~! 다른 풀이 중에 신기한 것이 있어서 더 봐야겠다.

![image](https://user-images.githubusercontent.com/96808980/172963499-07b0c9e2-e54f-4648-bf71-dd1fe1d77f27.png)

### 신기한 풀이

> why? `Array(n)`으로 `""`의 요소가 5개인 배열을 생성하고 모든 요소를 0으로 채우고 `map()`으로 모든 요소를 순회하면서 `(e, i)`에서 인덱스를 가리키는 `i`를 n에 빼줌으로서 순차적으로 요소가 저장이 된다. `map()`으로 인해 새로운 배열이 생성된다.

```js
const reverseSeq = n => {
  return Array(n).fill(0).map((e, i) => n - i );
};
```
