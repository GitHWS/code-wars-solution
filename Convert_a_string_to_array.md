# Convert a string to an array

## Requirement

<p>Write a function to split a string and convert it into an array of words.</p>

  1. 문자열을 분해하여 배열로 만들어라

## Example

```js
"Robin Singh" ==> ["Robin", "Singh"]

"I love arrays they are my favorite" ==> ["I", "love", "arrays", "they", "are", "my", "favorite"]
```

<br>

### 첫번째 나의 시도

> why? 문자열을 배열로 바꿀 때는 `split()`을 사용하면 된다! 구분자를 `" "`으로 하면 `" "`을 배열의 ","로 바꿔서 배열로 형변환한다.
> 
```js
function stringToArray(string){
  return string.split(" ")
}
```
- 결과

> why? 정답!

![image](https://user-images.githubusercontent.com/96808980/172503969-a04c18f6-94ec-4502-8308-8f8b9c9200b3.png)
