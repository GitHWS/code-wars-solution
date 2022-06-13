# List Filtering

## Requirement

<p>In this kata you will create a function that takes a list of non-negative integers and strings and returns a new list with the strings filtered out.</p>

  1. 음수가 아닌 정수와 문자열을 요소를 가진 배열로 필터링하여 반환하는 함수를 완성시켜라

## Example

```js
filter_list([1,2,'a','b']) == [1,2]
filter_list([1,'a','b',0,15]) == [1,0,15]
filter_list([1,2,'aasf','1','123',123]) == [1,2,123]
```

<br>

### 첫번째 나의 시도

> why? 배열 내 조건에 맞는 것을 골라내기 위해 `filter()` 메서드를 사용하고 조건으로 1.음수가 아닌  2.정수/문자열이기 때문에 조건식을 아래처럼 작성했다.
> 
```js
function filter_list(l) {
  return l.filter(item => typeof item === "number" && item >= 0);
}
```
- 결과

![image](https://user-images.githubusercontent.com/96808980/173381288-2145f04b-8d34-47e2-8576-b3f1599e1c71.png)

> why? 정수는 처리를 했는데 "문자열일 때" 처리를 어떻게 해야할까 하는 문제였다...
