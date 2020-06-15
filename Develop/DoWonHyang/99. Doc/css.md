# Css
0. Tip
    - margin, padding은 top or bottom한가지만 사용하는것이 좋다
        - 중구난방 쓰게되면 나중에 헷갈리기에

    - box-sizing : border-box; (테두리까지 박스 크기에 포함)

    - image display: block; 처리 (이미지 태그는 유일하게 inline태그이면서 width값을 조절 혼란을 막기위해 사용)

1. display (Block, inline, inline Block)
    - Block
        - 영역 표시 (width, height, margin, padding 사용가능)
        - 영역 마지막에는 margin으로 채워진다.

    - lnline
        - 흐름 (width, height, margin, padding 등 사용 불가)
        - block과 다르게 inline이 끝난 후 바로 다음 내용이 표시
    
    - inline block
        - 짬뽕과 같은 존재 둘다 혼합되어있음

2. float
    - 가로배치를 위한 property
    - float 시 display block으로 변화
    - float 시 부모요소가 찾지 못하기 때문에 레이아웃이 망가진다( float 시 레이아웃이 붕뜬다 생각하면될듯 )
    - How to fix (overflow:hidden, clearfix)
        - overflow:hidden 그냥 된다.
        - clear 
            - property 사용 시 자식요소가 float된 영역을 인지하여 부모요소의 레이아웃이 망가지지않는다.
            - clear에서 content를 이용하며, 의미없는 태그를 넣기보다는 css가상요소로 레이아웃이 망가지지 않게둔다.
                - pseudo (::before, ::after) clear: left, display:block 설정과 content: ''이 필수

3. position
    - 요소를 원하는 위치에 이동시키기위헤

    - type(static, relative, absolute, fixed) -> 기준점(top, right, left, bottom)

    - static ( 기본값 )
    
    - relative ( float 처럼 붕 뜨지만 위치는 기억 ) -> 다른 요소에 영향을 주지않음
        - top 20px (위를 기준으로 옮김), right 20px(오른쪽을 기준으로 옮김)

    - absolute ( float랑 비슷 )
        - 천상천하 유아독존

        - display : block이지만 길은 막지는 못함

        - position이 static이 아닌 요소가 자기의 기준점이됨 (보통 relative를 기준으로 삼는게 좋다)
 
    - fixed (absolute랑 비슷) 차이는 fixed는 기준이 viewport(보고 있는 브라우저창)

    - 기준점은 right, left중 하나 top, bottom중 하나만 쓰는게 좋다

    - z-index (포지션 수직방향으로 레벨) 1이 아래 100이 위