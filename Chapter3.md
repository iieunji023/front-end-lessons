## 정리
### HTML태그에 스타일을주는 방법🔗

1. HTML 태그에 직접주는 방법 (앞으로 다룰 예정)
```
div {

  color:red;

}
```

* 어떤 **태그에 공통적인 스타일을 주고싶을 때** 사용하는 방법 

2. id 를 이용해 주는방법

```
#new-style {

color:red;

}
```

* class 와 사용방식이 비슷하지만 **한번에 하나의 스타일만** 줄수있음, **주로 자바스크립트에서 많이 쓰이고** 스타일링에는 많이 안쓰이는 방식

3. class를 이용해 주는 방법 (강의에서 사용된 방법)

```
.new-style {

color:red;

}
```

* **한번에 여러개의스타일**을 줄수있다. 제일 많이 쓰이는 방법 


4. 복합 선택자

> 일치 선택자:**두가지 조건을 동시에 만족**하는 요소 선택 

```
div.new-style{

      /*div태그에 new-style클래스

}
```

> 자식선택자

```
div>.new-style{

  /* div의 자식요소중 class="new-style"선택

}
```

> 후손 선택자

```
div .new-style{

/* div 후손요소들 중에서 class="new-style"

}
```

  <details>
    <summary>코드_html</summary>
    
    <!DOCTYPE html>
    <html lang="en">
    <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>Document</title>
      <link href="/chapter3/css/style.css" rel="stylesheet" type="text/css" />
    </head>
    <body>
      <div class="red border-blue">BTS</div>
      <img src="https://pbs.twimg.com/media/E_OPRLmVIAEXVPr.jpg" class="img-size"/>
      <div class="border-blue img-size margin-space padding-space">BOX</div>
    </body>
    </html>
  </details>

  <details>
    <summary>코드_css</summary>
    
    .red {
      color: red;
      background-color: yellow;
      text-align: center;
    }

    .border-blue {
      border: 1px solid blue;
    }

    .img-size {
      width: 200px;
      height: 200px;
    }

    .margin-space {
      margin-top: 40px;
      margin-left: 100px;
    }

    .padding-space {
      padding-top: 40px;
    }
  </details>

  <details>
    <summary>결과</summary>
    
  ![css](/img/css.png)
    
  </details>

### chapter3: 과제1
  <details>
    <summary>코드_html</summary>
    
    <!DOCTYPE html>
    <html lang="en">
    <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>Document</title>
      <link href="../css/style_hw1.css" rel="stylesheet" type="text/css" />
    </head>
    <body>
      <div>  
        <div class="box">Box 1</div> 
        <div class="box green">Box 2</div>  
        <div class="box blue">Box 3</div> 
    </div>
    </body>
    </html>
  </details>

  <details>
    <summary>코드_css</summary>
    
    .box {
      border: 50px solid red;
      width: 200px;
      padding: 50px;
      margin-bottom: 20px;
    }

    .green {
      border: 50px solid green;
      /* display:none; */
      visibility:hidden
    }

    .blue {
      border: 50px solid blue;
    }
  </details>

  <details>
    <summary>결과</summary>
    
  ![hw1](/img/hw1.png)
    
  </details>

  > [display:none과 visibility:hidden의 차이](https://unabated.tistory.com/entry/displaynone-%EA%B3%BC-visibilityhidden-%EC%9D%98-%EC%B0%A8%EC%9D%B4)
  * display:none  <-> block
    * 아예 사라지게 하는 것. 보이지도 않고 해당 공간도 존재하지 않게 됨
  <details>
    <summary>display:none</summary>
    
  ![hw1](/img/display.png)
    
  </details>

  * visibility:hidden <-> visible
    * 보이지만 않고 해당 공간은 존재. width와 height 값을 주었다면 그만큼 공간은 존재하게 됨
  <details>
    <summary>visibility:hidden</summary>
    
  ![hw1](/img/visibility.png)
    
  </details>
  
