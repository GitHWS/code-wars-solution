# Friend or Foe?

## Requirement

<p>Make a program that filters a list of strings and returns a list with only your friends name in it. If a name has exactly 4 letters in it, you can be sure that it has to be a friend of yours! Otherwise, you can be sure he's not...</p>

  1. 이름의 글자 수가 4글자인 친구만 필터링하라

## Example

```js
Input = ["Ryan", "Kieran", "Jason", "Yous"] => Output = ["Ryan", "Yous"]
```

<br>

### 첫번째 나의 시도

> why? 매개변수로 배열을 받기 때문에 `filter()` 메서드를 사용하면 조건에 맞는 요소만 골라서 새로운 배열로 생성해준다. 그리고 `return`을 작성해주는 것을 절대 잊지말자! 
```js
function friend(friends){
  return friends.filter(name => name.length === 4)
}
```
- 결과

> why? 성공! filter의 콜백함수를 넣는 것을 기억하면 쉽게 풀 수 있는 문제였다!

![스크린샷 2022-06-13 오후 10 55 25](https://user-images.githubusercontent.com/96808980/173369805-8402ce92-e1f4-48cd-9b4e-ddda3a255d8f.png)
