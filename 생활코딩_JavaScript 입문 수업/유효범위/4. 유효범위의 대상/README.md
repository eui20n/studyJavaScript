# 유효범위의 대상
자바 스크립트는 함수에 대한 유효범위만을 제공함
```
  // case JavaScript
  for(var i = 0; i < 1; i++){
    var name = "Hello World";
  }
  console.log(name); // Hello World => for문 안에서 선언했지만, 밖에서도 사용 가능
```

```
  // case Java
  for(int i = 0; i < 1; i++){
    String name = "Hello World";
  }
  System.out.println(name); // 에러 발생, name이라는 변수가 정의가 안됨
```
