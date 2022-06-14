# Shortest Word

## Requirement

<p>Simple, given a string of words, return the length of the shortest word(s). String will never be empty and you do not need to account for different data types.</p>

  1. 단어로 이루어진 문자열에서 가장 짧은 단어의 길이를 반환하라
  2. 문자열은 절대 비어있지 않으며 다른 타입을 신경쓸 필요가 없다.

## Example

```js
"bitcoin take over the world maybe who knows perhaps" => 3
"turns out random test cases are easier than writing out basic ones" => 3
"Let's travel abroad shall we" => 2
```

<br>

### 첫번째 나의 시도

> why? 각 단어마다 길이를 비교해야하기 때문에 `split(" ")`으로 단어를 요소로 가지는 배열로 만들고 각 요소의 길이를 구한다. 그리고 `Math.min()`을 사용하여 최소값을 구해서 리턴한다.
> 주의할 점은 `Math.min()`의 인자로 배열이 들어가선 안되고 전개구문으로 풀어줘야 된다.
```js
function findShort(s){
    const arr = s.split(" ").map(item => item.length);
    const min = Math.min(...arr);
    return min
}
```
- 결과

![image](https://user-images.githubusercontent.com/96808980/173576225-37018aef-e3d7-4c64-9605-cdbc63f7a2dd.png)
