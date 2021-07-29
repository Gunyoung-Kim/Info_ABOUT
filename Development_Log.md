# Info

## 개발일지

### 2021.5.26

1. 프로젝트 설계
 
2. 데이터베이스 테이블 설계
 
3. domain package 완성
 
4. mysql 연결 코드 완성 

### 2021.5.27

1. Domain 유효성 검증 및 검증 메시지 관련 코드 추가

2. 각 종 Controller 구현
   
   - 메인 뷰, 로그인 뷰, 회워 가입 뷰 전용 Controller
   - 모든 회원 정보 가져오는 RestController

3. Domain 관련 Repository, Service 구현 

4. 메인 뷰, 로그인 뷰, 회원 가입 뷰 템플릿 생성
 
### 2021.5.28

1. Security Config, SecurityAuthenticationFilter, UserDetails, UserDetailsService 구현

2. 비밀 번호 암호화로 DB 저장

3. Content 도메인 추가 및 Content Repository, Service 구현

### 2021.5.30

1. 포트폴리오 전용 뷰 생성, 포트폴리오 전용 뷰 컨트롤러 생성

2. Spring Security와 thymeleaf extras Spring Security 를 이용한 로그인, 로그아웃 구현

### 2021.5.31

1. 프로필 수정 뷰 및 관련 뷰 컨트롤러 구현

2. 프로젝트 생성 뷰 및 관련 뷰 컨트롤러 구현

3. Space 엔티티에 필드(SNS 주소, Description) 추가

4. 프로젝트 열람 뷰 구현

### 2021.6.1

1. AuthenticationProvider 추가

2. 개인 정보 수정 URL 변경 ( 기존: url에 해당 email 노출, 해당 email 사용 -> 현재: SecurityContext에서 Authentication 가져와서 이를 활용(url에 email 노출 안되게))

3. Email 중복 확인 컨트롤러 구현

4. content 생성 컨트롤러에 유저 확인 코드 추가, content 생성 뷰 수정(보기 편하게)

5. content 수정 뷰 및 컨트롤러 구현, 해당 뷰에서 사용할 DTO 구현(ContentDTO)

### 2021.6.2

1. ViewController -> 3개의 Controller(ContentController, PersonController, SpaceController)로 분기

2. Controller 설명 주석 추가

3. Error 페이지 및 컨트롤러 구현

4. 이메일 중복확인 프론트 구현

5. 프로젝트 뷰에 프로젝트 기간 추가

### 2021.6.3

1. DbConfig 삭제 -> DB 연결 정보 application.properties로 이동

2. Test 용 데이터베이스 설정 분리 -> application-test.properties, h2 임베디드 데이터베이스 사용

3. ContentController- deleteContent 실패 처리 코드 추가

4. ContentController Test Code 작성

### 2021.6.4

1. DTO 객체들 Validation 적용

2. SpaceController Test Code 작성

3. PersonController Test Code 작성

### 2021.6.5

1. RestfulController Test Code 작성

2. 메인 페이지 리스트 페이지 구현

3. 회원 탈퇴 컨트롤러 및 테스트 코드 구현

### 2021.6.6

1. Domain 관련 Service 클래스들 (PersonService, SpaceService, ContentService) Test Code 작성

2. Login, Join, ProfileUpdate 뷰 깔끔하게 정리

3. AWS EC2 인스턴스와 연결

### 2021.6.7

1. 개인 프로젝트 개수 제한 - 최대 50개

2. 도메인 네임 등록 (www.info-gun.net)

### 2021.6.8

1. 배포 스크립트 (deploy.sh) 작성

2. travisCI 설정 파일 작성(.travis.yml) 및 연결 

3. travisCI 와 S3 연결 

4. S3와 CodeDeploy 연결

### 2021.6.9

1. CSS, IMG 파일 레포지토리에 추가

2. 코드 자동 배포 구현 

3. 첫 배포 (ver 0.0.2)
