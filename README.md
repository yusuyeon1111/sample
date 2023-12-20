# 유수연 포트폴리오
>캐치 프레이즈 ( 나를 보여줄 수 있는 한마디 )

</br>

## :pushpin: Intro
- Back-end 개발자를 희망합니다

</br>

## :pushpin: Contact
- 이메일: yusuyeon443@gmail.com
- 깃헙: https://github.com/yusuyeon1111

</br>

## :pushpin: Projects

---

### 1. [핵심 프로젝트](https://github.com/2023-SMHRD-IS-CLOUD-1/1stProject.git)
>HEF  (팀 프로젝트)  
>개발 기간: 2023.11.22 ~ 2020.12.8  
>  
>기술 스택:  
<div align="center">
	<P>🎇platforms & languages </P>
	<img src="https://img.shields.io/badge/Java-007396?style=flat&logo=Java&logoColor=white" />
	<img src="https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=HTML5&logoColor=white" />
	<img src="https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=CSS3&logoColor=white" />
	<img src="https://img.shields.io/badge/oracle-F80000?style=flat&logo=oracle&logoColor=white"/>
	<img src="https://img.shields.io/badge/javascript-F7DF1E?style=flat&logo=javascript&logoColor=white"/>
</div>
<div align="center">
	<P>🔨Tools</P>
	<img src="https://img.shields.io/badge/eclipseide-525C86?style=flat&logo=eclipseide&logoColor=white"/>
	<img src="https://img.shields.io/badge/visualstudiocode-007ACC?style=flat&logo=visualstudiocode&logoColor=white"/>
	<img src="https://img.shields.io/badge/apachetomcat-F8DC75?style=flat&logo=apachetomcat&logoColor=white"/>
	<img src="https://img.shields.io/badge/github-181717?style=flat&logo=github&logoColor=white"/>
	<img src="https://img.shields.io/badge/python-776AB?style=flat&logo=python&logoColor=white"/>
</div>
>  
>[프로젝트 상세 설명](https://github.com/JungHyung2/gitio.io) 참고

---

### 3. [세 번째 프로젝트](https://github.com/JungHyung2/gitio.io)
>세 번째 프로젝트 간략 소개  (개인 프로젝트)  
>개발 기간: 2018.1.18 ~ 2018.4.5  
>  
>기술 스택:  
>Java 8 / Spring Boot / Gradle / Spring Data JPA / QueryDSL  
>H2 / MySQL / Spring Security / Jsoup / Vue.js / Element U  
>  
>[프로젝트 상세 설명]
><details>
<summary><b>핵심 기능 설명 펼치기</b></summary>
<div markdown="1">

### 1. 전체 흐름
(![image](https://github.com/yusuyeon1111/sample/assets/142488306/27c619c8-4cb2-412a-964c-57637b5eb1b3)
1. 의뢰인이 심부름 의뢰글을 작성합니다
2. 의뢰글을 수행인이 심부름 페이지에서 검색해서 조회할 수 있습니다.
3. 수행인이 의뢰글에 수행 신청을 하게되면
4. 의뢰인의 수행인 신청 목록 확인 서비스에서 수행인의 프로필을 확인할 수 있습니다
5. 의뢰인은 수행인의 신청 목록을 확인해 신청을 수락할 수 있고 거절할 수 있습니다.
6. 신청을 수락하게 되면 심부름은 매칭되고 매칭 여부가 데이터베이스 상에서 변화됩니다.

### 4.2. 사용자 요청
![](https://zuminternet.github.io/images/portal/post/2019-04-22-ZUM-Pilot-integer/flow_vue.png)

- **URL 정규식 체크** :pushpin: [코드 확인](https://github.com/Integerous/goQuality/blob/b587bbff4dce02e3bec4f4787151a9b6fa326319/frontend/src/components/PostInput.vue#L67)
  - Vue.js로 렌더링된 화면단에서, 사용자가 등록을 시도한 URL의 모양새를 정규식으로 확인합니다.
  - URL의 모양새가 아닌 경우, 에러 메세지를 띄웁니다.

- **Axios 비동기 요청** :pushpin: [코드 확인]()
  - URL의 모양새인 경우, 컨텐츠를 등록하는 POST 요청을 비동기로 날립니다.

### 4.3. Controller

![](https://zuminternet.github.io/images/portal/post/2019-04-22-ZUM-Pilot-integer/flow_controller.png)

- **요청 처리** :pushpin: [코드 확인](https://github.com/JungHyung2/gitio.io/blob/d35d29b64c0e8b9653862bdcc1e6b997d2436ec9/index.html#L57C1-L57C202)
  - Controller에서는 요청을 화면단에서 넘어온 요청을 받고, Service 계층에 로직 처리를 위임합니다.

- **결과 응답** :pushpin: [코드 확인]()
  - Service 계층에서 넘어온 로직 처리 결과(메세지)를 화면단에 응답해줍니다.

### 4.4. Service

![](https://zuminternet.github.io/images/portal/post/2019-04-22-ZUM-Pilot-integer/flow_service1.png)

- **Http 프로토콜 추가 및 trim()** :pushpin: [코드 확인]()
  - 사용자가 URL 입력 시 Http 프로토콜을 생략하거나 공백을 넣은 경우,  
  올바른 URL이 될 수 있도록 Http 프로토콜을 추가해주고, 공백을 제거해줍니다.

- **URL 접속 확인** :pushpin: [코드 확인]()
  - 화면단에서 모양새만 확인한 URL이 실제 리소스로 연결되는지 HttpUrlConnection으로 테스트합니다.
  - 이 때, 빠른 응답을 위해 Request Method를 GET이 아닌 HEAD를 사용했습니다.
  - (HEAD 메소드는 GET 메소드의 응답 결과의 Body는 가져오지 않고, Header만 확인하기 때문에 GET 메소드에 비해 응답속도가 빠릅니다.)

  ![](https://zuminternet.github.io/images/portal/post/2019-04-22-ZUM-Pilot-integer/flow_service2.png)

- **Jsoup 이미지, 제목 파싱** :pushpin: [코드 확인]()
  - URL 접속 확인결과 유효하면 Jsoup을 사용해서 입력된 URL의 이미지와 제목을 파싱합니다.
  - 이미지는 Open Graphic Tag를 우선적으로 파싱하고, 없을 경우 첫 번째 이미지와 제목을 파싱합니다.
  - 컨텐츠에 이미지가 없을 경우, 미리 설정해둔 기본 이미지를 사용하고, 제목이 없을 경우 생략합니다.


### 4.5. Repository

![](https://zuminternet.github.io/images/portal/post/2019-04-22-ZUM-Pilot-integer/flow_repo.png)

- **컨텐츠 저장** :pushpin: [코드 확인]()
  - URL 유효성 체크와 이미지, 제목 파싱이 끝난 컨텐츠는 DB에 저장합니다.
  - 저장된 컨텐츠는 다시 Repository - Service - Controller를 거쳐 화면단에 송출됩니다.

</div>
</details>
