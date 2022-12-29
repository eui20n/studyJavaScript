# 객체지향 프로그래밍
서로 연관이 있는 것들을 묶은 것을 객체지향 프로그래밍이라고 함   
객체 안에 또 객체가 들어갈 수 있음
* 예시
```
  // 정의
  var grade = {
    'list' : {'kim' : 10, 'eui' : 20, 'nyun' : 30},
    'show' : function(){
      alert('Hello world'); // 함수도 객체로 들어올 수 있음
      alert(this) // this는 함수가 속해있는 객체를 가르키는 변수로, 여기서는 grade를 가르킴
    }
  }
  
  // 호출
  grade['list']; // {'kim' : 10, 'eui' : 20, 'nyun' : 30}
  grade['list']['kim']; // 10
  grade['show'](); // Hello world
```
