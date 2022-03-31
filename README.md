<h1>끊임 없이 배우고 싶은 신입 개발자 조연하 입니다.</h1>

## Intro
>+ name : 조연하
>+ tel : 010.5138.1950
>+ email : <whdusgk0605@naver.com>
<br>

## Project 
> ### <b>Hello,Traveler<b> (4인 팀 프로젝트)<br>
>개발기간 : 2021.12.01 ~ 2022.02.27 <br>
><br>
> 여행을 좋아하는 사람들을 위한 여행커뮤니티<br>
> 유저들과 여행에 관한 여러 소통을 주고 받을 수 있으며, 여행사 기업을 통해 여행 상품을 판매 합니다.<br>
> <br>
>:punch: <b>주요 사용기술</b> :punch:<br>
><br>
><img src="https://img.shields.io/badge/java-007396?style=for-the-badge&logo=java&logoColor=white"></a>
><img src="https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white"></a>
<img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"></a>
<img src="https://img.shields.io/badge/css-1572B6?style=for-the-badge&logo=css3&logoColor=white"></a>
<img src="https://img.shields.io/badge/spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white"></a>
<img src="https://img.shields.io/badge/JSON-000000?style=for-the-badge&logo=JSON&logoColor=white"></a>
<img src="https://img.shields.io/badge/Apache-D22128?style=for-the-badge&logo=Apache&logoColor=white"></a><br>
<img src="https://img.shields.io/badge/Apache Tomcat-F8DC75?style=for-the-badge&logo=Apache Tomcat&logoColor=white"></a>
<img src="https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=Oracle&logoColor=white"></a>
<img src="https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jQuery&logoColor=white"></a>
<img src="https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jQuery&logoColor=white"></a>
<img src="https://img.shields.io/badge/API-000000?style=for-the-badge&logo=API&logoColor=white"></a>
<br>


### 맡은 파트
>
>+ 회원가입 폼 입력 제한조건 :heavy_check_mark: [코드확인](https://github.com/YHDA0605/Portfolio/blob/604d63884ef6e3312068a31fe026e144644c1a9c/src/main/webapp/resources/js/regist.js#L83)
>+ 회원탈퇴 :heavy_check_mark: [코드확인](https://github.com/YHDA0605/Portfolio/blob/9dc1823fb54c116b299e9556d76acb2863367934/src/main/java/com/teamHT/helloTraveler/HomeController.java#L256)
>+ Kakao 로그인 API  :heavy_check_mark: [코드확인](https://github.com/YHDA0605/Portfolio/blob/68cb76ff3250b539c1f522f3594d4ad9b99d9fb8/src/main/java/com/teamHT/helloTraveler/KakaoController.java#L1)
><details>
><summary><b>트러블 슈팅</b></summary>
>:interrobang: kakao로그인 API 사용시 sns으로 로그인을 하면 api 에서 자동적으로 고유한 회원번호 10자리(id)가 주어져 이 id로 로그인을 실행 시켜야 하는데 
>기존 members 테이블에 있는 mem_id칼럼이 유니크&NotNull 로 지정 해뒀기 때문에 
>무조건적으로 mem_id 가 들어가지 않으면 안되는 상황이었다.
><br>
><br>
>:rainbow:해결방법
>sns 가입을 할때 회원 등록 service 에서  mem_id 칼럼에 값을 넣기 위해 임의로 "sns" 문자열을 넣고 maxcode로 db에서 회원수를 카운트해 회원이 추가 될때마다
>숫자가 하나씩 올라가는 방식으로 로직을 짜서 "sns" 문자열과 maxcode 를 합쳐 유니크와 NOTNULL의 조건을 충족시키는 sns가입 회원을 위한 mem_id 를 만들었다.
>:heavy_check_mark: [코드확인](https://github.com/YHDA0605/Portfolio/blob/371fe61c141fd2aa13d2c596f032c2e012abddd9/src/main/java/com/teamHT/helloTraveler/Svc/MembersServiceImpl.java#L229)
></details>
