# Opposites Attract

## Requirement

<p>Timmy & Sarah think they are in love, but around where they live, they will only know once they pick a flower each. If one of the flowers has an even number of petals and the other has an odd number of petals it means they are in love.

Write a function that will take the number of petals of each flower and return true if they are in love and false if they aren't.</p>

  1. flower1/flower2가 짝수, 홀수가 쌍으로 나오면 true를 반환하고
  2. 아니면 false를 반환한다.

## Example

```js
lovefunc(1,4) => true
lovefunc(2,2) => false
lovefunc(0,1) => true
lovefunc(0,0) => false
```

<br>

### 첫번째 나의 시도

> why? if문으로 우선 두개 중 하나만 홀수나 짝수가 되면 나머지 하나가 다른 것이 나오면 되기 때문에 처음에 짝수가 있는지 OR문으로 확인하고 있으면 다음 if문에서 홀수를 찾아 있다면 true를 반환하고 아니면 false를 반환한다.

```js
function lovefunc(flower1, flower2){
  if(flower1 % 2 === 0 || flower2 % 2 ===0){
    if(flower1 % 2 !== 0 || flower2 % 2 !== 0){
      return true
    }else{
      return false
    }
  }
}
```
- 결과

![image](https://user-images.githubusercontent.com/96808980/174328376-981b1571-a530-4d8d-8a29-338f64121db8.png)

