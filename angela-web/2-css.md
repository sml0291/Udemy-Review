# Introduction to CSS


## 30. Introduction to CSS

CSS = Cascading Style Sheet = style markup language (혼자선 아무것도 못함 ㅇㅇ)
HTML로 디자인 하려니 너무 코딩이 길어짐. 그래서 만듬 ㅇㅇ


## 31. Inline CSS

<body></body>에다가 넣는 방법

<예시>
<body style="background-color: blue;">
hex color 
구글에 hex color라고 치면 나옴: https://www.google.com/search?q=hex+color&rlz=1C1CHBF_enUS892US892&oq=hex+color&aqs=chrome.0.0i433l3j0j0i433l2j0l4.921j0j7&sourceid=chrome&ie=UTF-8


## 33. Internal CSS

<head></head> 안에다가 넣는 방법

<문제>
이런 걸 만들고 싶은 거임
![image](https://user-images.githubusercontent.com/76763879/110249809-a1402400-7f3d-11eb-8d03-1495057b4f10.png)

<정답>
<head>
  <style>
    body {
      background-color: powderblue;
    }
    hr {
      background-color: red;
      border-style: dotted;
      border-color: grey;
      border-width: 5px;
      width: 5%;
    }
  </style>
</head>

근데 위처럼 만들면 내가 생각한 1라인이 안나옴 ㅇㅇ 그럼 어케 하냐?
border-style: none;
border-top-style: dotted; 로 해주면 됨 ㅇㅇ


## 34. External CSS

<head>
  <link rel="stylesheet" href="styles.css">
</head>

그 다음 styles.css에다가 body {...} h1 {...} 이런 거 넣으면 됨


## 35. How to Debug CSS Code

1) Right click->Inspect
2) 어떤 element 위에서 inspect하면 그 코드가 뜸


## 36. The Anatomy of CSS Syntax

![image](https://user-images.githubusercontent.com/76763879/110249931-6094da80-7f3e-11eb-80f9-7cacf0c20ee0.png)
![image](https://user-images.githubusercontent.com/76763879/110249951-760a0480-7f3e-11eb-88c3-70118a3b5b47.png)

css 폴더 만들고 그 안에 넣어보기
<link rel="stylesheet" href="css/styles.css">


## 37. CSS Selectors

Tag Selector은 h1, body 등 이미 있는 애들고 선택하는 것 (예: h1)
Class Selector은 class="broccoli" 등으로 이름을 따로 정해서 선택하는 것 (예: .broccoli)
Id Selector은 class랑 같이 이름을 따로 정하는 건데, class는 여러번 쓸 수 있지만 id는 딱! 한개임 ㅇㅇ (예: #title) Class랑 Id의 또다른 차이점은, class는 여러 개를 같이 쓸 수 있는데, id는 딱 한 개만 쓸 수 있음. (예: class="broccoli circular" 하고 .brocolli{...} .circular{...}. 근데 아이디는 id="broccoli" 끝.)

pseudo class는 앞에 : 있는 애들 (예를 들면 :hover). 얘들은 HTML elements가 different states 있어서 ㅇㅇ 
<예>
h1:hover {
  color: orange;
}



# Intermediate CSS


## 41. What We'll Make - Stylised Personal Site

<문제>
![image](https://user-images.githubusercontent.com/76763879/110262646-ed10be80-7f79-11eb-9b1d-3c2e00476945.png)


## 42. What Are Favicons?

Favicon = 위에 있는 탭에 보이는 아이콘
favicon.cc 에서 만들어서 `Download Favicon` 누른 후에 그냥 내 폴더에 드래그 한 뒤
<link rel="icon" href="favicon.ico"> 넣으면 됨ㅇㅇ


## 43. HTML Divs

<div></div> = divide our contents on website = grouping together

<예>
<div>
  <h1>Hello!</h1>
  <p>I'm Gloria.</p>
</div>

div {
  background-color: red;
}


## 44. The Box Model of Website Styling - 이건 좀 어려운 컨셉이라 같이 비디오 보는 게 좋을듯?

pixel (static)
% (dynamic)

![image](https://user-images.githubusercontent.com/76763879/110263042-1c73fb00-7f7b-11eb-941a-e26ea7c91e7f.png)
![image](https://user-images.githubusercontent.com/76763879/110263079-33b2e880-7f7b-11eb-8fb7-612bd77b2f8c.png)
![image](https://user-images.githubusercontent.com/76763879/110263107-44635e80-7f7b-11eb-9267-8d367a31c8f2.png)

<문제>
![image](https://user-images.githubusercontent.com/76763879/110263197-8ee4db00-7f7b-11eb-8fe7-130330f55a7b.png)


## 45. CSS Display Property - 이것도 같이 보는 게 좋을 듯. 말로 설명하긴 좀 어려운 컨셉.

block elements는 전체적으로 쭈욱~~ 다 지꺼임 (예: <p>나 <h1> 이나 <div>나 <form>이나 <ol> 등)
<span></span> 이 안에 중간에 조금 underline 할 것 넣을 수 있음. 왜냠 inline display elemtn라서. (타이트하게 박스)
inline elements는 딱 자기것만임. (예: <span>, <img>, <a>)

이런 display는 바꿀 수 있음. 
p {
  display: inline; 혹은 display:inline-block;
}
span {
  display: block; 
}
참고로 display: none이면 걍 아예 처음부터 없는 것처럼 안보임. 
(참고로 visibility: none;은 거기 있지만 안보임)


## 47. CSS Static and Relative Positioning

z-axis (가장 앞에 있는 것 span, 그 다음 h1 그 다음 div
![image](https://user-images.githubusercontent.com/76763879/110263667-ff402c00-7f7c-11eb-9615-9530a56e8681.png)

![image](https://user-images.githubusercontent.com/76763879/110263721-24349f00-7f7d-11eb-88d5-99f4a3a98408.png)
1. static = 원래 default
2. relative = 원래 default(즉 static)에 비해서 반영된 거
<예>
img {
  position: relative;
  left: 30px; 
} 일 경우, 원래 default에 비해 왼쪽으로 30px space 두게 움직인 거
![image](https://user-images.githubusercontent.com/76763879/110263855-8b525380-7f7d-11eb-843f-030bf281e391.png)



## 48. Absolute Positioning

## 49. The Dark Art of Centering Elements with CSS

## 50. Font Styling in Our Personal Site

## 51. Learn More About Typography

## 52. Adding Content to Our Website

## 53. CSS Sizing

## 58. CSS Float and Clear
