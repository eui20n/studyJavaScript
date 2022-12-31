# private variable
private variable : 아무나 수정할 수 없게 변수를 숨기는 것
```
  function factory_movie(title){
    return {
      get_title : function (){
        return title;
      },
      set_title : function (_title){
        title = _title;
      }
    }
  }
  ghost = factory_movie('Ghost in the shell');
  matrix = factory_movie('Matrix');
```
- 위의 예시는 getter와 setter라고 생각하면 될듯
- factory_movie(title)에서 title이라는 변수의 값을 숨길 수 있음
