# TREND_EATER

국비 교육과정에서 수행한 최종 팀 프로젝트

제품 구매 및 매출에 대한 영향력 등 리뷰의 중요성이 증가하고 있습니다. 
또한 새로운 식품이 출시되면 해당 식품에 대한 정보가 부족하여 소비자가 접근하기 어려운 실정.
그래서 이러한 점들을 고려하여 실제 소비자 리뷰들을 중심으로 식품을 소개하여 소비자에게 다양한 정보를 제공하고 식품 정보에 대한 신뢰성을 제고 하기 위하여 사이트를 개발하게 되었습니다.
회원 페이지와 관리자 페이지 영역을 구분하였으며, 모든 게시판의 CRUD는 관리자 페이지에서 할 수 있도록 구현하였습니다.
회원은 상품을 구매할 수 있습니다. 그리고 관심상품을 스크랩 할 수 있으며, 상품에 리뷰를 작성하고  작성된 리뷰에 좋아요를 표현할 수 있습니다. 문의를 작성 할 수 있고, 원하는 상품 등록을 요청 할 수 있으며, 시식 신청이 진행 중인 상품에 대하여 신청 가능합니다.
마이페이지에서 관심상품 / 작성리뷰 / 관심리뷰 등을 확인 할 수 있습니다.

## 주요 기능

- **회원 가입 및 로그인**
    - 카카오 소셜 로그인 및 일반 로그인
    - 아이디 및 비밀번호 찾기
    - Bcrypt 비밀번호 암호화
    - Interceptor를 사용하여 로그인 인증 체크를 구현하여 미로그인시 로그인이 필요한 서비스에 접근하면 로그인 페이지로 이동

- **마이페이지**
    - 프로필 사진 추가 / 수정 기능
    - 개인정보 조회 및 수정(비밀번호 포함) 기능
    - 나의 시식 신청 목록 확인
    - 내가 작성한 리뷰 목록 확인 및 삭제
    - 내가 좋아요 한 리뷰 목록 확인 및 좋아요 취소
    - 스크랩(찜)한 상품 목록 확인 및 해당 상품 게시글 바로가기
    - 출석체크, 출석체크 시 포인트 지급, 출석 현황
    - 포인트 적립 및 사용 현황 확인 게시판
    - 주문 내역 및 내역 상세보기 확인

- **게시판**
    - 제품 및 리뷰 게시판
        - 리스트 페이징 처리
        - 상품 등록 요청 기능
        - 리스트 최신 / 리뷰 / 스크랩 순 정렬 기능
        - 상세보기 스크랩 기능
    - 시식 신청 게시판
        - 리스트 페이징 처리
        - 시식 신청하기 기능
        - 해당 제품 보기 기능
    - 이벤트 게시판 리스트 및 상세보기 / 페이징 처리
    - 공지사항 게시판 리스트 및 상세보기 / 페이징 처리
    - 문의사항 게시판 리스트 CRUD / 페이징 처리

- **구매**
    - 장바구니 기능
    - iamport API를 이용한 결제 기능

- **상품 검색**
    - 메뉴바에 상품명을 통한 검색 기능

- **리뷰**
    - 제품 리뷰 작성(평점, 좋은점, 아쉬운점, 사진업로드 )
    - 리뷰 신고 기능
    - 리뷰 좋아요 기능
    - 리뷰 정렬 기능

- **관리자 페이지**
    - 회원 리스트 / 회원 정보 엑셀 다운로드 / 회원 탈퇴 / 회원검색 기능
    - 상품 관리
        - 상품 CRUD / 시식 등록  / 제품 및 리뷰게시판 게시 및 삭제 기능
        - 상품명 검색 기능
        - 상품명 / 재고량 / 게시일 순 정렬 기능
        - 페이징 처리
    - 제품 및 리뷰 게시판 관리
        - 제품 및 리뷰 게시판 CRUD
        - 상품명 검색 기능
        - 상품명 / 리뷰 / 스크랩 순 정렬 기능
        - 페이징 처리
    - 리뷰 관리
        - 전체 리뷰 목록 확인 및 삭제 기능
        - 최신순 / 오래된순 / 좋아요순/ 높은평점 순 / 낮은평점 순 정렬 기능
        - 페이징 처리
    - 상품 요청 관리
        - 상품 요청 리스트 확인
        - 상품명 / 제조사명 등 검색 조건에 따른 검색 기능
        - 상품명 / 요청일/ 요청번호 순 정렬 기능
        - 페이징 처리
    - 시식 신청 게시판 관리
        - 상품관리 게시판에서 등록한 시식 신청 리스트 수정/ 삭제 / 게시 / 시식 종료 기능
        - 상품명 검색 기능
        - 신청 / 최신 / 상품명 / 마감일 순 정렬 기능
        - 페이징 처리
    - 시신 신청 리스트 관리
        - 시식 신청 게시판에서 신청한 신청자 리스트 확인
        - 상품명 / 아이디 / 이름 등 검색 조건에 따른 검색 기능
        - 신청번호/ 신청일 / 상품명순 정렬 기능
        - 페이징 처리
    - 이벤트 게시판  CRUD 및 페이징 처리
    - 공지사항 게시판 CRUD 및 페이징 처리
    - 1:1 문의 게시판 관리
        - 문의사항 리스트 확인 및 답변 등록 / 삭제 기능
        - 페이징 처리
    - 주문 관리
        - 주문 현황 확인 및 주문 상태 변경
        - 주문 상세보기
        - 주문 상태별 카테고리 모아 보기
        - 페이징 처리
    - 신고 리뷰 목록 관리
        - 해당 리뷰 삭제 기능
        - 신고 확인 기능
        - 최신순 / 오래된순/ 신고종류 순 정렬 기능
        - 페이징 처리


## 사용 기술

- JAVA 8/ Spring MVC / MyBatis / Bcrypt / Apache Tomcat 9.0 / Oracle 11g / SQL Developer
- HTML5 / CSS3 / jQuery / JS
- Kakao Login API / iamport API
- Github




## 담당 개발 내용

**프로젝트 협업을 위한 Git Project 생성 및 관리**

**DB 모델링 및 DB관리**

**메인 페이지 및 이벤트 게시판 디자인**
- 이벤트 배너 슬라이드, 신상품/평점/리뷰좋아요 등의 기준에 따른 상품을 슬라이드로 구현

**마이 페이지 내 스크랩 디자인 및 기능**
- 회원이 스크랩 한 상품에 리스트를 DB에서 불러와 출력하고 바로가기를 통해 해당 상품 상세페이지로 이동 구현

**상품 검색 기능**
- 메뉴바 검색창을 통해 상품명으로 원하는 상품을 검색하여 확인 가능

**리뷰 DML 시 상품 리뷰 평점 계산 및 리뷰 갯수 카운트 트리거**
- 리뷰 게시물 테이블에 DML이 실행될 때마다 해당 제품에 대한 8가지 항목의 점수 평균을 상품정보 테이블에 update 하고 제품 및 리뷰 게시판 테이블의 리뷰수 칼럼을 update 하는 트리거 사용

**스크랩 / 시식 신청 / 좋아요 카운트 트리거**
- 스크랩 / 좋아요 테이블에 insert 또는 delete 실행시 제품 및 리뷰게시판 테이블의 스크랩수와 레뷰 게시물의 좋아요수 컬럼을 update하는 트리거 사용
- 회원이 시식 신청(시식신청 테이블에 insert 실행) 시 시식 게시판 테이블의 신청자 수 컬럼을update하는 트리거 사용

**제품 및 리뷰 게시판 디자인 및 기능**
- 리스트 페이징 처리
- 상품 등록 요청 기능 : 모달창을 사용하여 회원이 입력한 정보를 DB에 저장
- 리스트 최신 / 리뷰 / 스크랩 순 정렬 기능
- 상품 리스트에서 해당 상품에 대한 리뷰 갯수를 확인 가능하도록 구현
- 제품 및 리뷰게시판 등록 후 7일이 지나면 신제품 라벨이 자동으로 사라지도록 구현
- 스크랩 기능
    - 상세보기 화면의 스크랩(하트) 버튼을 클릭하면 ajax를 활용하여 스크랩 테이블에 해당 제품과 회원을 insert하고 버튼을 변경(하트 색상)하도록 구현
    - 또한 상세보기 화면에서 스크랩 한 제품과 하지 않은 제품이 구분되어 출력되도록 구현
- 제품 리뷰 평점 구현
    - 상세보기 화면에서 평균만족도/추천의사/재구매의사 등에 대한 평균점수에 따라 이모티콘이 다르게 출력 되도록 구현하였으며, 각 항목의 점수에 대한 응답자수의 비중을 표현
    - HighChart를 사용하여 5가지 맛에 대한 점수를 차트로 구현
- 리뷰 좋아요 기능
    - ajax를 활용하여 제품의 리뷰목록에서 좋아요를 클릭 시 좋아요 테이블에 리뷰번호와 회원 아이디를 insert하고 좋아요 아이콘의 색상이 변경되도록 구현
    - 리스트에서 좋아요한 리뷰와 그렇지 않은 리뷰의 아이콘이 구분되어 출력되도록 구현

**시식 신청 게시판 디자인 및 기능**
- 리스트 페이징 처리
- 시식 신청하기 기능
    - 모달창을 사용하여 회원이 입력한 정보를 DB에 저장하고 이미 신청한 제품의 경우 신청하였다는 alert창 출력
- 해당 제품의 상세 페이지로 이동 할수 있도록 구현
- 각 시식 신청 상품에 대하여 마감 D-Day 카운트가 적용되어 신청 마감까지 얼마의 시간이 남았는지 실시간으로 표시되고 현재 신청자수를 출력하도록 구현
- 마감일시가 지나면 자동으로 신청종료 문구가 해당 요소 위에 생성되어 클릭이 안되도록 구현

**상품 관리**  
- 상품 CRUD / 제품 및 리뷰게시판 게시 기능 / 시식 등록
    - 상품 등록 기능을 통해 상품 등록 페이지로 이동하여 상품 등록에 필요한 정보를 입력하고 이미지를 업로드(이미지 미리보기 구현) 하여 DB에 저장
    - 수정하기 기능을 통해 상품의 정보와 이미지가 화면에 출력되고 이미지는 해당 이미지를 클릭하여 새로운 파일을 업로드하면 해당 이미지가 수정되도록 구현
    - 삭제 기능을 통해 해당 상품이 관리 게시판과 제품 및 리뷰게시판에서 모두 삭제되도록 구현
    - 상품 등록 후 ajax를 활용한 제품 게시 토글기능을 통해 제품 및 리뷰게시판에 상품이 게시 여부 결정
    - 시식 등록 버튼을 통해 신청 종료일을 입력 후 DB에 저장하면 시식 게시판 관리 페이지로 이동되며 시식 신청 게시판에 해당 상품이 게시되도록 구현
- 오라클 FUNCTION을 활용하여 상품 등록 / 수정  / 삭제시 상품 테이블과 상품게시판 테이블을 한번에 처리 하도록 구현
- 검색창에 상품명을 입력하여 원하는 상품을 검색할 수 있도록 구현
- 상품명 / 재고량 / 게시일 순 정렬 기능
- 페이징 처리

**제품 및 리뷰 게시판 관리** 
- 제품 및 리뷰 게시판 수정 삭제
    - 제품 및 리뷰게시판에 등록된 게시물 리스트 현황을 DB에서 불러와서 출력
    - 수정 및 게시 기능은 상품관리와 동일
- 검색창에 상품명을 입력하여 원하는 상품을 검색할 수 있도록 구현
- 상품명 / 리뷰 / 스크랩 순 정렬 기능
- 페이징 처리

**상품 요청 관리**
- 상품 요청 리스트 확인
- 상품명 / 제조사명 등 검색 조건을 선택하여 검색어에 따른 검색 기능 구현
- 상품명 / 요청일/ 요청번호 순 정렬 기능
- 페이징 처리

**시식 신청 게시판 관리**

- 상품관리 게시판에서 등록한 시식 신청 리스트 수정/ 삭제 / 게시 / 시식 종료 기능
    - 시식 등록한 상품에 대한 정보를 DB를 통해 불러와서 출력
    - 수정 기능을 통해 신청 종료일 및 진행상황(진행 또는 종료) 변경 가능
    - 삭제 기능을 통해 관리자 게시판과 회원게시판에서 모두 삭제 가능
    - ajax를 활용한 게시여부 토글 기능을 통해 시식 신청 게시판의 게시여부 결정
- 검색창에 상품명을 입력하여 원하는 상품을 검색할 수 있도록 구현
- 신청 / 최신 / 상품명 / 마감일 순 정렬 기능
- 페이징 처리

**시신 신청 리스트 관리**

- 시식 신청 게시판에서 신청한 신청자 리스트 확인
- 상품명 / 아이디 / 이름 등 검색 조건을 선택하여 검색어에 따른 검색 기능 구현
- 신청번호/ 신청일 / 상품명순 정렬 기능
- 페이징 처리
