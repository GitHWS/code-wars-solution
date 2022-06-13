# Beginner Series #2 Clock

## Requirement

<p>Clock shows h hours, m minutes and s seconds after midnight. Your task is to write a function which returns the time since midnight in milliseconds.</p>

  1. 시간을 구하는데 시/분/초를 밀리초로 변환한 합계를 구하여라
  2. 입력값은 `0 <= h <= 23`, `0 <= m <= 59`, `0 <= s <= 59`으로 조건을 설정한다.

## Example

```js
h = 0
m = 1
s = 1

result = 61000
```

<br>

### 첫번째 나의 시도

> why? 1초는 `1000ms`이니 s는 `*1000`, m은 60초니까 `*60000`, h는 60분이니 `*3600000`를 곱해서 합계를 내주면 된다!

```js
function past(h, m, s){
  let result = 0;
  if(0 <= s <= 59 && 0 <= m <= 59 && 0 <= h <= 23){
    return result = (s*1000) + (m*60000) + (h*3600000)
  }
}
```
- 결과

![image](https://user-images.githubusercontent.com/96808980/173392903-c6c12199-236c-4a70-9968-149bf66715b9.png)
