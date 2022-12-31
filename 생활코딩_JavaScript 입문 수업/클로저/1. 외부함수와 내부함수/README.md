# 외부함수와 내부함수
클로저(closure) : 내부함수가 외부함수의 맥락(context)에 접근할 수 있는 것   
<br>

## 내부함수와 외부함수
```
  function outter(){
    function inner(){
      var title = 'Hello world';
      console.log(title);
    }
    inner();
  }
  outter();
```
- inner는 내부함수이고 outter는 외부함수임
<br>
위의 코드를 다르게 쓰면 아래와 같음
```
  function outter(){
    var inner = function (){
      var title = 'Hello world';
      console.log(title);
    }
    inner();
  }
  outter();
```
- inner를 변수로 할 수 있음

## 클로저
```
  function outter(){
    var title = 'Hello world';
    function inner(){
      console.log(title); // 외부함수의 변수를 호출함
    }
    inner();
  }
  outter();
```
- 내부함수가 외부함수의 변수로 접근했음 => 클로저

