# 모듈화
```
<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8"/>
				<script type="text/javascript" src="greeting.js">
					// greeting.js의 내용이 여기에 위치하게 됨
				</script>
    </head>
    <body>
        <script>
            alert(welcome()); // greeting.js에 있는 welcome함수를 호출
        </script>
    </body>
</html>
```
- type="text/javascript"는 생략이 가능함
- greeting.js 라는 파일을 읽어서 script사이에 호출하는 것
