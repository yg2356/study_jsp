# 2023-12-27

### 이클립스 깃헙 연동및 jsp 테스트
  
<JAVA SE & JAVA EE 차이><br/>
JAVA SE :  독자적으로 실행되는 애플리케이션 개발 플랫폼<br/>
JAVA EE : JSP, Servlet 개발시 선택되는 플랫폼 & 서버가 필수<br/>

# 2024-01-01
어노테이션 : 컴파일러에 정보를 알려주는 기능, 자바프로그램 실행에 관한 내용을 설장하는 용도

# 2024-01-07
sheme : 사용할 프로토콜
<br>
URI : 문서 고유식별 번호 + URL
URL : 문서종보 & 위치

### WAS& SERVER & 컨테이너
|WAS|Web Application SerVer|클라이언트의 요청을 받은것을 응답받아 처리하는 서버(DB, 로직)|Tomcat|

|Web Server|클라이언트의 요청을 받은것을 응답받아 처리하는 서버(HTML,CSS,JS)|Apache|

※WAS는 웹 서버없이 독립적으로 존재 가능 ==> WAS > 웹서버

클라이언트 -> 웹서버 -> WAS

![1](https://github.com/yg2356/study_jsp/assets/59286004/04bba9fb-af54-4a16-82ae-347a7c5cb423)

컨테이너 : JAVA 서블릿과 상호작용하는 WAS의 구성요소

<img width="410" alt="2" src="https://github.com/yg2356/study_jsp/assets/59286004/5653cc1f-f483-46cb-b383-7daeaea237e3">

# 2024-01-08
GET : 클라이언트가 직접요청하는 파일 요청방식

POST : GET의 부족한 부분 보완 + 질의 문자열 전달 기능 기반의 요청방식

# 2024-01-11
GET요청방식<br>
- 질의문자열 주소 노출
- 헤더에 URI추가
- 질의문자열 길이 제한적
- 인코딩/ 디코딩 없이 처리 빠름
- URI 직접추가가능
  ==> 외부에 노출되는 경우에만 GET 사용

<a>태그 : GET방식으로 동작

? name = value&name=value 방식
![image](https://github.com/yg2356/study_jsp/assets/59286004/2c6dd999-544d-46a6-866b-5d837f4fb18f)

POST 요청방식<br>
-  질의문자열이 몸체에 포함
-  외부에 노출X
-  질의문자열 길이 제한 X
-  <form>태그 사용시에만 요청 가능

![image](https://github.com/yg2356/study_jsp/assets/59286004/a34685cd-b517-413f-86b6-d71cac174467)


결론:

GET = 서버의 데이터를 가져오는 단순 행위 - 선택 & 추출
POST = 서버의 데이터 값 수정이나 상태변화시

ex) GET : 읽기/ POST : 수정 / PUT : 등록 / DELETE : 삭제
