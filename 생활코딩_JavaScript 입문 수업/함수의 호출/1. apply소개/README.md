# apply소개
함수를 호출하는 새로운 특별한 방법
### 기본적인 호출
```
  function func(){
  
  }
  func(); // 함수명으로 호출하면 됨
```

### 특별한 방법(apply)
```
  function sum(arg1, arg2){
    return arg1 + arg2;
  }
  console.log(sum.apply(null, [1, 2]));
```
- 함수는 메소드를 가지고 있음, 여기서 apply는 메소드임
