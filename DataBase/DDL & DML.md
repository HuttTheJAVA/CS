### DDL (DATA DEFINITION LANGUAGE)

```
DDL은 SQL의 하위 집합으로 테이블, 뷰, 인덱스, 프로시저 같은 개체를 정의하는데 사용된다.
예로 CREATE , ALTER, DROP, TRUNCATE, RENAME 등이 있다.
```

- **CREATE** : 테이블, 뷰, 인덱스와 같은 데이터베이스 개체를 만들 때 쓰는 키워드
- **ALTER** : 기존에 생성된 개체를 수정하는데 사용되는 키워드
- **DROP** : 개체를 삭제하는데 사용되는 키워드
- **TRUNCATE** : 테이블의 구조와 인덱스는 유지하되 테이블 모든 행을 삭제하는 키워드
- **RENAME** : 개체의 이름을 바꾸는 데 사용되는 키워드
<br></br><br></br>
### DML (DATA MANIPULATION LANGUAGE)

```
DML은 SQL의 하위 집합으로 데이터베이스 내의 데이터를 조작하는 데 사용된다. 주로 데이터베이스에서
데이터 삽입, 삭제, 업데이트를 할 때 사용된다.
예로 SELECT, INSERT, UPDATE, DELETE 등이 있다.
```

- **SELECT** : 하나 이상의 테이블에서 데이터를(row) 검색하는 데 사용
- **INSERT** : 테이블에 새 데이터(row)를 삽입하는 데 사용
- **UPDATE** : 테이블의 기존 데이터(row)를 수정하는 데 사용
- **DELETE** : 테이블에서 데이터를 삭제하는 데 사용
<br></br><br></br>
> **DDL과 DML의 차이는 DDL은 대상을 정의하는데 사용되고, DML은 대상을 조작하는 데 사용된다는 점이다.**
>
