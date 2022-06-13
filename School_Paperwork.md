# Beginner Series #1 School Paperwork

## Requirement

<p>Your classmates asked you to copy some paperwork for them. You know that there are 'n' classmates and the paperwork has 'm' pages.</p>
<p>Your task is to calculate how many blank pages do you need. If `n < 0` or `m < 0` return `0`.</p>

  1. 서류복사를 n명만큼 했을 때 총 몇 페이지가 나오는지 알려주는 함수를 완성시켜라.
  2. 'n'명의 학생들이 있고 서류가 'm'페이지 분량이다.
  3. 만약 학생수나 페이지 수가 음수라면 `0`을 반환한다.

## Example

```js
n= 5, m=5: 25
n=-5, m=5:  0
```

<br>

### 첫번째 나의 시도

> why? 삼항 연산자로 풀면 학생수나 페이지 수 중 하나라도 음수일 때(`n < 0 || m < 0`) `0`을 반환하고 아닐 시 `n*m`의 값을 반환한다.

```js
function paperwork(n, m) {
  return n < 0 || m < 0 ? 0 : n*m
}
```
- 결과

![image](https://user-images.githubusercontent.com/96808980/173387756-e084ac06-a113-4f7d-9d6a-8002d2be17a7.png)
