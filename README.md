# Front End Develop Class by JD

참고 : github.com/edu-ministori/git06
codesendbox 원본 주소 : https://codesandbox.io/s/class0611-bi2mkq?file=/README.md

- md 파일 문법//간단한 형식의 문서파일

````
# ~ ###### : 제목

- : 목록

``` ~ ``` : 코드 블럭(backtick)

````

## 클라이언트 서버 모델

- 소프트웨어 개발시 복잡한 네트워크 하드웨어를 배제한 공급자, 사용자 양쪽 부분만 고려하는 모델
- 클라이언트의 요청(request)과 서버의 응답(response)의 사이클을 통해 서비스와 데이터 처리등의 기능이 실행됨

### Front End Develop VS Back End Develop

- Front End, Back End 용어

  - Front : 사용자를 기준으로 사용자가 보게 되는 화면 영역
  - Back : 사용자가 보지 못하고 서버상에서 데이터처리, 기능 동작등이 이루어지는 영역

- FE Dev : 사용자가 볼 수 있는 화면 개발

  - Web FE Dev : 브라우저에서 처리되고 렌더링 되는 언어를 사용해서 개발
  - 언어 : HTML, CSS, Javascript

- BE Dev : 사용자가 보지 못하는 영역에서 데이터 처리
  - 서버에서 처리되는 언어를 사용해서 개발
  - Java, PHP, Python, Nodejs

## Nameing 표기법

- 네이밍하는 경우

  - HTML/CSS : id, class
  - js : 변수, 함수
  - 파일, 폴더

- 표기법의 의미

  - 2개 단어 이상의 개수로 네이밍할 때, 단어와 단어 사이를 구분해야함

- 표기법의 종류//코딩할때 효율에 직관적인 문제. 별다섯개 4개의 표기법을 모두 사용하면서 하면 효율이 매우 올라간다.
  - section_content : snake case : 파일, 폴더
  - section-content : kebab case : id, class
  - secrionContent : camel case : js
  - SecrionContent : pascal case : js의 Class
