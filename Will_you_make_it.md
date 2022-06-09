# Will you make it?

## Requirement

<p>You were camping with your friends far away from home, but when it's time to go back, you realize that your fuel is running out and the nearest pump is 50 miles away! You know that on average, your car runs on about 25 miles per gallon. There are 2 gallons left. Considering these factors, write a function that tells you if it is possible to get to the pump or not. Function should return true (1 in Prolog, NASM and COBOL) if it is possible and false (0 in Prolog, NASM and COBOL) if not. The input values are always positive.</p>

  1. 펌프에 갈 수 있다면 `true`, 갈 수 없다면 `false`를 반환해라

## Example

펌프까지의 거리는 `50`마일이 남았고 연료 `1`갤런당 `25`마일을 갈 수 있다. 현재 `2`갤런을 가지고 있다. 

```js
남은거리 50 -> 1마일당 25마일, 남은 갤런 2
```

<br>

### 첫번째 나의 시도

> why? 현재 가지고 있는 2갤런과 1갤런 당 갈 수 있는 거리가 25마일이기 때문에 이 둘을 곱해서 펌프까지 남은 거리와 비교해서 크다면 true, 작다면 false를 반환하면 될 것 같다.
> 
```js
const zeroFuel = (distanceToPump, mpg, fuelLeft) => {
  // TODO
  if(distanceToPump <= mpg * fuelLeft){
    return true;
  }else{
    return false;
  }
};
```
- 결과

> why? 성공! 실질적으로 내용은 같으나 다른 풀이도 있어서 한번 봐야겠다!

![스크린샷 2022-06-09 오전 9 12 52](https://user-images.githubusercontent.com/96808980/172739467-b9662268-f893-4e0b-a054-709f9a7fcb04.png)
