# SPACE COUNTER 만들기
아주 간단한 내용이지만 조금 독특한 것을 만들어보고 싶어서 제작하게 되었습니다.    

## onClick이벤트
html에서 작성 시 직접 Click이벤트를 부여할 수 있습니다.     
또는 javascript에서 작성 시에는 DOM에 접근해서 이벤트를 부여할 수 있습니다.     
```html
<button onClick="reset()">RESET</Button>
```
```javascript
const resetBtn = document.querySelector('button');
resetBtn.addEventListener('click',함수)
```

## document의 키보드 메소드
키 메소드를 통해서 문서에서 이벤트를 발생시킬 수 있습니다.     
스페이스의 keycode는 32번입니다.      
일치하면 카운터 변수의 값을 증가시키고 textContent를 통해 값을 전달시킵니다.     

### onkeydown : 키를 눌렀을 때 발생하는 이벤트
### onkeypress : 키를 누르고 있는 동안 발생하는 이벤트
### onkeyup : 키를 눌렀다 놓았을 때 발생하는 이벤트
