# 클로저의 응용
## 클로저를 사용할 때 발생할 수 있는 실수
```
  var arr = [];
  for(var i = 0; i < 5; i++){
    arr[i] = function (){
      return i;
    }
  }
  
  for(var index in arr)(
    console.log(arr[index]());
  )
```
- 이렇게 했을 때, 기대값은 0, 1, 2, 3, 4가 출력되는 것임
- 하지만 실제 출력값은 5, 5, 5, 5, 5임
- 이러한 출력이 나오는 이유는 첫 번째 for문의 i는 외부 변수가 아님 => i의 값은 전역변수라서 결국 5가 되기 때문에 5가 출력되는 것임

<br>

### 해결
```
  var arr = [];
  for(var i = 0; i < 5; i++){
    arr[i] = function(idx){
      return function (){
        return idx;
      }
    }(i);
  }
  for(var index in arr){
    console.log(arr[index]());
  }
```
- 0, 1, 2, 3, 4가 출력됨
