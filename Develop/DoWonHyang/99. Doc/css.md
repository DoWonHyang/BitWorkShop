# Css
0. Tip
    - margin, padding은 top or bottom한가지만 사용하는것이 좋다
        - 중구난방 쓰게되면 나중에 헷갈리기에

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

