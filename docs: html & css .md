# HTML, CSS
docs: HTML, CSS에 대한 간략한 설명
## 목차
1. HTML
2. CSS




## 1. html이란?
* Hyper Text Markup Language
* 웹 사이트의 각 요소가 무엇을 뜻하는지 알려주는 언어

```!Doctype:html```로 html 타입을 정해준다.

### 1-1. meta tag 
* 추가 정보를 알려주는 것
* 웹페이지에 검색했을 때 나오는 내용이 meta 내용이다.
```ruby
<meta charset="utf-8">
<meta name="description" content="Welcome to my web">
```
### 1-2. head에는 information body에는 contents가 들어간다.

### 1-3. semantic & non semantic
* sematnic은 뜻, 의미가 있는 태그
* non-semantic은 아무 의미가 없는 태그

```ruby
Semantic (의미를 가지는 tag들)
<h1>this is title</h1>
<section>This is an important section</section>
------------------------------------------------
Non-Semantic (의미가 없는 tag들)
<div>우리가 박스 같은 것이 필요할때 사용</div>
<span>텍스트를 위한 컨테이너가 필요할 때 사용</span>
```
### 1-4. ID & Class
>* ID : 각 element당 ID는 한개씩만 가질 수 있다. ID는 고유하기 때문에 마치 **여권번호**같은 것
>```ruby
><header id="headerNumberOne" class="defaultHeader">
>```
> 즉, 고유한 element를 사용할때 ID를 적용한다.
<br>

>* Class : 내 이름처럼 반복가능하다. 2개 이상의 element가 중복해서 class를 가질 수 있다.
> 즉, 고유하지 않은 반복되는 element의 경우 class를 적용한다.


## 2. CSS란?
* html을 더욱 쉽고 사용자가 보기 좋게 스타일을 꾸밀 수 있게 도와주는 속성
* Selector 파트와 Property로 이루어짐.
>```ruby
>h1{   Property-value=true ; }
> h1은 셀럭터 {}안의 내용이 property가 된다
>```
>모든 태그들이 셀렉터가 될 수 있음 , 그안의 값을 정하는 것을 property-value라 한다.

### 2-1. CSS를 HTML에 넣는 방법
* inline 방법
```ruby
<style>
  background-color: red;
}
</style>
```
>하지만 같은 배경색을 써야하는 모든 html에 해당 css를 붙여넣기해야한다.
>굉장히 **비효율적이다.

* External 적용 방법
css파일 자체를 적용시킨다. 적용방법은 html의 head에 css를 불러준다.
```ruby 
<link href="styles.css" rel="stylesheet">
(css가 있는 파일의 경로를 넣어준다)
```
### 2-2. Box 모델
* [Box model](https://media.vlpt.us/images/kpl5672/post/de021ddb-fe7e-4041-9224-15748afdb064/boxmodel.gif)을 그림으로 먼저 확인해보자.
* border를 기준으로 안쪽을 padding 바깥쪽을 margin이라고 한다. 어느 방향으로 원하는대로 간격을 조절할 수 있다. 

```ruby
만약 padding을 상-하-좌-우 모두 간격을 주고 싶으면 
padding : 10px;

상-하, 좌-우 를 각각 주고 싶다면
padding : 20px 10px; 로 작성

상,우,하,좌 (시계방향)으로 각각 주고싶다면
padding : 5px 10px 15px 20px; 로 작성한다.

border-width :5px;
border-color :red;
border-style :dashed;

border:5px solid red; 로 줄여쓸 수도 있다. 
```

### 2-3. Inline & Block & Inline Block
