# SpringBoot Project
* 도서 구매 및 중고거래 플랫폼

## 📌 담당 기술 구현 - 안영준 
1) BootStrap 을 이용한 반응형 웹 디자인 메인 및 전체파트별 디자인 적용
2) 메인 베너 및 이벤트 베너/아이콘 제작 
3) 회원 및 게시판 / 마이페이지
   * 회원가입
     - 아이디 중복 확인,주소API사용, 각 input 별 유효성 검사 후 회원가입  <br>
       추천인 입력시 추천인 포인트지급, 포인트 리스트에 업데이트
   * ID 찾기
     - 이메일, 핸드폰 번호 인증후 회원정보 찾기. 문자전송 API 와 이메일전송 객체 사용  <br>
       가입된 회원만 인증번호전송, 랜덤인증번호 와 입력인증번호 일치시 ID 및 정보 조회 
   * 게시판 리스트
     - 게시글 리스트 , 비밀 글 일시 로그인된 관리자와 본인만 조회할수 있도록 구현, 페이징 처리  <br>
     관리자의 게시글 일시 작성자 관리자 로 표기 
   * 게시글 등록
     - 로그인된 회원의 기본 정보를 출력하고 입력받은 게시글 등
   * 게시글 상세
     - 비밀글 일시 로그인된 관리자와 본인만 조회가능 , 일반글 비 로그인시에도 조회가능 처리
   * 관리자 1:1 문의
     - 로그인된 회원의 기본 정보를 출력, 입력받은 문의를 관리자의 이메일로 전송
   * 댓글 전체조회/등록/댓글추천/댓글신고
     - 해당 게시글에 전체댓글조회,댓글 등록, 각 댓글마다 Ajax 사용 댓글 추천, 댓글 신고기능 (15회 신고 누적시 자동삭제)
      <br>
   * 마이페이지 > 회원정보 수정
     - 회원 정보(이메일, 휴대전화, 주소) 변경 , 회원 아이콘 일러스트 이미지 변경 
   * 마이페이지 > 리뷰 조회
     - 상품, 리뷰 테이블을 참조해 join문 을 이용한 해당 상품에 내가 작성한 리뷰 조회
   * 마이페이지 > 주문 현황 조회
     - 상품, 주문, 주문상세 테이블을 참조해 join 문을 이용한 내 주문 리스트 조회
   * 마이페이지 > 내 게시글 조회 / 수정 
     - 로그인된 회원의 기본정보를 출력, 내가 남긴 게시글 조회, 수정, 삭제 한페이지에서 개별 처리  <br>
       게시글 삭제시 해당 게시물은 삭제된 게시물로 표기 
   * 마이페이지 > 내 댓글 조회 / 수정 / 삭제
     - 회원, 게시글, 댓글 테이블 참조 join 문을 이용해 내가 작성한 댓글 조회,수정 및 삭제 구현  <br>
       댓글 수정시 (수정) 표기
       
4) 관리자 페이지
   * 회원의 관리자 여부를 통해 관리자 페이지 접근권한 부여
   * 관리자 > 관리자 메인 전체 회원 분석/통계
     - 관리자 메인 회면에 회원별 관리자 / 회원 / 탈퇴회원 / 활동중인 회원 차트 그래프 라이브러리로 통계 분석표 구현
   * 관리자 > 회원관리 >  전체회원 조회 / 검색
     - 전체 회원 정보조회, 페이징처리, 검색 기능 구현, Ajax 로 간편주소 조회 기능 구현
   * 관리자 > 회원관리 >  회원 상세 조회 / 수정 / 삭제 
     - 개별 회원 클릭시 회원의 상세 조회, 수정, 삭제 및 아이콘 변경, 탈퇴처리(로그인제한) 기능 구현 
   * 관리자 > 신고 게시글 조회 / 삭제
     - 전체 게시글 중 신고처리된 게시글 관리 , 신고사유와 신고 횟수 조회 및 삭제기능 구현  <br>
       관리자가 게시글 삭제시 게시글에 달린 댓글또한 삭제 
   * 관리자 > 신고 댓글 조회 / 수정 / 삭제
     - 전체 댓글 중 신고 댓글 관리 , 신고사유와 신고 횟수 조회 및 신고 횟수 초기화 혹은 삭제기능 구현

## 📰 UI
* 메인 화면
  - 비 로그인
  ![image](https://github.com/ayj8487/DADOK/assets/78454625/d97195d0-840d-464a-8f6c-05c9b13063dd)

  - 로그인시 
  ![image](https://github.com/ayj8487/DADOK/assets/78454625/537aff49-83dc-4a0a-b341-5fca8d50e359)
* 회원가입
  ![image](https://github.com/ayj8487/DADOK/assets/78454625/b664be6d-3748-4ebb-a929-9c3b6f8862e0)
  ![image](https://github.com/ayj8487/DADOK/assets/78454625/4e08570b-55c2-42ba-8914-0a24fe23d773)
* 회원정보 찾기
  ![image](https://github.com/ayj8487/DADOK/assets/78454625/6c4d5af8-7803-4fbc-a4ee-f3edfaf68caa)
  ![image](https://github.com/ayj8487/DADOK/assets/78454625/26f72cdd-909f-421b-bf55-9bd2d6561758)
  ![image](https://github.com/ayj8487/DADOK/assets/78454625/0c98c1a8-c007-4a3b-acfc-939fb0ac2e26)
  ![image](https://github.com/ayj8487/DADOK/assets/78454625/fdf7c79a-64c5-4ee3-9969-1b5baebd1dc5)
* 자유게시판
  ![image](https://github.com/ayj8487/DADOK/assets/78454625/56c47969-b75f-445d-a579-93853f42fa90)
  ![image](https://github.com/ayj8487/DADOK/assets/78454625/7f97feaa-bcf1-4d4b-b2ae-556032af8f72)
  ![image](https://github.com/ayj8487/DADOK/assets/78454625/b6263d73-68da-4bb1-9c61-57b90d8b6697)
  ![image](https://github.com/ayj8487/DADOK/assets/78454625/bb1502dc-3efe-4f1c-b8c5-b24cb7ea5632)
  ![image](https://github.com/ayj8487/DADOK/assets/78454625/d7120cd6-f8bf-4d7a-96dc-8077f84ebace)
* 1:1 문의
  ![image](https://github.com/ayj8487/DADOK/assets/78454625/36719e3a-4d60-4173-8e0e-fe657b8a9b12)
* 마이페이지
  ![image](https://github.com/ayj8487/DADOK/assets/78454625/085d3957-86ed-434a-aaea-209bc72353b9)
* 주문현황
  ![image](https://github.com/ayj8487/DADOK/assets/78454625/72509bbf-eae5-417d-a83d-12ab94eae666)
* 내정보
  ![image](https://github.com/ayj8487/DADOK/assets/78454625/4a7f16bd-2010-447b-9ddc-b0a71f8241cb)
  ![image](https://github.com/ayj8487/DADOK/assets/78454625/97eebccf-4f8b-4c73-943e-be57717799ec)
* 내게시글
  ![image](https://github.com/ayj8487/DADOK/assets/78454625/b4d084b8-99fb-42ac-9683-af1f748c1189)
* 내댓글
  ![image](https://github.com/ayj8487/DADOK/assets/78454625/d3ce080b-73b6-4c2d-9f2a-540af57481ed)

* 관리자 메인
  ![image](https://github.com/ayj8487/DADOK/assets/78454625/7d4ff66e-c516-4c09-a3bf-9be26dbdb8c9)

* 회원관리
  ![image](https://github.com/ayj8487/DADOK/assets/78454625/7e2f8445-d8aa-4faa-a0de-fad09d0f1abb)

* 회원상세
  ![image](https://github.com/ayj8487/DADOK/assets/78454625/8945d2fe-4c7d-4567-9617-23f3e8d50aa3)
  ![image](https://github.com/ayj8487/DADOK/assets/78454625/dee7202f-df2c-4292-86ff-6db49b1ad9b3)

* 신고관리
  ![image](https://github.com/ayj8487/DADOK/assets/78454625/db1a6506-f647-41c7-885d-a765b25c8e33)

       
## ⏰ 개발 기간
* 2023.10.27 ~ 2023.11.29

## 🖥️ 개발 환경
* Java 11.0.12
* STS 2.7.17
* Oracle 11.2.0.2.0
* JDBC 8   

