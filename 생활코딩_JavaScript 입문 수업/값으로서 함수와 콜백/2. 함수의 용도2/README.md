# 함수의 용도2
함수는 함수의 리턴값으로도 사용할 수 있음
```
  function cal(mode){
    var funcs = {
      'plus' : function(left, right) {return left + right},
      'minus' : function(left, right) {return left - right}
    }
    return funcs[mode];
  }
  console.log(cal('plus')(2, 1)); // 3
  // cal('plus') 바로 리턴값을 만남 => funcs['plus']
  // funcs['plus']는 메소드임, 즉 cal('plus')가 funcs['plus']가 됨
  // cal('plus')(2, 1)은 funcs['plus'](2, 1)이 되어서 3이 반환됨
```
<br>
배열의 값으로도 함수를 사용할 수 있음   
<br>
이런식으로 변수, 매개변수, 리턴값으로 사용될 수 있는 것을 first-class citizen(object, value)라고 부름
