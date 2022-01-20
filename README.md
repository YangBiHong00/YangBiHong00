회원테이블
    아이디
	회원이름
	주소
제품 테이블
    제품이름
	가격
	제조일자
	제조회사
	남은 수량

모델링

Shop 스키마 생성
접속 생성 SqlDeveloper

테이블 생성 (DDL)

아이디는 영문 8자
회원이름 한글 5자
주소 20글자



create index idx_indexTBL_firstname ON indexTBL(first_name);


select * from indexTBL; where First_name = 'Jack';
3번째 아이콘 계획 실행


CREATE TABLE Shop.indexTBL
AS
   SELECT first_name, last_name, hire_date
   FROM HR.employees;
   
   create view shop.membertbl_view as
 select memberName, memberAddress FROM shop,membertbl;
 


-- 스토어드 프로시저
select count(*) from memberTBL;
select count(*) from producttbl;
