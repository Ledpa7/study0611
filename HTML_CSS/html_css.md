# HTML

- Cobtebts

  - Text
  - Media
    - Image, video, Audio

- Structure
  - Semantic : 의미 있는 구조
  - Layout

## HTML basic

- HTML : Hyper Text Markup Language

  - Hyper Text : 하이퍼링크로 연결된 문서 => 웹페이지(콘텐츠, 구조)
  - Markup : 표시
  - Language : 언어

- HTML 문법

  - 명칭 : Tag / Element
  - 구성 : 시작태그 ~ 종료태그
  - 종료태그가 없는 태그 : 빈태그(Empty Element)

  ```
  <Tag> content </Tag> : Element

  <tag ...> : Empty Element
  ```

- HTML 속성(attribute)
  - HTML Element를 표시할때 필요한 추가정보 입력
  - Name="value"
    '''
    <a href="https://www.naver.com">네이버</a>

<img src="photo.jpg">
'''

## HTML Basic Structure

```
<!DOCTYPE html>
<html>
  <head>
    <title></title>
  </head>
  <body></body>
</html>
```

### DOCTYPE

- HTML 문서타입
  - HTML 버전
  - HTML5 표준

### Head - 웹사이트 기본 정보

- meta : 웹사이트의 관련 정보(검색엔진)
- title : 웹사이트의 제목

### Body - 웹사이트 컨텐츠 정보

- 웹사이트에 contents, structre 표시되는 모든 태그

## HTML Contents

### Text

#### heading(제목)

- h(heading) : 제목태그
- 1 ~ 6 단계로 표시됨

#### paragraph(단락)

- p(paragraaph) : 단락태그
- 강제줄바꿈, 강제 공백은 이식되지 않고 공백 한 칸으로만 인식
  - Line berak : br(강제줄바꿈 태그)
  - space : &nbsp;(강제 공백 엔터티[entity])
  - hr(horizontal rule) : 수평선 긋기
    - 단락을 선의 형태로 구분

#### List(목록)

- 순서있는 목록
- ul(unordered List) : 순서없는 목록
- ol(Ordered List) : 순서있는 목록
- li(List Item) : 목록 항목

\*\* 포함관계(Nested Structure)

- 태그안에 다른 태그들이 포함되는 것
- 포함하는 요소
  - 조상요소(Ancestor)
  - 부모요소(Parent)
- 포함되는 요소
  - 자식요소(Child)
  - 자손요소(Descendant)
- 옆에 나란히 있는 요소 - 형제요소(Sibling)

'''
(1) <html>
(2)   <body>
(3)     <h1> 내용 제목 </h1>
(4)     <p>
(5)     단락내용<br>
        </P>
      <body>
    </html>
'''

(1)조상요소 | 기준요소 | 조상요소
(2)조상요소 | 자식요소 | 부모요소
(3)        | 자손요소 | 형제요소
(4)부모요소 | 자손요소 | 기준요소
(5)기준요소 | 자손요소 | 자식요소

- Description List(설명 목록)

  - dl(descriptip List)
  - dt(descriptip table)
  - dd(descriptip )

#### Table(표)

- table
- thead(table head) : 표 상단 - 제목
- tbody(table body) : 컨텐츠, 데이터
- tr(table row) : 행
- th(table header) : 제목
- td(table data) : 칸(열)

#### Hyper Link(하이퍼 링크)

- a(anchor)
- 기본 속성 : Href(hypertext reference) : 연결할 위치(웹페이지)

- 링크 이동 표시
  - 외부링크
  - 내부링크 : Bookmark

### Media

#### Image(이미지)

- img(image)
  - 빈 요소
- 기본 속성
  - src(source) : 이미지 파일 이름, 위치
  - alt(alternate text) : 대체 텍스트 - 이미지가 화면에 표시되지 않을때, screen reder
'''

<img src="photo.jpg" alt="">
'''

#### Video(영상)

-video, source
- 속성
  - video 태그 : on/off 형태attribute
    - controls : 동영상 제어 버튼
    - autoplay : 자동재생
    - muted : 음소거
    - loop : 반복 재생
  - source 태그
  - src : 파일 이름, 경로
  - tyoe : 미디어의 형식
  
- Youtube 영상

## HTML Structure

### Semantic

- header
  - logo, login...
- nav(navigation)
  - menu
- section
  - 본문 영역
- article
  - 본문 영역
- aside
  - 본문 영역, 부수적인 컨텐츠
- footer
  - 연락처, 주소, 회사 이름...

### Layout

- block & Inline
  - Block 요소
    - 태그가 브라우저에 표시될때 각 태그 영역이 새 줄에서 표시
    - 태그 영억이 부모요소에 전체 채워짐
  - Inline 요소
    - 태그가 브라우저에 표시될때 각 태그 영역이 같은 줄에서 표시
    - 태그 영역이 콘텐츠에 맞춰짐

### contrainer element

- 

## 경로 지정 방식

- 파일 위치, 인터넷 주소(URL)
- 상대 경로
  - 리소스 파일을 사용하는 HTML 파일 기준
  - html 파일 위치에 따라서 주소(URL) 변경
  - root(/) 폴더를 기준으로 주소 적용 => root 상대 경로

'''
  [root(/)] - [html1] - home.html
            - [html2] - about - about.html[]
            - [images] - photo.jpg

1) home.html -> photo.jpg
- ../images/photo.jpg
- /images/photo.jpg

2) about.html -> photo.jpg
- ../../images/photo.jpg
- /images/photo.jpg
'''

- 절대 경로
  - 이미지를 표시하는 HTML 페이지가 기준이 아니고 해당 서버가 기준 
  - 서버부터 주소(URL)를 사용하기 때문에 변동이 없음.

'''
image.com

  [root(/)] - [html1] - home.html
            - [html2] - about - about.html[]
            - [images] - photo.jpg

1) home.html
- www.images.com/images/photo.jpg

2) about.html
- www.image.com/images/photo.jpg

'''

## 강조 태그, 기타 태그

- 텍스트 특정 부분 강조
  - strong : 강한 강조
  - em(phasize) : 일반 강조
  - mark : html5 버전 

- 텍스트를 표현할 때 부족한 태그를 보완하는 태그
  - i(talic)
  - b(old)

# CSS

- content styling
  - text styling
  - media styling

- layout(structure styling)
  - 가로배치(flexbox)

## CSS Basic

- CSS : Cascading Style Sheet

'''
h1 {color:blue;font-size:20px;}

h1 {
  color:blue:
  font-size:20px;

}
'''

## Selector(선택자)

- 선택자로 HTML 요소를 선택
- HTML 요소 선택 방법
  - Simple Selector(단순 선택자)
    - Tag/Element 이름 사용
    - class 이름 사용
    - id 이름 사용

'''
<a href="https://www.naver.com" class = "naver">네이버</a>
<a href="https://www.daum.com" id="daum">다음</a>

/* a 태그 2개모두 red 적용 */
a {
  color:red;
}

/* a 태그 각각 다른 color 적용 */
.naver {
  color:blue;
}

#daum{
  color:green;
}

'''

### id, class 이름의 특징

- id 
  - 같은 HTML 페이지에서 고유(유일)해야 함 
    - 프로그래밍 언어의 변수(백엔드)와 연결 가능성이 있음
  - HTNL 요소에 여러개의 id 이름 사용 불가능 

- class
  - 같은 HTML 페이지에서 여러번 사용가능함
  - HTML 요소에 여러 개의 class 이름 사용 가능

'''
<p class="paragraph">단락1</p>
<p class="paragraph">단락2</p> (o)
<p id="content">단락3</p>
<p id="content">단락4</p> (x)


<p class="gnb-list-item">회사소개</p>
''' 

### CSS 선택자 우선순위

- cascading 규칙
  - 동일한 대상에 여러 스타일이 적용될 때 제일 마지막에 적용된 스타일이 반영

- 선택자 우선순위
  - 선택자 종류에 따라 css 적용 우선순위가 다르게 정의
  - cascading 규칙을 따르지 않고 CSS를 적용할 때 사용
  - inline : 1000
  - id : 100
  - class : 10
  - tag : 1