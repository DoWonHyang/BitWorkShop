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

    - return은 단 한개만 반환

3. 배열(array)
    - return은 1개만 반환 하지만 배열을 이용하여, 연관된 여러 데이터를 반환

    - 배열을 만드는 초기화하는 방법
        - var temp = []; , var temp = [1, 2];

    - 배열 제어
        - push ( 배열의 끝에 원소 추가 ) ex) arr.push(1);

        - concat (여러개의 원소 추가) ex) arr.concat([1, 2]);

        - unshift ( 첫번째 원소로 추가 ) ex) arr.unshift(0);

        - splice ( 배열 사이에 값을 추가 및 사이 값을 추출)

        - shift (첫번째 원소 제거)

        - pop (마지막 원소 제거)

        - sort, reverse (정렬)

4. 객체 (object)
    - 구조적인 프로그램을 구성하기 위하여 중요

    - 객체를 만드는 초기화하는 방법
        - var temp ={};
            - temp['first'] = 1;
            - temp['second'] = 1;

        - var temp = new Object();

        - var temp = {'first' : 1, 'second' : 2};

    - 접근방법
        - temp['first'];

        - temp.first;

    - temp['fir'+'st']; O, temp.'fir'+'st' X


5. 모듈 (module), 라이브러리(library)
    - 프로그램의 재사용성을 높이기 위하여
    
    - 이점 : 가독성, 용량, 트래픽 등등 

    - web browser host(web, node 등등) 환경 -> script src = "app.js"

    - node host 환경 -> temp = require("./app/js");


    