[마크다운 작성법](https://post.naver.com/viewer/postView.nhn?volumeNo=24627214)

HTML
==========
Semantic Web
-----------
- 의미론 적 웹으로, SEO에 도움이 된다.
- 대표적인 시맨틱 요소들
    - hearder
    - nav
    - aside
    - section
    - article
    - footer
    - h#, strong, em  

meta tag
-----------
- meta tag : escription, keywords, author, 기타 메타데이터 정의에 사용된다.  메타데이터는 브라우저, 검색엔진(keywords) 등에 의해 사용된다.
    - <meta name="keywords" content="HTML, CSS, XML, XHTML, JavaScript"> : SEO key keywords
    - <meta name="description" content="Web tutorials on HTML and CSS"> : 웹페이지 설명
    - <meta http-equiv="refresh" content="30"> : 웹페이지를 30초마다 refresh

a tag
-----------
- target 속성의 값
    - target="\_self" : 현재 윈도우에서 링크를 연다(default).
    - target="\_blank" : 새로운 윈도우 혹은 탭에서 링크를 연다.

form tag
-------------
- 대표적인 attribute
    - action : url을 값으로 받으며, form data가 전송된다.
    - method : get 혹은 post를 값으로 받으며, form data의 전달 방식을 지정한다.
        * get : data를 전송 url에 쿼리스트링으로 보낸다. 보안에 취약
        * post : 전송 데이터가 url에 노출되지 않지만 느리다.

- form tag 내에 존재하는 input tag
- type에 따라, 모양이 달라진다.
- name 값을 attribute key, value 값을 attribute value로 하여 key=value 형태로 전송된다.

''' html
<form action="http://~" method="get">
    <input type="" name="" value="">
</form>
'''

(출처: https://poiemaweb.com)[https://poiemaweb.com]


Django
==========
1. 프로젝트 생성 후 최초 migrate
2. 앱 생성
3. 모델 작성 및 makemigrations, migrate  
(settings.py에 생성 앱 추가)
