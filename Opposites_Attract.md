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

> why? if문으로 2로 나누었을 때 나머지의 값이 같을 경우 짝수나 홀수 결과만 있는 것이니 false, 아니면 true를 출력한다.

```js
function lovefunc(flower1, flower2){
    if(flower1 % 2 === flower2 % 2){
        return false
    }else{
        return true
    }
}
```

```js
function lovefunc(flower1, flower2){
  return flower1 % 2 === flower2 % 2 ? false : true
}
```
- 결과

![image](https://user-images.githubusercontent.com/96808980/174329664-c782f072-b2fd-41be-9ecc-582a88d6dfea.png)

