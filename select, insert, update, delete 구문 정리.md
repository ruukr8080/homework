# 목차

1. [[SELECT 구문 예제]]
2. [[INSERT 구문 예제]]
3. [[UPDATE 구문 예제]]
4. [[DELETE 구문 예제]]
`
---
# [[SELECT 구문 예제]]

1) **SELECT * FROM** member;   // member에 모든 데이터 조회

 2) **SELECT** name, age **FROM** usertable;   // member테이블의 id,main 칼럼 조회

 4) **SELECT * FROM** member **ORDER BY** age;   // id를 기준으로 오름차순 정렬

 5) **SELECT * FROM** member **ORDER BY** age **DESC**;   // id를 기준으로 내림차순 정렬

6) **SELECT * FROM** member **WHERE** name = 'han';   // name이 han인 데이터 출력

7) **SELECT * FROM** member **WHERE** age < 20;   // age가 20미만인 데이터 출력

8) **SELECT * FROM** member **WHERE** age >= 10 **AND** age <= 20;   // age가 10이상, 20이하인 데이터 출력

9) **SELECT * FROM** member **WHERE** age **IN** (10, 20);   // age가 10 또는 20인 데이터 출력

10) **SELECT * FROM** member **WHERE** name **LIKE** '%a%';   // name에 'a' 단어가 포함된 데이터 출력

---
# [[INSERT 구문 예제]]  

**INSERT INTO** member(name, age) **VALUES** ('han', 20) ;   

// member 테이블에 name은 han, age는 20인 데이터 삽입

---

# [[UPDATE 구문 예제]]

**UPDATE** member **SET** age=30 **WHERE** name='han';   

// member테이블에 name이 han인 칼럼의 age를 30으로 변경

---

# [[DELETE 구문 예제]]

**DELETE** **FROM** member **WHERE** name='han';   

// member 테이블에 name이 han 데이터를 삭제

---

# 추가
- **JOIN (= INNER JOIN) :** 두 테이블을 연결후, 양쪽 테이블에 해당 컬럼이 모두 존재하는 데이터만 출력
- **LEFT OUTER JOIN** : 두 테이블을 연결후, 왼쪽 테이블의 모든 데이터 출력
- **RIGHT OUTER JOIN :** 두 테이블을 연결후, 오른쪽 테이블의 모든 데이터 출력
- **FULL OUTER JOIN :** 두 테이블을 연결후, 양쪽 테이블의 모든 데이터 출력

