# Remove First and Last Character

## Requirement

<p>It's pretty straightforward. Your goal is to create a function that removes the first and last characters of a string. You're given one parameter, the original string. You don't have to worry with strings with less than two characters.</p>

  1. 문자열의 맨 앞/뒤 글자를 지워서 결과를 출력하라

## Example

```js
없음
```

<br>

### 첫번째 나의 시도

> why? 문자열 메서드인 `substring()`이나 `slice()`를 사용하여 맨 앞/뒤의 글자를 잘라줄 수 있을 것 같아 작성한 방법이다.

```js
function removeChar(str){
 return str.slice(0, 1).slice(0, str.length);
};

removeChar("hello") // "h"
```
- 결과

> why? `substring()`이나 `slice()` 메서드는 "잘린 부분"만 반환하고 체이닝을 통해 사용했지만 맨 앞 글자만 적용이 되었다..😅
> 
![image](https://user-images.githubusercontent.com/96808980/172214370-bfdda687-c1ea-4b4a-9887-30638744fda7.png)



### 두번째 나의 시도

> why? 나머지 부분을 반환하기 위해 맨 처음의 글자와 마지막 글자를 제외하기 위해 `substing(1, str.length-1)`을 사용했다. 

```js
function removeChar(str){
 return str.substring(1, str.length-1);
};

removeChar("hello") // "ell"
```
- 결과

> why? 나머지 부분을 반환하여 맨 앞과 뒤의 글자가 삭제된 결과를 얻을 수 있었다. 위에서 말한 메서드는 "잘린 부분"을 반환하기 때문에 주의해야한다!

![image](https://user-images.githubusercontent.com/96808980/172213671-f92bff6c-214e-492a-a539-348bd8e18433.png)
