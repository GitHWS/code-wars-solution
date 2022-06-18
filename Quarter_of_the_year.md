# Quarter of the year

## Requirement

<p>Given a month as an integer from 1 to 12, return to which quarter of the year it belongs as an integer number.</p>

  1. 주어진 1~12까지 "월"을 의미하는 정수가 있다.
  2. 주어진 정수를 통해 분기를 반환하는 함수를 완성하라
  3. 

## Example

```js
2 => 1
6 => 2
11 => 4
```

<br>

### 첫번째 나의 시도

> why? 우선 입력 시 month에 들어갈 숫자가 0보다 큰 정수여야 함으로 1차적으로 if문을 사용했고, 비교연산을 통해 범위를 정해줘서 각 분기를 반환했다.

```js
const quarterOf = (month) => {
  if(month > 0){
    if(month <= 3){
      return 1;
    }else if(month <= 6 && month > 3){
      return 2;
    }else if(month <= 9 && month > 6){
      return 3;
    }else{
      return 4;
    }
  }
}
```

- 결과

![image](https://user-images.githubusercontent.com/96808980/174444916-3f8d6120-1e3b-4cb9-96c1-9185146f50c8.png)
