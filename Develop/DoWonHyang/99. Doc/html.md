# Html

1. sementic tag (header, nav, aside, section)
    - header 문서 도입부에 사용하는태그

    - nav 문서 이동시에 사용하는 태그
        - section elements로 heading태그(h1, h4 등등) 사용 필수

    - main html에서 가장 중요한 부분을 감싸는 태그
        - 하나의 html에서 Main은 1번만 사용 가능
        - section, nav, aside 안에 main은 올 수 없다.
        - sementic elements가 아니므로 heading태그 사용 X

    - section 완벽하게 하나의 기능을 수행할때 사용
        - section elements로 heading태그(h1, h4 등등) 사용 필수

2. Form tag (form 필수 attribute : action(url), method(GET, POST))
    - input
        - type
            - text

            - password

            - file
                - multiple attribute : 파일을 여러개 업로드 할때 사용
                - accept attribute : 받을 파일종류를 정함 (ex) image/png, .jpg, video/* 등등)

    - submit
        - form태그에서 사용하는 버튼

3. list tag (ol, ul, dl)
    - ol 리스트의 순서의 의미가 있을경우 사용하는 태그
        - ol 태그의 자식은 무조건 li태그만 올 수 있다.

    - ul 리스트의 순서의 의미가 없을경우 사용하는 태그
        - ul 태그의 자식은 무조건 li태그만 올 수 있다.
        
    - dl 정의가 필요한 리스트
        - div, dt, dd태그만 올 수 있다.
        - dt 리스트의 제목
        - dd 정의 데이터
        - ex) Naver(dt) 한국의 it 대장주(dd)


4. Media tag (image, audio, video)
    - Media : Text가 아닌 파일을 지칭
        - audio, video Attribute
            - src : audio 파일 경로
            - controls 있어야지 컨트롤이 나온다
            - autoplay 자동재생
            - loop autoplay 무한 자동재생

5. div, span tag
    - div
        - 스타일링을 할때 영역을 그루핑 시 사용 (무분별한 남용 금지) -> 나중에 볼때 어려움
    
    - span
        - 문단내에 특정 부분을 그루핑 시 사용

6. WAI-ARIA
    - 일반사용자가 아닌 다르게 사용하는 사람들을 위해

    - aria-label
        - 시각장애인 등 화면을 볼 수 없는 사람을 위해 있는 태그(스크린 리더기)
        - 전 후 상황 없이 알기 어려운 1, 5시, 5dollar등 부연 설명이 필요한 부분에 작성
        - css처리를 통한 히든으로도 가능