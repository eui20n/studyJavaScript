# 전역 변수와 지역 변수
유효범위(scope) - 변수의 수명
```
  // version 1.
  var vscope = 'global';
  function fscope(){
    alert(vscope);
  }
  fscope(); // global
```
```
  // version 2.
  var vscope = 'global';
  function fscope(){
    var vscope = 'local';
    alert(vscope);
  }
  fscope(); // local
```
```
  // version 3.
  var vscope = 'global'; // 전역 변수
  function fscope(){
    var vscope = 'local'; // 지역 변수
  }
  fscope();
  alert(vscope); // global
```
```
  // version 4. 
  var vscope = 'global';
  function fscope(){
    vscope = 'local'; // 전역변수인 vscope을 바꾼 것
  }
  fscope();
  alert(vscope); // local
```
```
  // version 5.
  var vscope = 'global'; // 전역 변수
  function fscope(){
    var vscope = 'local'; // 전역 변수
    vscope = 'local change'; // 바로 위가 바뀜
  }
  fscope();
  alert(vscope); // global
```
- var를 써서 정의한 변수는 전역변수가 됨
  - 근데 만약에 해당 변수이름과 같은 지역변수가 있으면 지역변수가 바뀜
  - 쉽게 이해하는 것은 선언을 한 곳을 기준으로 전역변수가 된다고 생각하면 될 듯
