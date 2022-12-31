# arguments란
함수 안에서 함수의 여러가지 정보(특히 인자)를 담고 있는 객체, 배열과 비슷해서 유사 배열이라고 함
```
  function sum(){
    var i, _sum = 0;
    for(i = 0; i < arguments.length; i++){
      document.write(i + ' : ' + arguments[i] + '<br />');
      _sum += arguments[i]
    }
    return _sum;
  }
  document.write('result : ' + sum(1, 2, ,3, 4));
```
- sum이라는 함수에 매개변수는 없지만, sum(1, 2, 3, 4)처럼 호출을 해도 상관이 없음
  - 자바 스크립트는 굉장히 관대한 언어라서 그럼
- arguments에는 사용자가 전달한 인자가 들어가 있음
  - 즉, 위의 경우에는 arguments에 [1, 2, 3, 4]가 들어가 있음
