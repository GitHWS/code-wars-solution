# Remove String Spaces

## Requirement

<p>Simple, remove the spaces from the string, then return the resultant string.</p>

  1. 문자열의 공백을 없애고 결과를 반환하라
  2. 
  3. 

## Example

```js
'8 j 8   mBliB8g  imjB8B8  jl  B' => '8j8mBliB8gimjB8B8jlB'
```

<br>

### 첫번째 나의 시도

> why? `split(" ")`로 공백을 기준으로 나누어 배열로 만들고 `join("")`로 합쳐서 문자열로 반환한다.
```js
function noSpace(x){
  return x.split(" ").join("");
}
```
- 결과

![image](https://user-images.githubusercontent.com/96808980/174445736-ebaafe5c-00c9-4126-acc2-9a9c08007383.png)
