# 객체의 문법
배열과 유사한 역할을 함   
차이점은 객체는 인덱스를 문자와 같은 것으로 만들 수 있음   
다른 언어에서의 객체는 연관 배열, 맵, 딕셔너리가 있음   
```
  // 정의 1.
  var objectName = {key1 : value1, key2 : value2, ...}
  
  // 정의 2.
  var objectName = new Object();
  objectName[key1] = value1;
  objectName[key2] = value2;
  ...
  
  // 호출 1.
  objectName[key1]; // value1
  
  // 호출 2.
  objectName.key1; // value1

```
