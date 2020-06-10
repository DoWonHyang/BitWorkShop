# JavaScript
1. javascript 웹브라우저를 제어하기 위한 언어

2. javascript의 탈브라우저
- serverside script(ex node.js) java, php, python 등등
- clientside script

## JavaScript (언어)

0. type
    - undefined vs null
        - undefined 의도하지 않은, null 의도한
        - undefined == null //true
        - undefined === null //false
    
    - '==' 시 1은 true로 간주 그외 false 간주
        - true == 1 //true

    - Nan 계산할 수 없는
        - Nan === Nan //false

1. 연산자
    - '==', '==='(strict)의 차이
        - 1 == "1" true
        - 1 === "1" false
        - 같은 의미이며 데이터 형식까지 검사
        - 프로그램의 버그를 발생 시킬 가능성이 높기에 '==' 지양, '==='지향한다.

2. 함수(function)
    - 코드의 재사용성을 높이기위하여 사용
    
    - 함수를 정의하는 방법
        - function numbering(){
            document.write(blar);
        }

        - var numbering = function (){
            document.write(blar);
        }

        - (function (){
            document.write(blar);
        })(); -> 익명 함수 : 정의를 하면서 호출하는 경우, 1번만 호출하는 경우 사용