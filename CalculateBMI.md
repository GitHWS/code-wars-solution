# Calculate BMI

## Requirement

<p>Write function bmi that calculates body mass index `(bmi = weight / height^2)`.</p>

  1. BMI지수를 계산하는 함수를 만들어라
  2. bmi = weight / height^2

## Example

```js
if bmi <= 18.5 return "Underweight"

if bmi <= 25.0 return "Normal"

if bmi <= 30.0 return "Overweight"

if bmi > 30 return "Obese"
```

<br>

### 첫번째 나의 시도

> why? BMI 지수를 계산한 값을 변수에 할당하고 그것을 주어진 범위와 일치하는지 비교를 하여 각 범위마다 반환할 문자열을 설정한다.
> 
```js
function bmi(weight, height) {
  let BMI = (weight) / (height * height)
  if(BMI <= 18.5){
    return "Underweight"
  }
  
  if(BMI <= 25.0){
    return "Normal"
  }
  
  if(BMI <= 30.0){
    return "Overweight"
  }
  
  if(BMI > 30){
    return "Obese"
  }
}
```
- 결과

![image](https://user-images.githubusercontent.com/96808980/173884831-27b1d667-7bfb-4394-b67f-a267f153d6ae.png)
