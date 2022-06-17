# Area or Perimeter

## Requirement

<p>You are given the `length` and `width` of a 4-sided polygon. The polygon can either be a rectangle or a square.
If it is a square, return its area. If it is a rectangle, return its perimeter.</p>

  1. 정사각형의 둘레를 구하는 함수를 완성해라.
  2. 함수는 파라미터로 가로길이와 세로길이를 받는다.

## Example

```js
6, 10 --> 32
3, 3 --> 9
```

<br>

### 첫번째 나의 시도

> why? 각 2개씩 가지는 가로와 세로의 합을 구하면 둘레가 나오기 때문에 가로와 세로를 합하고 2를 곱해준다. 그리고 만약 가로와 세로의 길이가 같은 정사각형일 경우 면적을 반환하기 위해 가로와 세로의 값을 곱하고 반환한다.
```js
const areaOrPerimeter = function(l , w) {
  if(l === w){
    return l*w;
  }else{
    return (l + w)*2
  }
};
```
- 결과

![image](https://user-images.githubusercontent.com/96808980/174338557-b4690ebc-7976-4f42-b2de-ba9a5ca86777.png)
