# Traffic light

## Requirement

<p>You're writing code to control your town's traffic lights. You need a function to handle each change from `green`, to `yellow`, to `red`, and then to `green` again.

Complete the function that takes a string as an argument representing the current state of the light and returns a string representing the state the light should change to.

For example, when the input is `green`, output should be `yellow`.</p>

  1. 신호등 표현한 함수를 완성하라 
  2. 초록색이면 노란색, 노란색이면 빨간색, 빨간색이면 다시 초록색 출력하게 하라

## Example

```js
"green" => "yellow"
"yellow" => "red"
"red" => "green"
```

<br>

### 첫번째 나의 시도

> why? 매개변수 `current`가 조건식에 맞게 작성해서 결과를 반환한다.
> 
```js
function updateLight(current) {
  if(current === "green"){
    return "yellow";
  }else if(current === "yellow"){
    return "red";
  }else if(current === "red"){
    return "green"
  }
}
```
- 결과

![image](https://user-images.githubusercontent.com/96808980/175559318-61210756-e57a-4fb7-9a86-8269cd5be3a5.png)
