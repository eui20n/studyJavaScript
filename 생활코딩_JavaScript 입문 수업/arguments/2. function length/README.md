# function length
매개변수의 수를 알기
- arguments.length : 실제로 어떠한 함수로 유입된 인자가 몇개인지 알려주는 것, 실제로 정의한 매개변수가 몇개인지는 알 수 없음
- 함수명.length : 함수가 정의한 매개변수의 숫자
```
  function zero(){
    console.log(
      'zero.length', zero.length,
      'arguments', arguments.length
    )
  }
  zero(); // zero.length 0, arguments 0

  function one(arg){
    console.log(
      'one.length', one.length,
      'arguments', arguments.length
    )
  }
  one('var1', 'var2'); // one.length 1, arguments 2
```
