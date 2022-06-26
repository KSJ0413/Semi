# SemiProject

### 1, 로그인 페이지 
 - 아이디 찾기 (비동기, 이름, 이메일 -> 아이디)
 - 패스워드 찾기 (비동기, 아이디, 이름 -> 패스워드)

### 2. 나의정보 -> 사진수정 기능 추가 

### 3. 관리자페이지 -> 상품조회(read)  추가

### 4. 상품상세페이지에서 -> review 기능 추가하기 (댓글 기능 참조)
   - review 테이블 생성 
   create table review(
   rnum int not null auto_increment primary key,
   content varchar(500) not null,
   regdate date not null,
   id varchar(10) not null,
   contentsno int(7) not null,
   foreign keycontentsno references contents(contentsno)
);
   - 로그인해야 댓글 쓰기, 본인이 쓴 댓글만 지우고,수정

### 5. community -> Notice 기능 생성 (notice 참조)
   - 생성,수정,삭제 => 관리자
   - 목록, 조회 => 모두


   #### 여기까지만 했습니다.
------------- 
6. 상품 detail 페이지에서 장바구니 추가기능 및  
    장바구니 목록 생성
 - cart 테이블 생성

7. 상품 detail 페이지에서 주문생성 기능 만들기 및
    주문 목록 , 주문 조회(read) 생성 
