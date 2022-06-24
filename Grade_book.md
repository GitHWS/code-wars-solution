# Grade book

## Requirement

<p>Complete the function so that it finds the average of the three scores passed to it and returns the letter value associated with that grade.

</p>

  1. 3가지 점수의 평균을 계산해서 범위에 맞는 점수를 반환하라.

## Example

```js
Numerical Score	       Letter Grade
90 <= score <= 100	=> 'A'
80 <= score < 90    => 'B'
70 <= score < 80    => 'C'
60 <= score < 70    => 'D'
0 <= score < 60	    => 'F'
```

<br>

### 첫번째 나의 시도

> why? 평균 점수를 구하는 문제, if문의 조건만 주의하도록 하면 된다. 
> 
```js
function getGrade (s1, s2, s3) {
  let average = (s1 + s2 + s3) / 3
  if(average >= 90 && average <= 100){
    return "A"
  }else if(average >= 80 && average < 90){
    return "B"
  }else if(average >= 70 && average < 80){
    return "C"
  }else if(average >= 60 && average < 70){
    return "D"
  }else{
    return "F"
  }
}
```
- 결과

![image](https://user-images.githubusercontent.com/96808980/175557133-76a0d369-dd38-4033-bd4f-3a18d519d4e4.png)
