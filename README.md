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
                #jb { /*선택자가 id일 경우 앞에 #기호 사용/
                  }
              </style>
              <body>
                <a id="jb"> </a> /*선택자를 jb로 설정*/
              </body>

        2. class : 부여된 이름이 같은 tag 
              <style>           
                .jb { /*선택자가 class일 경우 앞에 .기호 사용*/
                  }
              </style>
              <body>
                <a class="jb jp"> </a> /*선택자를 jb와 jp 2개로 설정가능*/
              </body>              
              
        3. tag : 동일한 tag가 대상
              <style>           
                h1, h2 { /*모든 h1 과 h2 tag는 대상*/
                  }
              </style>
              <body>
                <h1>page</h1>
                <h2>page</h2>
              </body>
              
        4. * : 모두가 대상
        5. 우선순위 : id - class - tag 순이며 동일할경우는 가장 마지막[최근] 선택자


4. 선택자
        
        
        
        
        
        
        
              
