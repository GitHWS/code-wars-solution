# Descending Order

## Requirement

<p>Your task is to make a function that can take any non-negative integer as an argument and return it with its digits in descending order. Essentially, rearrange the digits to create the highest possible number.

</p>

  1. 음수가 아닌 정수를 인자로 받아 재조합하여 가장 큰 숫자로 만드는 함수를 완성하라

## Example

```js
Input: 42145 Output: 54421

Input: 145263 Output: 654321

Input: 123456789 Output: 987654321
```

<br>

### 첫번째 나의 시도

> why? `[...n.toString()]`으로 문자열로 만들어 배열로 형변환 시킨 다음 `sort()`로 오름차순을 시키고 `reverse()`로 역순으로 정렬하고 `join()`으로 합쳐준다. 여기서 가장 혼란스러웠던 점이 맨 앞의 `+`가 없어서 문자열이 계속 반환되었기 때문에 계속 틀렸었다. 데이터 타입에 대해서 주의해야할 것 같다.

```js
function descendingOrder(n){
  return +[...n.toString()].sort().reverse().join("")
}
```
- 결과

![image](https://user-images.githubusercontent.com/96808980/175067586-8b70ff88-4997-4f33-9a33-d0b534be4710.png)
