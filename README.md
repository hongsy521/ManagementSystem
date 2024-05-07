과제 주제 : 내배캠 스프링 수강생들을 관리하는 프로그램


<요구사항 정의>
필수과목 : Java 객체지향 Spring JPA MySql
선택과목 : 디자인패턴, Spring Security, Redis, MongoDB

최소 3개 이상의 필수과목, 2개 이상의 선택과목을  선택
캠프기간동안 선택한 과목별로 총 10회 시험을 본다
캠프매니저는 수강생들을 등록 및 관리
캠프매니저는 수강생들의 과목과 시험점수를 등록 및 관리
점수 데이터 타입 : 정수형, 점수에 따라 등급이 매겨진다
필수과목 등급산정기준 : A(95~100) / B(90~94) / C(80~89) / D(70~79) F(60~69) / N (~59)
선택과목 등급산정기준 : A(90~100) / B(80~89) / C(70~79) / D(60~69) F(50~59) / N (~49)

<필수요구사항>
1. 수강생관리 : 고유번호 중복x
- 수강생 정보 등록 : 고유번호, 이름, 과목목록
- 수강생 목록 조회 : 고유번호, 이름 (출력 형식 자유, 고유번호+이름 조회)

2. 점수관리
- 등록하려는 과목의 회차 점수가 이미 등록되어있다면 등록할 수 없다. (등록할 때는 덮어쓸수 없고, 점수수정 필요하면 2-3 기능을 활용해서 수정해야함)
- 회차는 1~10으로 제한한다
- 점수는 0~100으로 제한한다
1) 수강생의 과목별 시험회차 및 점수를 등록
- 점수를 등록하면 자동으로 등급 추가 저장 (점수만 적으면 등급 자동계산)
2) 수강생의 과목별 회차 점수를 수정할 수 있다
3) 수강생의 특정 과목 회차별 등급을 조회할 수 있다 (출력 형식 자유, 회차+등급 조회)

<추가요구사항>
1) 수강생 상태 관리(상태종류 : Green Red Yellow) : 그냥 기분같은거 말하는듯
2) 수강생 정보 조회(출력 형식 자유, 고유번호+이름+상태+선택한과목명 조회)
3) 수강생 정보 수정(이름, 상태 수정기능)
4) 상태별 수강생 목록 조회 (조회조건 추가)
5) 수강생 정보 삭제(점수기록도 같이 삭제)
6) 수강생의 과목별 평균 등급 조회(출력 형식 자유, 과목명+평균등급 조회)
7) 특정 상태 수강생들의 필수 과목 평균 등급 조회(출력 형식 자유, 수강생이름+필수과목평균등급 조회)
