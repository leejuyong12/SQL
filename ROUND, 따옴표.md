반올림 원할때 ROUND 사용

ROUND(대상, 0)  -  0은 소수점 포함 안되게(소수 첫번째 자리에서 반올림)

ROUND(대상)  - 이렇게만 해도 소수점 포함 안되게 소수 첫번째자리에서 반올림한다.(default 값)

```sql

-- MySQL

SELECT ROUND(AVG(DAILY_FEE),0) AS 'AVERAGE_FEE'
FROM CAR_RENTAL_COMPANY_CAR
WHERE CAR_TYPE = 'SUV';


-- Oracle

SELECT ROUND(AVG(DAILY_FEE),0) AS AVERAGE_FEE -- 홑따옴표 불가능, 쌍따옴표 가능
FROM CAR_RENTAL_COMPANY_CAR
WHERE CAR_TYPE = 'SUV'; -- 홑따옴표 가능, 쌍따옴표 불가능
```



(')홑따옴표 : 문자열을 감싸주는 기호
(")쌍따옴표 : 컬럼명 등을 감싸주는 기호

 

컬럼명을 쓸때는 쌍따옴표, 문자열은 홑따옴표 !



