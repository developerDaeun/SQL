# SELECT

- [모든 레코드 조회하기](https://programmers.co.kr/learn/courses/30/lessons/59034)

```sql
-- 코드를 입력하세요
SELECT ANIMAL_ID, ANIMAL_TYPE, DATETIME, INTAKE_CONDITION, NAME, SEX_UPON_INTAKE
FROM ANIMAL_INS
ORDER BY ANIMAL_ID; -- 오름차순 정렬
```

- [역순 정렬하기](https://programmers.co.kr/learn/courses/30/lessons/59035)

```sql
-- 코드를 입력하세요
SELECT NAME, DATETIME
FROM ANIMAL_INS
ORDER BY ANIMAL_ID DESC; -- DESC : 내림차순 정렬
```

- [아픈 동물 찾기](https://programmers.co.kr/learn/courses/30/lessons/59036)

```sql
-- 코드를 입력하세요
SELECT ANIMAL_ID, NAME
FROM ANIMAL_INS
WHERE INTAKE_CONDITION = "Sick"
ORDER BY ANIMAL_ID;
```

- [어린 동물 찾기](https://programmers.co.kr/learn/courses/30/lessons/59037)

```sql
-- 코드를 입력하세요
SELECT ANIMAL_ID, NAME
FROM ANIMAL_INS
WHERE INTAKE_CONDITION != "Aged"
ORDER BY ANIMAL_ID;
```

- [동물의 아이디와 이름](https://programmers.co.kr/learn/courses/30/lessons/59403)

```sql
-- 코드를 입력하세요
SELECT ANIMAL_ID, NAME
FROM ANIMAL_INS
ORDER BY ANIMAL_ID;
```

- [여러 기준으로 정렬하기](https://programmers.co.kr/learn/courses/30/lessons/59404)

```sql
-- 코드를 입력하세요
SELECT ANIMAL_ID, NAME, DATETIME
FROM ANIMAL_INS
ORDER BY NAME, DATETIME DESC; -- 이름은 오름차순, 날짜는 내림차순
```

- [상위 n개 레코드](https://programmers.co.kr/learn/courses/30/lessons/59405)

```sql
-- 코드를 입력하세요
SELECT NAME
FROM ANIMAL_INS
ORDER BY DATETIME -- 가장 먼저 보호소에 들어온 동물순으로 오름차순
LIMIT 1; -- 하나만 출력
```

