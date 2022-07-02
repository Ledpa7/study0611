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

### Layout
