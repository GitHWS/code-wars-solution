# Is he gonna survive?

## Requirement

<p>A hero is on his way to the castle to complete his mission. However, he's been told that the castle is surrounded with a couple of powerful dragons! each dragon takes 2 bullets to be defeated, our hero has no idea how many bullets he should carry.. Assuming he's gonna grab a specific given number of bullets and move forward to fight another specific given number of dragons, will he survive?</p>

  1. 용은 2발의 총알로 한마리를 잡을 수 있다.
  2. 용사가 가지고 있는 총알로 모든 용을 잡을 수 있는지 계산하는 함수를 완성하라

## Example

```js
bullets 10, dragons 5 => true
bullets 7, dragons 4 => false
```

<br>

### 첫번째 나의 시도

> why? 영웅이 가지고 있는 총알의 수가 용의 숫자의 2배보다 많으면 true를 반환하고 아니라면 false를 반환하는 삼항연산자를 만들었다.

```js
function hero(bullets, dragons){
  return bullets >= dragons * 2 ? true : false
}
```

- 결과

![스크린샷 2022-06-21 오전 12 11 28](https://user-images.githubusercontent.com/96808980/174632193-4976c829-a5c2-4679-b69a-b4c6727e786e.png)
