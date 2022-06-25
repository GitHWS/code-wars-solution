# Filling an array (part 1)

## Requirement

<p>We want an array, but not just any old array, an array with contents! Write a function that produces an array with the numbers `0` to `N-1` in it.</p>

  1. 0부터 주어진 숫자의 `-1`한 값까지 배열의 요소로 모두 넣어 반환하라

## Example

```js
arr(5) // => [0,1,2,3,4]
```

<br>

### 첫번째 나의 시도

> why? 예전 문제와 비슷하게 배열에 요소를 넣어야하기 때문에 빈 배열을 변수로 만들어주고 for문을 통해 N 미만의 값까지만 반복을 하여 하나씩 빈 배열에 `push()`해준다. 

```js
const arr = N => {
  const emptyArr = []
  for(let i = 0; i < N; i++){
    emptyArr.push(i);
  }
  return emptyArr;
}
```

- 결과

![image](https://user-images.githubusercontent.com/96808980/175762708-b6d06523-0691-488f-a87c-1050e189a8d9.png)
