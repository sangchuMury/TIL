# 에러코드
``` SQL 
-- Error Code: 1227. Access denied; you need (at least one of) the CREATE USER privilege(s) for this operation
-- 오류 코드: 1227. 액세스가 거부되었습니다. 이 작업에 대한 CREATE USER 권한이 필요합니다(최소 하나).
```

MySQL Connection을 생성하고 사용자 계정 생성 및 권한 부여를 하는 도중 위와 같은 Error 메세지를 마주했다.

## 권한 조회 코드
``` SQL 
show grant for 사용자;
```
``` SQL
-- result massage
'GRANT USAGE ON *.* TO `사용자`@`%`'
```
usage(삭제하면 로그인조차 안됨) rnjs

