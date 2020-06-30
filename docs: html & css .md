# HTML, CSS
docs: HTML, CSS에 대한 간략한 설명

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



