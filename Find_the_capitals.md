# Find the capitals

## Requirement

<p>Write a function that takes a single string (`word`) as argument. The function must return an ordered list containing the indexes of all capital letters in the string.

</p>

  1. 문자열에서 대문자만을 찾아 인덱스를 배열에 저장하는 함수를 완성하라

## Example

```js
'CodEWaRs' => [0,3,4,6]
```

<br>

### 첫번째 나의 시도

> why? 우선 대문자의 인덱스를 저장할 빈 배열을 변수로 만들어 놓고 주어진 문자열에서 대문자를 뽑아 `split("")`으로 배열로 만들어서 반복문으로 인덱스번째 요소들을 하나씩 주어진 요소의 인덱스 넘버를 알아내서 빈 배열에 `push()`한다.

```js
var capitals = function (word) {
	let arr = [];
  let upperCases = word.replace(/[a-z]/g, '').split("");
  
  for(let i = 0; i < upperCases.length; i++){
    arr.push(word.indexOf(upperCases[i]));
  }  
  return arr;
};
```
- 결과
![image](https://user-images.githubusercontent.com/96808980/175563423-9c350b15-52ec-45dc-a277-b47478b1d3ca.png)
