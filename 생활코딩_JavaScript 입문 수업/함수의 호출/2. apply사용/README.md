# apply 사용
```
  o1 = {val1 : 1, val2 : 2, val3 : 3}
  o2 = {v1 : 10, v2 : 50, v3 : 100, v4 : 25}
  function sum(){
    var _sum = 0;
    for(name in this){
      _sum += this[name];
    }
    return _sum;
  }
  console.log(sum.apply(o1)); // 6
  console.log(sum.apply(o2)); // 185
```
- this는 호출할 때 정해짐 => apply가 결정을 해줌
- 여기서 apply함수의 인자의 값이 this가 되는 것
