# String 객체의 정규 표현식
### String.match() => RegExp.exec()와 비슷
```
  var pattern = new RegExp('a');
  var str = 'abc';
  str.match(pattern); // ["a"]
  
  var str = 'bcd';
  str.match(pattern); // null
```

### String.replace()
```
  var pattern = new RegExp('a');
  var str = 'abc';
  str.replace(pattern, 'A'); // Abc
```
- 패턴과 일치하는 값을 원하는 값으로 바꿔줌
