# 옵션
### i
- 정규 표현식의 패턴이 대소문자를 구분하게 하거나, 구분하지 않게 하는 것
```
  var pattern = /a/i;
  "Abcd".match(pattern); // ["A"] => 대소문자를 구분하지 않음
```

### g
- 문자열에 패턴에 해당하는 것들을 다 반환하게 하는 것
```
  var pattern = /a/;
  "abcda".match(pattern); // ["a"]
  
  var pattern = /a/g;
  "abcda".match(pattern); // ["a", "a"]
```
<br>
<br>

> 옵션은 중첩이 됨
