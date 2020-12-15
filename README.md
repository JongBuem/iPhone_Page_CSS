# iPhone_Page_CSS

1. CSS

        웹페이지를 보기 좋고 아름답게 꾸며주며, 한번에 여러개의 tag들의 정보를 변경가능하다. 
        유지보수, 가독성, 효울이 상승되며, 코드의 길이를 줄일 수 있다.

2. CSS 작성

        1. html의 hrad 안에 작성하는 방식.
            <head>
              <style>           /*style내에 작성되면 html중에서 CSS라고 알려 주는 것이다.*/
                h1 {            /*전체 h1 tag를 가르키는 '선택자'*/
                    color:red;  /*property[속성] : value[값]*/
                  }
              </style>
            </head>
           
        2. html tag내에 속성에 작성하는 방식.
            <h1 style="color:red"> HI </h> <!-- HI를 빨강색으로 변경 -->
            <h1 style="color:red; text-align:center"> HI </h> <!-- HI를 빨강색으로 위치는 가운데로 변경 -->


3. 선택자
      
        1. id : 유일무의한 값으로 지정된 하나의 tag 
              <style>           
                #jb {                   /*선택자가 id일 경우 앞에 #기호 사용/
                  }
              </style>
              <body>
                <a id="jb"> </a>        /*선택자를 jb로 설정*/
              </body>

        2. class : 부여된 이름이 같은 tag 
              <style>           
                .jb {                   /*선택자가 class일 경우 앞에 .기호 사용*/
                  }
              </style>
              <body>
                <a class="jb jp"> </a> /*선택자를 jb와 jp 2개로 설정가능*/
              </body>              
              
        3. tag : 동일한 tag가 대상
              <style>           
                h1, h2 {                /*모든 h1 과 h2 tag는 대상*/
                  }
              </style>
              <body>
                <h1>page</h1>
                <h2>page</h2>
              </body>
              
        4. * : 모두가 대상
        5. 우선순위 : id - class - tag 순이며 동일할경우는 가장 마지막[최근] 선택자


4. 그리드

        1. 각블록을 나란히 나열 할 수 있다. [caniuse.com은 그리드가 적용되는 브라우저확인]
           그리드는 style 내에 작성한다.
                div {
                     display:grid;                          /*grid단위로 변경*/
                     grid-template-columns: 1fr 1fr 1fr;    /*3개를 3등분 나열*/
                   }
         
        2. 그리드사이 갭의 간격을 설정 할 수 있다.
              grid-gap:50px; 또는 grid-gap:50px 100px;       /*갭의 크기설정*/
              grid-row-gap:50px;                             /*열사이 갭의 크기를 50만큼*/
        
        3. 시작과 끝을 지정가능하다.
             div {
                grid-column-start:1;                         /*첫번째 열에서 시작*/
                grid-column-start:3;                         /*세번째 열에서 끝*/
                }
                
        4. 그리드는 행(row)과 열(column)로 구현될 수 있다.
        
        
4. 반응형디자인

        화면크기에 따라 웹페이지 각 요소들이 반응하여 최적화된 모습으로 변환시키는 것        
        style 내에 작성한다.  [media 쿼리를 사용하며 max는 기준이하, mim는 기준이상]
                @media (max-width:600px) {      /*페이지 크기가 600이하일 경우 반응*/
                  .a{                           
                    display: block;             /*페이지 크기가 600이하일 경우 발생 이벤트*/
                  }
                  .b{
                    border-right:none;          /*페이지 크기가 600이하일 경우 발생 이벤트*/
                  }
                  h1{
                    border-bottom: none;        /*페이지 크기가 600이하일 경우 발생 이벤트*/
                  }
                }

5. link 

       link는 별도의 CSS파일을 다운로드하여 기존에 존재하는 것 처럼 동작시켜준다. 
       link를 사용하면 재사용, 유지보수, 가독성, 사용성이 증가하며 중복성을 감소하는 장점이있다.
       먼저 style tag를 재외한 CSS작성 코드를 별도의 이름의 파일로 저장 (제목.css)
       head tag에 <link rel"stylesheet" href="제목.css"> 작성한다


6. 결론
        
        CSS에서는 선택자와 속성을 많이 알수록 푸부한 표현이가능하다.
        
       
       
       
       
       
       
       
       
       
       
       
       
       
       
       
       
       
