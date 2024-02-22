## 개인 프로젝트: 블로그
#### 개관
|제목|내용|
|----|----|
|프로젝트명|블로그 페이지 만들기|
|프로젝트에 대한 설명|개인 블로그를 만들 수 있는 페이지를 제작|
|프로젝트 기간 및 규모|2023-11-27 ~ 2023-12-03 (7일) <br> 1명|
|프로젝트 개발 이슈|초기 개발시 계정별로 분리해두지 않아 나중에 분리할 수 있게 하며 코드를 대량 수정해야 했다|
|프로젝트 결과물·성과|[블로그 레포지토리](https://github.com/portk/blog)|
||![blog_login](https://github.com/portk/portfolio/blob/main/images/blog_login.png)|
||![blog_register](https://github.com/portk/portfolio/blob/main/images/blog_login.png)|
||![blog](https://github.com/portk/portfolio/blob/main/images/blog.png)|

#### 구체사항
|항목|내용|
|----|----|
|프로젝트에서 구현한 기능|로그인, 로그아웃, 계정별 페이지, 회원가입, 회원탈퇴, 게시판 생성, 게시글 작성, 파일 업로드, 댓글 작성, 대댓글 작성|
|프로젝트에서 사용한 기술스택|REST API, React, Spring Boots 3|
|해당 기술 스택을 사용한 이유|React : 자바스크립트 프레임워크로 싱글페이지 어플리케이션을 구축하기 위해 선정하였습니다 <br> Spring Boot 3 : 자바 프레임워크로 DB와 통신하며 REST API를 구축하기 위해 선정하였습니다.|
|성과|REST-API를 통한 백과 프론트 통신 성공<br>useParams 훅을 통한 계정별 페이지 분리|
|보완점|분리 과정중 발생한 페이지 오류 재확인 및 수정<br>업로드된 파일 정보에 대한 DB 테이블의 외래키 문제로 발생한 파일 업로드의 난해한 과정 수정<br>로그인 방식에 대한 수정|
|프로젝트를 수행하며 성장한점 및 느낀점|REST-API를 구성하고 사용할 수 있게 되었다.<br>파라미터를 다양한 곳에서 받아서 사용할 수 있게 되었다.<br>React의 Router기능을 원활하게 사용할 수 있게 되었다.|
