# 콜백
```
  numbers = [20, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1];
  function sortNumber(a, b){
    return a - b;
  }
  console.log(number.sort()); // 1 10 2 20 3 4 5 6 7 8 9 => 문자 처럼 정렬이 됨
  
  // sort라는 메소드는 매개변수로 함수값을 넣을 수 있음
  console.log(number.sort(sortNumber)); // 1 2 3 4 5 6 7 8 9 10 20
```
- numbers.sort(sortNumber)에 있는 sortNumber가 콜백함수
- 즉, 값으로서 함수를 전달받을 수 있어서, 이 콜백함수 가지고 원래 함수가 가진 수행 방식을 완전히 바꿀 수 있음
