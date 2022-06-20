# Counting sheep...

## Requirement

<p>Consider an array/list of sheep where some sheep may be missing from their place. We need a function that counts the number of sheep present in the array (true means present).</p>

  1. 배열 내의 양(true)의 갯수를 세서 반환하는 함수를 완성해라

## Example

```js
[true,  true,  true,  false,
  true,  true,  true,  true ,
  true,  false, true,  false,
  true,  false, false, true ,
  true,  true,  true,  true ,
  false, false, true,  true] => return 17
```

<br>

### 첫번째 나의 시도

> why? 우선 배열 내에서 `true`만을 가져와야하기 때문에 `filter()`를 사용하였고 나온 결과값의 length로 갯수를 세서 반환한다.

```js
function countSheeps(arrayOfSheep) {
  return arrayOfSheep.filter(item => item === true).length;
}
```

- 결과

![image](https://user-images.githubusercontent.com/96808980/174633224-b666a065-7bbb-4b63-b375-d6bdc9629e5f.png)
