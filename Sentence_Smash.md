# Sentence Smash

## Requirement

Write a function that takes an array of words and smashes them together into a sentence and returns the sentence. You can ignore any need to sanitize words or add punctuation, but you should add spaces between each word. Be careful, there shouldn't be a space at the beginning or the end of the sentence!

  1. 함수에 배열을 매개변수로 넣었을 때 한 문장으로 뭉쳐줄 것
  2. 각 단어 사이 공백을 추가할 것
  3. 문장의 시작이나 끝에 공백이 없을 것

## Example

```js
['hello', 'world', 'this', 'is', 'great']  =>  'hello world this is great'
```

<br>

### 첫번째 나의 시도

> 내 생각 : 배열 메서드인 `join(",")`으로 배열의 형태 그대로 문자열로 형변환하고 `replaceAll(",", " ")` 메서드를 이용하여 ","를 빈 공백인 " "로 바꿔주면 되지않을까?

```js
function smash (words) {
   return words.join(",").replaceAll(",", " ");
};

smash([]); // ''
smash(['hello', 'world', 'this', 'is', 'great']); // 'hello world this is great'
```

- 결과

> why? 결과는 맞는데 왜 안되는걸까..? 혹시 응답속도 때문인가..

![image](https://user-images.githubusercontent.com/96808980/172203023-232bab90-6006-42fd-b0de-64992118d7dc.png)


### 두번째 나의 시도

> 내 생각 : 앞에서 했던 `join(",")`를 `join(' ')`으로 바꿔주면 간단한 것이였다.. 굳이 `replaceAll(",", " ")`를 사용할 필요가 없었다..😅

```js
function smash (words) {
   return words.join(" ")
};

smash([]); // ''
smash(['hello', 'world', 'this', 'is', 'great']); // 'hello world this is great'
```

- 결과

> why? 왜 심지어 더 느린데 왜 정답일까..? 🤔

![image](https://user-images.githubusercontent.com/96808980/172204722-0edbea99-dd36-421e-9787-c995de094a0a.png)
