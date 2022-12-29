# 캡처
```
  var pattern = /(\w+)\s(\w+)/; // (문자 공백 문자)를 나타낸 정규식으로 ()는 한 그룹임을 의미하는 것임
  var str = "eui nyun";
  
  var result = str.replace(pattern, "$2, $1"); // $는 그룹을 사용하기 위해서 필요한 것으로, $2는 2번째 그룹, $1은 첫번째 그룹이라서 결과가 아래처럼 나옴
  console.log(result); // nyun, eui

```
- 그룹을 지정 후 활용하는 것을 캡처 라고함
