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
    - \<meta name="keywords" content="HTML, CSS, XML, XHTML, JavaScript"\> : SEO keywords
    - \<meta name="description" content="Web tutorials on HTML and CSS"\> : 웹페이지 설명
    - \<meta http-equiv="refresh" content="30"\> : 웹페이지를 30초마다 refresh

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

```html  
<form action="http://~" method="get">
    <input type="" name="" value="">
</form>
```

html 내용 출처는 https://poiemaweb.com 입니다.


Django
==========
1. 프로젝트 생성 후 최초 migrate
2. 앱 생성
3. models.py 작성 및 makemigrations, migrate  
(settings.py에 생성 앱 추가)
4. shell에서 확인해보기 (from posts.models import Post)
5. superuser 생성 및 admin.py에 Post 등록
6. admin page 커스터마이징
7. urls.py -> views.py -> html 흐름 생성
8. lovely app 추가 및 settings.py에 등록
9. project의 url.py 수정, app의 views, templates 생성 및 수정
10. include로 urls 분산화(lovely app 내 urls.py 생성, 작성)
11. main.html에 링크 생성
12. urls.py에 name 지정, main.html 링크 수정
13. urls.py에 app_name 지정, main.html 링크 재수정
14. settings.py에 templates의 경로를 추가
15. MyFirstDjango/templates/에 base.html 생성
16. base.html에 bootstrap cdn으로 복사
17. base.html에 templaes 태그 추가({% block content %}등)
18. main.html, first.html 등에 연결 ({% extends 'base.html' %})
19. settings.py에 STATICFILES_DIRS 추가
20. MyFirstDjango에 static 폴더를 비롯한 하위 폴더 및 파일 생성
21. base.html에 {% load static %} 과 <link rel="stylesheet" href="{% static 'css/project.css' %}"> 추가
22. project.css에 시험 할 style 추가
23. project의 templates/share/에 \_navbar.html 생성 (이름 무관)
24. 재사용할 코드, html에 {% include 'share/\_navbar.html' %}로 호출
25. 정적파일 이미지 삽입하기 {% load static %}, <img src="{% static 'img/gejang.jpg' %}" alt="간장게장">
