# 자바웹프로그래밍(2) 실습

## 2주차 - 스프링 부트 개발환경, 테스트 완료
- 개발 환경: VS Code + Spring Boot 4.1.2 + Java 25 (Maven, Jar)
- 의존성: Spring Boot DevTools, Lombok, Spring Web, Spring Web Services, Thymeleaf, Spring Data JPA, MySQL Driver
  - DB 관련(Spring Data JPA, MySQL Driver)은 아직 DB 설정이 없어서 `pom.xml`에서 주석 처리
- [index.html : 실행 / 수정 완료](demo/src/main/resources/templates/index.html) - 메인 페이지, `/hello` 링크
- [hello.html](demo/src/main/resources/templates/hello.html) - `th:text="${data}"`로 컨트롤러 값 출력
- [DemoController.java](demo/src/main/java/com/example/demo/DemoController.java) - `@GetMapping("/hello")` URL 매핑
- **2주차 연습문제**: URL 맵핑과 컨트롤러 추가하기
  - `hello.html`에 두번째 헬로 페이지 링크 추가 (`/hello2`)
  - 컨트롤러에 `hello2` 메서드 추가, 모델 속성 5개(name, major, subject, week, message) 추가
  - [hello2.html](demo/src/main/resources/templates/hello2.html)에서 속성 5개 출력

### 실행 방법
`demo/src/main/java/com/example/demo/DemoApplication.java` 열고 `Ctrl + F5` → http://localhost:8080
