# RegExp 객체의 정규 표현식
### RegExp.exec() => 추출
```
  var pattern = new RegExp('a');
  pattern.exec('abcd'); // ['a'] => 찾고자 하는 a가 나옴
  pattern.exec('bcd'); // null => 찾고자 하는 a가 없어서 null값이 나옴
```
- 찾는 대상을 배열로 리턴함

### RegExp.test() => 존재 유무 체크
```
  var pattern = new RegExp('a');
  pattern.test('abcd'); // true. a가 있음
  pattern.test('bcd'); // false, a가 없음
```
