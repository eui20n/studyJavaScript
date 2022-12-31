# 클로저란
내부함수가 외부함수에 접근할 수 있는 것이 클로저임   
근데 외부함수가 더이상 사용하지 않아도 내부함수는 외부함수에 접근할 수 있음
```
  function outter(){
    var title = 'Hello world';
    return function(){
      console.log(title);
    }
  }
  inner = outter();
  inner();
```
- inner는 outter의 반환값을 받음
- outter의 반환값은 함수임 => title을 출력함
- inner가 받은 함수는 title에 대한 정보는 없지만 inner를 호출하면 title이 호출이 됨 => 클로저 때문에 가능
