## 정리
```<link href="style.css" rel="stylesheet" type="text/css" />```
* style.css
  * css 파일을 html에 연결시켜주는 것
  * 스타일을 적용시켜줌

> ```<div>```태그
* 영역을 나눠줌
  <details>
    <summary>코드</summary>
    
    ```
    <!DOCTYPE html>
    <html lang="en">
    <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>basic</title>
      <link href="style.css" rel="stylesheet" type="text/css" />
    </head>
    <body>
      <div>My name is eunji</div>
      nice to meet you
    </body>
    </html>
    ```
  </details>

  <details>
    <summary>결과</summary>
    
    ![div](/img/div.png)
    
  </details>


> ```<p>```태그
* 영역을 나눠줌
  <details>
    <summary>코드</summary>
    
    ```
    <!DOCTYPE html>
    <html lang="en">
    <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>basic</title>
      <link href="style.css" rel="stylesheet" type="text/css" />
    </head>
    <body>
      <div>My name is eunji</div>
      I am 27 years old
      <p>nice to meet you</p>
    </body>
    </html>
    ```
  </details>

  <details>
    <summary>결과</summary>
    
    ![p](/img/p.png)
    
  </details>

#### div와 p 태그의 차이점
* div보다 p태그가 줄의 간격(높이)이 더 넓다.

> ```<img>```태그
* 태그가 하나만 있다
  * ```<img src="이미지 주소"/>```
  * src = source

  <details>
    <summary>결과</summary>
    
    ![div](/img/img.png)
    
  </details>

> ```<input>```태그
* ```<input type="" />```
  <details>
    <summary>코드</summary>
    
    ```
    div><input type="text" /></div>
    div><input type="number" /></div>
    <div><input type="password" /></div>
    ```
  </details>

  <details>
    <summary>결과</summary>
    
    ![input](/img/input.png)
    
  </details>

> ```<a>```태그
* 하이퍼링크와 같이 링크를 걸어주는 역할
* ```<a href=""></a>
* href = 하이퍼링크의 준말
* 클릭시 href에 작성한 주소로 이동
  <details>
    <summary>코드</summary>
    
    ```
    <div><a href="https://www.google.com">goto google</a></div>
    ```
  </details>
