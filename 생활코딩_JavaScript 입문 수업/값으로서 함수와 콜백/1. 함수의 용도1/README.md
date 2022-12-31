# 함수의 용도1
함수도 객체임 => 함수도 하나의 값이라고 생각하면 됨   
즉, 함수를 변수에 담을 수 있음 => 다른 언어와 차이점   
객체의 속성 값으로 담겨진 함수를 메소드라고 함   
```
  a = {
    b : function (){
    }
  }; // b의 value를 method라고 함
```
<br>
값이라서 인자로 전달이 가능함

```
  function cal(func, num){
    return func(num);
  }
  
  function increase(num){
    return num + 1;
  }
  
  console.log(cal(increase, 1)); // 2
  // cal의 매개변수 func에 함수 increase가 들어가고, num에 1이 들어감
  // 그럼 cal의 리턴값인 fun(num)에 increase(1)이라는 함수를 호출하는 것이 됨
  // 2가 출력됨
```
