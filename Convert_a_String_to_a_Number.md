# Convert a String to a Number!

## Requirement

<p>We need a function that can transform a string into a number. What ways of achieving this do you know?</p>
<p>Note: Don't worry, all inputs will be strings, and every string is a perfectly valid representation of an integral number.</p>

  1. 문자열을 숫자로 바꾸는 함수를 완성시켜라 

## Example

```js
"1234" => 1234
"605"  --> 605
"1405" --> 1405
"-7" --> -7
```

<br>

### 첫번째 나의 시도

> why? 메서드를 이용해도 되지만 문자열에 `+`만 붙여줘도 숫자형으로 변경할 수 있다.
> 
```js
const stringToNumber = function(str){
  return +str
}
```
- 결과

![image](https://user-images.githubusercontent.com/96808980/173969208-72144533-8e82-4f16-aff7-cbcaa7ac2f59.png)
