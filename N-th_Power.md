# N-th Power

## Requirement

<p>This kata is from check py.checkio.org

You are given an array with positive numbers and a non-negative number N. You should find the N-th power of the element in the array with the index N. If N is outside of the array, then return -1. Don't forget that the first element has the index 0.

</p>

  1. 숫자 N이 가리키는 배열의 인덱스 `N`번째를 `N`제곱하는 함수를 완성시켜라 
  2. 만약 해당하는 인덱스가 없을 경우 `-1`을 출력한다.
  3. 인덱스는 0부터 시작함을 잊지마라

## Example

```js
array = [1, 2, 3, 4] and N = 2, then the result is 3^2 == 9;
array = [1, 2, 3] and N = 3, but N is outside of the array, so the result is -1.
```

<br>

### 첫번째 나의 시도

> why? 우선 if문으로 요소의 값이 비어있거나 정의되지 않았을 때 `-1`을 반환하게 하고 요소의 값이 존재하면 `array`의 인덱스 `n`를 괄호표기법으로 선택하고 제곱 연산을 해준다.
> 
```js
function index(array, n){
  if(array[n] === undefined || array[n] === null){
    return -1;
  }else{
    return array[n] ** n;
  }
}
```
- 결과

![image](https://user-images.githubusercontent.com/96808980/175064978-5b1a8712-ea07-4713-b386-43f51e0e86cf.png)
