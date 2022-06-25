# Find the smallest integer in the array

## Requirement

<p>Given an array of integers your solution should find the smallest integer.

</p>

  1. 정수로 이루어진 배열에서 가장 작은 수를 반환하라

## Example

```js
[34, 15, 88, 2] => 2
[34, -345, -1, 100] => -345
```

<br>

### 첫번째 나의 시도

> why? 첫 시작이 `class`라 당황했지만 `class`의 메서드이기 때문에 기존 함수와 똑같이 하면 되는 문제였다. `arg`는 정수를 모아놓은 배열이고 전개 구문을 통해 배열을 문자열로 만들고 `Math.min()`으로 가장 작은 수를 반환한다.

```js
class SmallestIntegerFinder {
  findSmallestInt(args) {
   return Math.min(...args);
  }
}

// 실행은 이렇게!
let minInt = new SmallestIntegerFinder().findSmallestInt([1,2,3,4,5]) // 1
```

- 결과

![image](https://user-images.githubusercontent.com/96808980/175763315-9af7521a-6bb4-41d0-b5d2-8f7a5d15b0d9.png)
