# 웹표준 사이트

    웹표준을 준수하여 만든 사이트입니다.   
    IR효과, W3C CSS&HTML 체크를 거쳤습니다.
    사용한 라이브러리: slick, LightGallery, jQuery

### 목차
1. [Header](#1-header)   
   1. [Header menu](#11-header-menu)
   2. [Header title](#12-header-title)
   3. [Header icon](#13-header-icon)
2. [Content](#2-content)
   1. [Content nav](#21-content-nav)
   2. [Content title](#22-content-title)
   3. [Content banner](#23-content-banner)
   4. [Content notice](#24-content-notice)
       1. [Notice01](#241-notice01)
       2. [Notice02](#242-notice02)
       3. [Notice03](#243-notice03)
       4. [Notice04](#244-notice04)
       5. [Notice05](#245-notice05)
       6. [Notice06](#246-notice06)
3. [Footer](#3-footer)

### Preview
<img src="/readme_img/preview.png" width="700px" alt="preview">

---

# 1. Header
<img src="/readme_img/header.PNG" width="900px" alt="header">

## 1.1 Header menu

- HTML
```
<a href="#">Designer</a>
<a href="#">Publisher</a>
<a href="#">Youtube</a>
```
- CSS
```
.header .header-menu { text-align: right; }
.header .header-menu a { color: #fff; padding: 10px 0 10px 13px; display: inline-block; }
```

> display 속성값별 차이점   

    - none: 요소를 렌더링하지 않도록 설정한다. 요소가 차지하는 영역도 없앤다.   
    - block: 가로 영역을 모두 채운다. block 다음으로 오는 요소는 자동으로 줄바꿈이 된다.  
    - inline: height, width값을 설정할 수 없으며 줄바꿈이 일어나지 않는다.   
    inline 다음으로 오는 요소는 오른쪽에 배치된다.   
    - inline-block: 크기를 조정할 순 있지만 줄바꿈은 이루어지지 않는다.
    
## 1.2 Header title
- HTML
```
<div class="header-tit">
 <h1>Professional Publisher &amp; Designer</h1>
 <a href="https://www.youtube.com" target="_blank">Youtube.com</a>
</div>
```

- CSS
```
.header .header-tit { text-align: center; }
.header .header-tit h1 { background-color: #4aa8da; font-size: 28px; padding: 5px 20px 6px 20px; margin-top: 40px; color: #fff; font-weight: normal; text-transform: uppercase; }
.header .header-tit a { display: inline-block; background-color: #2698cb; font-size: 18px; color: #fff; padding: 5px 20px 6px 20px; margin-top: -5px; }
```

## 1.3 Header icon
- HTML
```
<div class="header-icon">
  <a href="#" class="icon1">
    <span class="ir_pm"> icon1 </span>
  </a>
  <a href="#" class="icon2">
    <span class="ir_pm"> icon2 </span>
  </a>
  <a href="#" class="icon3">
    <span class="ir_pm"> icon3 </span>
  </a>
  <a href="#" class="icon4">
    <span class="ir_pm"> icon4 </span>
  </a>
</div>
```

- CSS
```
.header .header-icon { text-align: center; margin-top: 30px; }
.header .header-icon a { width: 60px; height: 60px; display: inline-block; background: url(../img/icon.png); margin: 0 3px; }
.header .header-icon a.icon1 { background-position: 0 0; }
.header .header-icon a.icon2 { background-position: 0 -60px; }
.header .header-icon a.icon3 { background-position: 0 -120px; }
.header .header-icon a.icon4 { background-position: 0 -180px; }
.header .header-icon a.icon1:hover { background-position: -60px 0; }
.header .header-icon a.icon2:hover { background-position: -60px -60px; }
.header .header-icon a.icon3:hover { background-position: -60px -120px; }
.header .header-icon a.icon4:hover { background-position: -60px -180px; }
```

> 이미지 스프라이트로 아이콘들을 하나의 파일로 압축하여 사용    
> 각각의 맞는 이미지들은 `background-position`속성을 통해 좌표로 설정

---

# 2. Content
<img src="/readme_img/content.PNG" width="900px" alt="content">

## 2.1. Content nav
<img src="/readme_img/content_nav.PNG" width="900px" alt="content_nav">

- HTML
```
<div id="cont_nav">
 <div class="container">
   <h2 class="ir_su">전체 메뉴</h2>
   <div class="nav">
     <div>
       <h3>HTML Reference</h3>
       <ol>
         <li><a href="#">HTML 태그(Tag)</a></li>
         <li><a href="#">블록 요소/인라인 요소</a></li>
         <li><a href="#">DTD 선언</a></li>
         <li><a href="#">언어 속성 설정</a></li>
         <li><a href="#">HTML &lt;title&gt;</a></li>
         <li><a href="#">HTML &lt;meta&gt;</a></li>
         <li><a href="#">특수문자</a></li>
         <li><a href="#">하이퍼 링크</a></li>
         <li><a href="#">HTML &lt;style&gt;</a></li>
         <li><a href="#">HTML &lt;html&gt;</a></li>
         <li><a href="#">HTML &lt;head&gt;</a></li>
         <li><a href="#">HTML &lt;div&gt;</a></li>
         <li><a href="#">HTML &lt;colgroup&gt;</a></li>
         <li><a href="#">HTML &lt;caption&gt;</a></li>
       </ol>
     </div>
     <div>
       <h3>CSS Reference</h3>
       <ol>
         <li><a href="#">CSS 선택자</a></li>
         <li><a href="#">CSS 단위</a></li>
         <li><a href="#">CSS 색상</a></li>
         <li><a href="#">CSS 선언 방법</a></li>
         <li><a href="#">상대주소와 절대주소</a></li>
         <li><a href="#">CSS float</a></li>
         <li><a href="#">이미지 표현 방법</a></li>
         <li><a href="#">이미지 스프라이트</a></li>
         <li><a href="#">IR 효과</a></li>
         <li><a href="#">이미지 최적화</a></li>
         <li><a href="#">background-color</a></li>
         <li><a href="#">border-style</a></li>
         <li><a href="#">font-size</a></li>
         <li><a href="#">text-align</a></li>
       </ol>
     </div>
     <div class="last">
       <h3>Webstandard</h3>
       <ol>
         <li><a href="#">웹 표준</a></li>
         <li><a href="#">웹 접근성</a></li>
         <li><a href="#">W3C</a></li>
         <li><a href="#">웹 접근성 연구소</a></li>
         <li><a href="#">네이버 널리</a></li>
         <li><a href="#">다음 다룸</a></li>
         <li><a href="#">Webstandard</a></li>
       </ol>
     </div>
   </div>
 </div>
</div>
```

- CSS
```
#cont_nav { background-color: #f6fdff; display: none; }
.nav { overflow: hidden; padding: 30px 0; }
.nav > div { float: left; width: 40%; }
.nav > div.last { width: 20%; }
.nav > div h3 { font-size: 18px; color: #25a2d0; margin-bottom: 4px; }
.nav > div ol { overflow: hidden; }
.nav > div ol li { float: left; width: 50%; }
.nav > div.last ol li { width: 100%; }
.nav > div ol li a:hover{ text-decoration: underline; }
```

> `float: left`속성을 이용하여 요소들을 배치   
> `float: left`속성을 사용할 경우 부모 요소에게 `overflow: hidden`속성을 꼭 붙여줄 것

## 2.2. Content title
- HTML
```
<div id="cont_tit">
 <div class="container">
   <div class="tit">
     <h2>"나는 퍼블리셔다"</h2>
     <a href="#" class="btn"><span class="ir_pm">전체메뉴</span></a>
   </div>
 </div>
</div>
```

- CSS
```
#cont_tit { background-color: #eaf7fd; }
.tit { position: relative; }
.tit h2 { font-size: 40px; text-align: center; padding: 5px 0; letter-spacing: 2px; color: #2c94c4; font-family: 'Nanum Brush Script', cursive; }
.tit .btn { position: absolute; top: 5px; right: 0; width: 60px; height: 60px; background: url(../img/icon.png) no-repeat 0-600px; }
.tit .btn.on { background-position: 0 -660px; }
```

- JS
```
$(".tit .btn").click(function (e) {
  e.preventDefault();
  $("#cont_nav").slideToggle(200);
  $(this).toggleClass("on");
});
```

> `position: absolute`속성을 이용해 요소를 배치   
> `position: absolute`속성을 사용할 경우 부모 요소에게 `position: relative`속성을 부여   
> `preventDefault()`함수를 사용하여 클릭할 때마다 새로고침하는 현상을 제어

## 2.3. Content banner
<img src="/readme_img/content_banner.PNG" width="900px" alt="content_banner">

- HTML
```
<div id="cont_ban">
 <div class="container">
   <div class="ban">     
     <div>
       <a href="#">
         <img src="img/banner_link1.jpg" alt="웹 표준 지침서 보기" />
       </a>
     </div>
     <div>
       <a href="#">
         <img src="img/banner_link2.jpg" alt="CSS 버튼 만들기" />
       </a>
     </div>
     <div>
       <a href="#">
         <img src="img/banner_link3.jpg" alt="로그인 폼 만들기" />
       </a>
     </div>
     <div>
       <a href="#">
         <img src="img/banner_link1.jpg" alt="웹 표준 지침서 보기" />
       </a>
     </div>
     <div>
       <a href="#">
         <img src="img/banner_link2.jpg" alt="CSS 버튼 만들기" />
       </a>
     </div>
     <div>
       <a href="#">
         <img src="img/banner_link3.jpg" alt="로그인 폼 만들기" />
       </a>
     </div>
     <div>
       <a href="#">
         <img src="img/banner_link1.jpg" alt="웹 표준 지침서 보기" />
       </a>
     </div>
     <div>
       <a href="#">
         <img src="img/banner_link2.jpg" alt="CSS 버튼 만들기" />
       </a>
     </div>
     <div>
       <a href="#">
         <img src="img/banner_link3.jpg" alt="로그인 폼 만들기" />
       </a>
     </div>
   </div>
 </div>
</div>
```

- CSS
```
#cont_ban { background-color: #dceff7; }
.ban { position: relative; padding: 24px 0 40px; }
.ban .slick-prev { position: absolute; left: -80px; top: 80px; width: 43px; height: 43px; background: url(../img/icon.png) no-repeat -150px 0; text-indent: -9999px; }
.ban .slick-next { position: absolute; right: -80px; top: 80px; width: 43px; height: 43px; background: url(../img/icon.png) no-repeat -150px -43px; text-indent: -9999px; }
.ban .slick-prev:hover { background-position: -193px 0; }
.ban .slick-next:hover { background-position: -193px -43px; }
.ban img { border: 4px solid #dcdcdc; }
.ban img:hover { border-color: #98bcdc; }
.ban .slick-slide { margin: 10px; }
.ban .slick-dots { position: absolute; bottom: 15px; display: block; width: 100%; text-align: center; }
.ban .slick-dots li { display: inline-block; width: 15px; height: 15px; margin: 5px; }
.ban .slick-dots li button { font-size: 0; line-height: 0; display: block; width: 15px; height: 15px; cursor: pointer; background: #5bdfeb; border-radius: 50%; }
.ban .slick-dots li.slick-active button { background: #2b91c8; }
```

- JS
```
$(".ban").slick({
  infinite: true,
  slidesToShow: 3,
  slidesToScroll: 3,
  autoplay: true,
  autoplaySpeed: 3000,
  dots: true,
});
```

> slick-slider 라이브러리를 사용

## 2.4. Content notice

### 2.4.1. Notice01
<img src="/readme_img/notice01.PNG" width="300px" alt="notice01">

- HTML
```
<div class="column col1">
 <h3>
   <span class="ico_img ir_pm">아이콘</span>
   <span class="ico_tit">Notice</span>
 </h3>
 <p class="ico_desc">
   가장 웹 페이지에서 기본이 되는 게시판 유형입니다.
 </p>
 <div class="notice">
   <h4>Web Publisher Notice</h4>
   <ul>
     <li>
       <a href="#">
         display:inline과 display:block의 차이점은 무엇인가요?
       </a>
     </li>
     <li>
       <a href="#">
         HTML 태그 중에 dl,dd,ul,ol,li의 차이점이 무엇인가요?
       </a>
     </li>
     <li>
       <a href="#">
         HTML 태그 중에 strong과 em 태그의 차이점은 무엇인가요?
       </a>
     </li>
     <li>
       <a href="#">
         컨텐츠 요소를 가운데로 오게 하는 방법을 알려주세요!
       </a>
     </li>
     <li>
       <a href="#">
         독타입을 선언하는 이유에 대해서 설명하세요.
       </a>
     </li>
   </ul>
   <a href="#" class="more ir_pm" title="더보기">더보기</a>
 </div>
 <div class="notice2">
   <h4>Web Designer Notice</h4>
   <ul>
     <li>
       <a href="#"> JPG, PNG, GIF의 차이점이 무엇인가요? </a>
       <span>2018.11.16</span>
     </li>
     <li>
       <a href="#">
         UI 디자인과 UX 디자인의 차이점을 설명하세요.
       </a>
       <span>2018.11.16</span>
     </li>
     <li>
       <a href="#">
         인터랙션 디자인의 핵심은 무엇이라고 생각하나요?
       </a>
       <span>2018.11.16</span>
     </li>
     <li>
       <a href="#">
         포트폴리오를 하면서 가장 잘 했다고 생각하는 부분은
         무엇인가요?
       </a>
       <span>2018.11.16</span>
     </li>
     <li>
       <a href="#">
         웹 디자인과 모바일 디자인의 차이가 무엇이라고
         생각하나요?
       </a>
       <span>2018.11.16</span>
     </li>
   </ul>
   <a href="#" class="more ir_pm" title="더보기">더보기</a>
 </div>
</div>
```

- CSS
```
.notice { position: relative; }
.notice h4 { font-size: 14px; color: #0093bd; padding-bottom: 3px; font-weight: bold; }
.notice ul li { overflow: hidden; text-overflow: ellipsis; white-space: nowrap; background: url(../img/dot.gif) no-repeat 0 8px; padding-left: 8px; }
.notice ul li a { font-size: 12px; }
.notice a.more { position: absolute; right: 0; top: 0; display: block; background: url(../img/icon.png) -150px -90px; width: 17px; height: 17px; }
.notice2 { position: relative; margin-top: 15px; }
.notice2 h4 { font-size: 14px; color: #0093bd; padding-bottom: 3px; font-weight: bold; }
.notice2 li { overflow: hidden; background: url(../img/dot.gif) no-repeat 0 8px; padding-left: 8px; }
.notice2 li a { float: left; width: 65%; overflow: hidden; text-overflow: ellipsis; white-space: nowrap; }
.notice2 li span { float: right; width: 30%; text-align: right; }
.notice2 a.more { position: absolute; right: 0; top: 0; display: block; background: url(../img/icon.png) -150px -90px; width: 17px; height: 17px; }
```

> 텍스트를 한 줄로 표현할 때 사용하는 속성 3가지   

    overflow: hidden;   
    text-overflow: ellipsis;   
    white-space: nowrap;

### 2.4.2. Notice02
<img src="/readme_img/notice02.PNG" width="300px" alt="notice02">

- HTML
```
<div class="column col2">
 <h3>
   <span class="ico_img ir_pm">아이콘</span>
   <span class="ico_tit">Notice</span>
 </h3>
 <p class="ico_desc">
   가장 웹 페이지에서 기본이 되는 게시판 유형입니다.
 </p>
 <div class="notice3">
   <h4>Html Reference</h4>
   <ul>
     <li>
       <a href="#">
         <img src="img/notice01.jpg" alt="이미지1" />
         <strong>[HTML] table</strong>
         <span>table 태그는 표를 만들 때 사용합니다.</span>
       </a>
     </li>
     <li>
       <a href="#">
         <img src="img/notice02.jpg" alt="이미지2" />
         <strong>[HTML] div</strong>
         <span
           >div 태그는 문서의 섹션을 만들거나 영역을 나눌 때
           사용합니다.</span
         >
       </a>
     </li>
     <li>
       <a href="#">
         <img src="img/notice03.jpg" alt="이미지3" />
         <strong>[HTML] dl</strong>
         <span
           >dl 태그는 용어를 설명하는 목록형 태그입니다.</span
         >
       </a>
     </li>
     <li>
       <a href="#">
         <img src="img/notice04.jpg" alt="이미지4" />
         <strong>[HTML] em</strong>
         <span>em 태그는 텍스트를 강조할 때 사용합니다.</span>
       </a>
     </li>
   </ul>
   <a href="#" class="more ir_pm" title="더보기">더보기</a>
 </div>
</div>
```

- CSS
```
.notice3 { position: relative; }
.notice3 h4 { font-size: 14px; color: #0093bd; padding-bottom: 3px; font-weight: bold; }
.notice3 li { position: relative; padding: 8px 0 14px 60px; }
.notice3 li a img { width: 50px; position: absolute; left: 0; top: 0; border: 1px solid #0093bd; }
.notice3 li a strong { display: block; overflow: hidden; text-overflow: ellipsis; white-space: nowrap; }
.notice3 li a span { display: block; overflow: hidden; text-overflow: ellipsis; white-space: nowrap; font-size: 12px; }
.notice3 a.more { position: absolute; right: 0; top: 0; display: block; background: url(../img/icon.png) -150px -90px; width: 17px; height: 17px; }
```

> `em`요소와 `strong`요소의 차이점

    em: 해당 컨텐츠의 강세를 나타내는 요소
    strong: 중요성, 심각성, 긴급성을 표현한 요소

### 2.4.3. Notice03
<img src="/readme_img/notice03.PNG" width="300px" alt="notice03">

- HTML
```
<div class="column col3">
 <h3>
   <span class="ico_img ir_pm">아이콘</span>
   <span class="ico_tit">Notice</span>
 </h3>
 <p class="ico_desc">
   가장 웹 페이지에서 기본이 되는 게시판 유형입니다.
 </p>
 <div id="login_wrap">
   <h4 class="ir_su">로그인 정보</h4>
   <form id="login_form" name="login_form" action="post">
     <fieldset>
       <legend class="ir_su">로그인 및 관련 설정</legend>
       <div class="login_header">
         <h5 class="ir_su">로그인 보안</h5>
         <div class="lh_check">
           <input
             id="info_check"
             type="checkbox"
             class="input_check"
           />
           <label for="info_check">로그인 상태 유지</label>
         </div>
         <div class="lh_ip">IP보안 <em>ON</em></div>
       </div>
       <div class="login_content">
         <h5 class="ir_su">로그인 영역</h5>
         <div class="lc_text">
           <label for="uid" class="ir_su">아이디</label>
           <input
             type="text"
             id="uid"
             name="uid"
             class="input_text"
             maxlength="20"
             placeholder="아이디"
           />
           <label for="upw" class="ir_su">비밀번호</label>
           <input
             type="password"
             id="upw"
             name="upw"
             class="input_text"
             maxlength="20"                            
             placeholder="비밀번호"
           />
         </div>
         <button class="lc_btn" type="submit">로그인</button>
       </div>
       <div class="login_footer">
         <h5 class="ir_su">로그인 문제해결</h5>
         <ul>
           <li>
             <a href="#"><strong>회원가입</strong> / </a>
           </li>
           <li>
             <a href="#">아이디</a> ·
             <a href="#">비밀번호 찾기</a>
           </li>
         </ul>
       </div>
     </fieldset>
   </form>
 </div>
 <div class="popup">
   <h4>Advertisement</h4>
   <ul>
     <li class="layer">
       <a href="#"><img src="img/sban07.jpg" alt="이미지1" /></a>
     </li>
     <li class="window">
       <a href="#"><img src="img/sban08.jpg" alt="이미지2" /></a>
     </li>
     <li class="last" id="lightgallery">
       <a href="img/webstandard3.jpg">
         <img src="img/sban09.jpg" alt="이미지3" />
       </a>
     </li>
   </ul>
 </div>
</div>
```

- CSS
```
#login_wrap { margin-bottom: 15px; background: #f2f4f5; padding: 15px; }
.login_header { overflow: hidden; font-size: 12px; height: 30px; }
.login_header .lh_check { float: left; padding-right: 15px; }
.login_header .lh_check .input_check { vertical-align: -2px; }
.login_header .lh_ip { float: left; }
.login_header .lh_ip em { color: #0093bd; text-decoration: underline; }
.login_content { position: relative; }
.login_content .lc_btn { position: absolute; top: 0; right: 0; width: 62px; height: 47px; background: #fff; border: 1px solid #bebebe; }
.login_content .input_text { width: 182px; height: 16px; padding: 2px 5px; border: 1px solid #bebebe; margin-bottom: 3px; background: #fff; }
.login_footer { margin-top: 5px; }
.login_footer li { display: inline; }
.login_footer li a { font-size: 12px; }
.popup h4 { font-size: 14px; color: #0093bd; padding-bottom: 4px; font-weight: 700; }
.popup ul { overflow: hidden; }
.popup ul li { float: left; width: 93px; margin-right: 5px; }
.popup ul li.last { margin-right: 0; }
.popup ul li img { width: 100%; }
```

- JS
```
lightGallery(document.getElementById("lightgallery"), {
  speed: 300,
});

$(".window").click(function (e) {
  e.preventDefault();
  window.open(
    "popup.html",
    "popup01",
    "width=800, height=590, left=50, top=50, scrollbars=0, toolbar=0, menubar=0"
  );
});

$(".layer").click(function (e) {
  e.preventDefault();
  // $("#layer").css("display", "block");
  $("#layer").slideDown();
});
$("#layer .close").click(function (e) {
  e.preventDefault();
  // $("#layer").css("display", "none");
  $("#layer").slideUp();
});
```

> 팝업 종류는 레이어 팝업, 윈도우 팝업, 라이트박스 등이 있음

- 레이어 팝업
<img src="/readme_img/popup01.PNG" width="300px" alt="popup01">

- 윈도우 팝업
<img src="/readme_img/popup02.PNG" width="300px" alt="popup02">

- 라이트박스
<img src="/readme_img/popup03.PNG" width="300px" alt="popup03">

> 라이트박스는 `LightGallery` 라이브러리를 사용


### 2.4.4. Notice04
<img src="/readme_img/notice04.PNG" width="300px" alt="notice04">

- HTML
```
<div class="column col4">
 <h3>
   <span class="ico_img ir_pm">아이콘</span>
   <span class="ico_tit">Notice</span>
 </h3>
 <p class="ico_desc">
   가장 웹 페이지에서 기본이 되는 게시판 유형입니다.
 </p>
 <div class="notice_hover">
   <h4>Mouse Hover</h4>
   <ul>
     <li>
       <a href="#">
         <span>
           <img src="img/sban01.jpg" alt="이미지1" />
           <em>바로가기</em>
         </span>
         <strong>와이어 프레임</strong>
       </a>
     </li>
     <li>
       <a href="#">
         <span>
           <img src="img/sban02.jpg" alt="이미지2" />
           <em>바로가기</em>
         </span>
         <strong>스케치 작업</strong>
       </a>
     </li>
     <li class="last">
       <a href="#">
         <span>
           <img src="img/sban03.jpg" alt="이미지3" />
           <em>바로가기</em>
         </span>
         <strong>UI 디자인</strong>
       </a>
     </li>
   </ul>
 </div>
 <div class="notice_hover2 mt15">
   <h4 class="ir_su">Mouse Hover2</h4>
   <ul>
     <li>
       <a href="#">
         <span>
           <img src="img/sban04.jpg" alt="이미지4" />
           <em>바로가기</em>
         </span>
         <strong>HTML</strong>
       </a>
     </li>
     <li>
       <a href="#">
         <span>
           <img src="img/sban05.jpg" alt="이미지5" />
           <em>바로가기</em>
         </span>
         <strong>CSS</strong>
       </a>
     </li>
     <li class="last">
       <a href="#">
         <span>
           <img src="img/sban06.jpg" alt="이미지6" />
           <em>바로가기</em>
         </span>
         <strong>jQuery</strong>
       </a>
     </li>
   </ul>
 </div>
</div>
```

- CSS
```
.notice_hover h4 { font-size: 14px; color: #0093bd; padding-bottom: 3px; font-weight: bold; }
.notice_hover ul { overflow: hidden; }
.notice_hover li { float: left; width: 93px; margin-right: 5px; text-align: center; }
.notice_hover li.last { margin-right: 0; }
.notice_hover li a span { position: relative; display: block; width: 93px; height: 93px; line-height: 93px; }
.notice_hover li a span img { width: 100%; }
.notice_hover li a span em { visibility: hidden; position: absolute; left: 0; top: 0; background: rgba(0, 0, 0, 0.7); color: #fff; width: 100%; height: 100%; }
.notice_hover li a span:hover em { visibility: visible; }
.notice_hover li a strong{ padding-top: 3px; display: inline-block; font-size: 12px; }
.notice_hover2 ul { overflow: hidden; }
.notice_hover2 li { float: left; width: 93px; margin-right: 5px; text-align: center; }
.notice_hover2 li.last { margin-right: 0; }
.notice_hover2 li a span { position: relative; display: block; width: 93px; height: 93px; }
.notice_hover2 li a span img { width: 100%; }
.notice_hover2 li a span em{ visibility: hidden; position: absolute; left: 0; bottom: 0; background: rgba(0, 0, 0, 0.7); color: #fff; width: 100%; }
.notice_hover2 li a span:hover em { visibility: visible; }
.notice_hover2 li a strong { padding-top: 3px; display: inline-block; font-size: 12px; }
```

> `visibility: hidden`속성은 `display: none`과 달리 요소가 사라지지만 영역은 존재

### 2.4.5. Notice05
<img src="/readme_img/notice05.PNG" width="300px" alt="notice05">

- HTML
```
<div class="column col5">
 <h3>
   <span class="ico_img ir_pm">아이콘</span>
   <span class="ico_tit">Notice</span>
 </h3>
 <p class="ico_desc">
   가장 웹 페이지에서 기본이 되는 게시판 유형입니다.
 </p>
 <div class="tab_menu">
   <h4 class="ir_su">탭 메뉴</h4>
   <ul>
     <li class="active">
       <a href="#">공지사항1</a>
       <ul>
         <li>
           <a href="#">
             첫 번째 공지사항 탭 메뉴 테스트 목록입니다. 첫 번째
             공지사항 탭 메뉴 테스트 목록입니다.
           </a>
         </li>
         <li>
           <a href="#">
             첫 번째 공지사항 탭 메뉴 테스트 목록입니다. 첫 번째
             공지사항 탭 메뉴 테스트 목록입니다.
           </a>
         </li>
         <li>
           <a href="#">
             첫 번째 공지사항 탭 메뉴 테스트 목록입니다. 첫 번째
             공지사항 탭 메뉴 테스트 목록입니다.
           </a>
         </li>
       </ul>
     </li>
     <li>
       <a href="#">공지사항2</a>
       <ul>
         <li>
           <a href="#">
             두 번째 공지사항 탭 메뉴 테스트 목록입니다.
           </a>
         </li>
         <li>
           <a href="#">
             두 번째 공지사항 탭 메뉴 테스트 목록입니다.
           </a>
         </li>
         <li>
           <a href="#">
             두 번째 공지사항 탭 메뉴 테스트 목록입니다.
           </a>
         </li>
       </ul>
     </li>
     <li>
       <a href="#">공지사항3</a>
       <ul>
         <li>
           <a href="#">
             세 번째 공지사항 탭 메뉴 테스트 목록입니다.
           </a>
         </li>
         <li>
           <a href="#">
             세 번째 공지사항 탭 메뉴 테스트 목록입니다.
           </a>
         </li>
         <li>
           <a href="#">
             세 번째 공지사항 탭 메뉴 테스트 목록입니다.
           </a>
         </li>
       </ul>
     </li>
   </ul>
 </div>
 <div class="notice4 mt15">
   <h4>최신 <em>공지사항</em></h4>
   <ul>
     <li>
       <a href="#">
         웹 디자이너와 웹 퍼블리셔의 차이점은 무엇인가요?
       </a>
       <span>2018.11.19</span>
     </li>
     <li>
       <a href="#">
         웹 디자이너와 웹 퍼블리셔의 차이점은 무엇인가요?
       </a>
       <span>2018.11.19</span>
     </li>
     <li>
       <a href="#">
         웹 디자이너와 웹 퍼블리셔의 차이점은 무엇인가요?
       </a>
       <span>2018.11.19</span>
     </li>
   </ul>
   <a href="#" class="more" title="더보기">더보기</a>
 </div>
</div>
```

- CSS
```
.tab_menu { position: relative; border: 1px solid #ccc; padding: 8px; height: 105px; }
.tab_menu ul { overflow: hidden; border-bottom: 1px solid #ccc; }
.tab_menu ul li { float: left; border: 1px solid #ccc; margin-right: -1px; margin-bottom: -1px; }
.tab_menu ul li a { padding: 5px 10px; display: block; }
.tab_menu ul li ul { position: absolute; left: 0; top: 48px; width: 270px; border: 0; }
.tab_menu ul li ul li { float: none; border: 0; background: url(../img/dot.gif) no-repeat 9px 8px; padding-left: 18px; }
.tab_menu ul li ul li a { overflow: hidden; text-overflow: ellipsis; white-space: nowrap; width: 100%; padding: 0 0 3px 0; }
.tab_menu ul li.active { background: #2c94c4; }
.tab_menu ul li.active a { color: #fff; }
.tab_menu ul li.active ul li a { color: #333; }
.notice4 { position: relative; border: 1px solid #ccc; }
.notice4 h4 { font-size: 14px; color: #0093bd; padding: 8px 10px; font-weight: bold; border-bottom: 1px solid #ccc; }
.notice4 h4 em { color: #cf3292; }
.notice4 ul { padding: 10px; left: 0; top: 45px; }
.notice4 ul li { overflow: hidden; background: url(../img/dot.gif) no-repeat 0 8px; padding-left: 8px; padding-bottom: 2px; }
.notice4 ul li a { float: left; overflow: hidden; text-overflow: ellipsis; white-space: nowrap; width: 60%; }
.notice4 ul li span { float: right; width: 30%; text-align: right; padding-right: 8px; }
.notice4 a.more { position: absolute; top: 9px; right: 9px; }
```

- JS
```
let $tab_list = $(".tab_menu");
$tab_list.find("ul ul").hide();
$tab_list.find("li.active > ul").show();

function tabMenu(e) {
  e.preventDefault();
  let $this = $(this);
  $this
    .next("ul")
    .show()
    .parent("li")
    .addClass("active")
    .siblings("li")
    .removeClass("active")
    .find(">ul")
    .hide();
}
$tab_list.find("ul>li>a").click(tabMenu).focus(tabMenu);
```

### 2.4.6. Notice06
<img src="/readme_img/notice06.PNG" width="300px" alt="notice06">

- HTML
```
<div class="column col6">
 <h3>
   <span class="ico_img ir_pm">아이콘</span>
   <span class="ico_tit">Notice</span>
 </h3>
 <p class="ico_desc">
   가장 웹 페이지에서 기본이 되는 게시판 유형입니다.
 </p>
 <div class="gallery">
   <h4>포트폴리오</h4>
   <div class="gallery_btn">    
     <button class="gb_icon1 play">
       <span class="ir_pm">시작</span>
     </button>
     <button class="gb_icon2 pause">
       <span class="ir_pm">정지</span>
     </button>
     <button class="gb_icon3 prev">
       <span class="ir_pm">이전이미지</span>
     </button>
     <button class="gb_icon4 next">
       <span class="ir_pm">다음이미지</span>
     </button>
   </div>
   <div class="gallery_img">     
     <div>
       <a href="#">
         <img src="img/gallery01.jpg" alt="갤러리1" />
       </a>
     </div>
     <div>
       <a href="#">
         <img src="img/gallery02.jpg" alt="갤러리2" />
       </a>
     </div>
     <div>
       <a href="#">
         <img src="img/gallery03.jpg" alt="갤러리3" />
       </a>
     </div>
     <div>
       <a href="#">
         <img src="img/gallery04.jpg" alt="갤러리4" />
       </a>
     </div>
     <div>
       <a href="#">
         <img src="img/gallery05.jpg" alt="갤러리5" />
       </a>
     </div>
   </div>
 </div>
</div>
```

- CSS
```
.gallery { position: relative; border: 1px solid #ccc; height: 255px; overflow: hidden; }
.gallery h4 { font-size: 14px; color: #0093bd; border-bottom: 1px solid #ccc; padding: 10px 0 8px 11px; font-weight: 700; }
.gallery .gallery_btn { position: absolute; right: 5px; top: 7px; }
.gallery .gallery_btn button{ float: left; margin: 1px 2px; display: block; width: 23px; height: 23px; background: url(../img/icon.png) no-repeat; }
.gallery .gallery_btn .gb_icon1 { background-position: -150px -120px; }
.gallery .gallery_btn .gb_icon2 { background-position: -150px -143px; }
.gallery .gallery_btn .gb_icon3 { background-position: -150px -166px; }
.gallery .gallery_btn .gb_icon4 { background-position: -150px -189px; }
.gallery .gallery_btn .gb_icon1:hover { background-position: -173px -120px; }
.gallery .gallery_btn .gb_icon2:hover { background-position: -173px -143px; }
.gallery .gallery_btn .gb_icon3:hover { background-position: -173px -166px; }
.gallery .gallery_btn .gb_icon4:hover { background-position: -173px -189px; }
```

- JS
```
$(".gallery_img").slick({
  arrows: false,
  fade: true,
  pauseOnHover: true,
  infinite: true,
  autoplay: true,
  autoplaySpeed: 3000,
  speed: 300,
  slidesToShow: 1,
});
$(".play").click(function () {
  $(".gallery_img").slick("slickPlay");
});
$(".pause").click(function () {
  $(".gallery_img").slick("slickPause");
});
$(".prev").click(function () {
  $(".gallery_img").slick("slickPrev");
});
$(".next").click(function () {
  $(".gallery_img").slick("slickNext");
});
```

> slick-slide 라이브러리를 사용

---

# 3. Footer
<img src="/readme_img/footer.PNG" width="900px" alt="footer">

- HTML
```
<div id="footer">
  <div class="container">
    <h2 class="ir_su">푸터 영역</h2>
    <div class="footer">
      <ul>
        <li><a href="#">사이트 도움말</a></li>
        <li><a href="#">사이트 이용약관</a></li>
        <li><a href="#">사이트 운영규칙</a></li>
        <li>
          <a href="#"><strong>개인정보취급방침</strong></a>
        </li>
        <li><a href="#">책임의 한계와 법적고지</a></li>
        <li><a href="#">게시중단요청 서비스</a></li>
        <li><a href="#">고객센터</a></li>
      </ul>
      <address>Copyright 2022. Hyun-lo_Kim all rights reserved.</address>
      <div class="w3c mt15">
        <a href="http://validator.w3.org/check?uri=referer">
          <img
            src="http://www.w3.org/Icons/valid-xhtml10"
            alt="Valid XHTML 1.0 Transitional"
            height="31"
            width="88"
          />
        </a>
        <a href="http://jigsaw.w3.org/css-validator/check/referer">
          <img
            style="border: 0; width: 88px; height: 31px"
            src="http://jigsaw.w3.org/css-validator/images/vcss"
            alt="Valid CSS!"
          />
        </a>
      </div>
    </div>
  </div>
</div>
```

- CSS
```
.footer { padding: 25px 0; text-align: center; }
.footer ul { margin-bottom: 20px; }
.footer ul li { position: relative; display: inline; padding: 0 7px 0 10px; }
.footer ul li::before { content: ""; width: 1px; height: 12px; background: #ccc; position: absolute; left: 0; top: 2px; }
.footer ul li:first-child:before { width: 0; height: 0; }
```

> `width: 0; height: 0;`속성을 통해 요소를 숨길 수 있음
