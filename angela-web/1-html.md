# Section 2: Introduction to HTML


## 11. Introduction to HTML

HTML = HyperText Markup Language

<h1></h1> 부터 <h6></h6> 까지

MDN

<br>


## 12. The Anatonmy of an HTML tag

Browser에서 Right click->Inspect->Elements

![image](https://user-images.githubusercontent.com/76763879/110209270-21d52680-7e51-11eb-8338-4e3a0770c487.png)
![image](https://user-images.githubusercontent.com/76763879/110209287-30bbd900-7e51-11eb-807f-824bf8437a3a.png)
![image](https://user-images.githubusercontent.com/76763879/110209299-492bf380-7e51-11eb-8643-3ba43cdf5fa6.png)

![image](https://user-images.githubusercontent.com/76763879/110209239-fe11e080-7e50-11eb-9159-5697050da330.png)
![image](https://user-images.githubusercontent.com/76763879/110209315-68c31c00-7e51-11eb-9962-f4b4d65d8527.png)

<hr size="3" noshade>
<center></center>
<!-- -->


## 13. What we're building - HTML Personal Site

그냥 CS Professors' websites 보여줌 


## 14. What is the HTML Boilerplate? 

index.html
Boilerplate는 Atom에서 html 타이핑하고 엔터하면 나오는 거
<head></head> 이 안에 들어가는 건 구글링에 관련된 거 ㅇㅇ
<body></body> 이 안에 들어가는 게 진짜로 웹페이지에 보이는 거 ㅇㅇ
<title></title> 탭에 나오는 글자들
Atom에서 파일 클릭하고 오른쪽 클릭하고 Copy the full path 누르면 browser에서 바로 열기 가능


## 15. How to Structure Text in HTML

![image](https://user-images.githubusercontent.com/76763879/110209448-4bdb1880-7e52-11eb-9221-f05943d88290.png)
<p></p>
<em> vs <i> logical state vs physical state (구글링에 다르게 결과 나옴)
<strong> vs <b>


## 16. HTML List

<ul></ul> Unordered List
<ol></ol> Ordered List
<li></li> List Item (안에 넣음)


## 17. HTML Image Element

![image](https://user-images.githubusercontent.com/76763879/110209540-cb68e780-7e52-11eb-85d5-993a797542bc.png)
이미지가 웹에 게시된 경우: <img src="{웹이미지 URL}" alt="{구글링할 때 여기 뭘 넣으냐에 따라 검색결과 ㅇㅇ 예: angela profile picture}">
photobucket.com
<img src="angela.png" alt="angela profile picture">
<img src="images/angela.png" alt="angela profile picture">


## 18. HTML Links and Anchor Tags

Hypertext = Hyperlink로 text를 잇는 것
![image](https://user-images.githubusercontent.com/76763879/110220519-c4aa9680-7e8b-11eb-856b-116e974bd358.png)
<a href="http://www.google.com">Google</a>
![image](https://user-images.githubusercontent.com/76763879/110220559-fcb1d980-7e8b-11eb-9a9d-11e58b43e0ad.png)
<a href="hobbies.html">My Hobbies</a>

이미지가 웹에 게시된 경우: <img src="{웹이미지 URL}" alt="{구글링할 때 여기 뭘 넣으냐에 따라 검색결과 ㅇㅇ 예: angela profile picture}">
photobucket.com (여기서 많은 이미지 찾기 가능)



# Section 3: Intermediate HTML

## 20. HTML Tables

<table>
  <thead> //unnecessary - 왜 쓰냐면 CSS 때 쓰일 수도 있어서
    <tr>
      <th>Company</th>
      <th>Contact</th>
      <th>Country</th>
    </tr>
  </thead> //unnecessary
  <tbody> //unnecessary
    <tr>
      <td>Alfreds Futterkiste</td>
      <td>Maria Anders</td>
      <td>Germany</td>
    </tr>
    <tr>
      <td>Centro comercial Moctezuma</td>
      <td>Francisco Chang</td>
      <td>Mexico</td>
    </tr>
  </tbody> //unnecessary
  <tfoot> //unnecessary
  </tfoot> //unnecessary
</table>

<table border="1"> 근데 CSS 나와서 이런 거 ㄴㄴ임


## 21. Using HTML Tables for Layout

<table cellspacing="20"> //pixel임


## 23. How to Type Emojis

WIN + . 혹은 WIN + ;

<해보기>
![image](https://user-images.githubusercontent.com/76763879/110249185-8ddf8980-7f3a-11eb-84db-c0909ed81ec8.png)


## 25. HTML Forms

<form>
  <label>First name:</label>
  <input type="text" name="" value=""><br>
  <input type="submit" name="" value="Save">
  <input type="checkbox" name="" value="">
  <input type="password" name="" value="">
</form>

여러가지 타입
![image](https://user-images.githubusercontent.com/76763879/110249343-5cb38900-7f3b-11eb-8430-5974582d37a0.png)


## 26. Forms in Practice - Create a Contact Me Form

<textarea name="" rows="8" cols="80"></textarea>

<해보기>
![image](https://user-images.githubusercontent.com/76763879/110249414-9f756100-7f3b-11eb-94b0-f16cef396327.png)
<정답>
![image](https://user-images.githubusercontent.com/76763879/110249439-bddb5c80-7f3b-11eb-9bdb-29ec4e18268a.png)


## 27. Publish Your Website!

GitHub Page
