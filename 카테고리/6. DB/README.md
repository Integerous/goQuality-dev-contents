# 6. DB

> 📌 목차
> - [DB 일반](#DB-일반)
> - [SQL](#SQL)
> - [관계형DB](#관계형DB)
>   - [PostgreSQL](#PostgreSQL)
>   - [MySQL](#MySQL)
>   - [AWS/Azure/GCP](#AWS/Azure/GCP)
>   - [Supabase/Firebase](#Supabase/Firebase)
>   - [그 외](#그-외-관계형DB)
> - [NoSQL](#NoSQL)
>   - [MongoDB](#MongoDB)
>   - [Redis](#Redis)
>   - [AWS/Azure/GCP](#AWS/Azure/GCP)
>   - [그 외](#그-외-NoSQL)
> - [성능 최적화](#성능최적화)
> - [그 외](#그-외)

## DB 일반
- [데이터모델링의 기초 정리](http://bit.ly/2Pmdd4C)
- [엘라스틱서치 인덱스와 샤드 분할](https://danawalab.github.io/elastic/2020/07/21/Elasticsearch-Index-Shard-How.html)
- [JDBC로 실행되는 SQL에 자동으로 프로젝트 정보 주석 남기기](http://bit.ly/2Rz7lql)
- [RDB부터 검색엔진까지··· 내게 꼭 맞는 DB 고르기](http://bit.ly/2q1l24E)
- [CockroachDB 안녕?](http://bit.ly/2yXOWe6)
- [DBMS는 어떻게 트랜잭션을 관리할까?](https://d2.naver.com/helloworld/407507)
- [Commons DBCP 이해하기](https://d2.naver.com/helloworld/5102792)
- [한 눈에 살펴보는 PostgreSQL](https://d2.naver.com/helloworld/227936)
- [데이터 구조와 설계 -튜토리얼 [번역]](https://medium.com/@khwsc1/%EB%B2%88%EC%97%AD-%EB%8D%B0%EC%9D%B4%ED%84%B0-%EA%B5%AC%EC%A1%B0%EC%99%80-%EC%84%A4%EA%B3%84-%ED%8A%9C%ED%86%A0%EB%A6%AC%EC%96%BC-b25792a0aa86)
- [DB도 형상관리를 해보자!](https://meetup.toast.com/posts/173)
- [데이터베이스 개념정리](https://brunch.co.kr/@toughrogrammer/17)
- [SQL vs NoSQL [영상]](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)
- [Apache ShardingSphere를 이용한 DB Sharding](https://blog.naver.com/PostView.nhn?blogId=asei&logNo=221511101848&proxyReferer=http%3A%2F%2Fm.facebook.com)
- [중국의 어떤 서버 개발자의 DB설계](https://blog.naver.com/imays/221461537682)
- [우아한 형제들 메인 데이터베이스 IDC 탈출 성공기](https://woowabros.github.io/experience/2019/12/19/ruby_database.html)
- [Druid와 Bitmap Index](https://leeyh0216.github.io/2020-04-26/Apache_Druid_bitmap_index)
- [아직도 돈 주고 DB 쓰나요 for DBA [영상]](https://www.youtube.com/watch?feature=youtu.be&v=DXu3nbWa4AA&app=desktop)


## SQL
- [SQL joins visualizer](https://sql-joins.leopard.in.ua/)
- [PostgreSQL로 배우는 SQL 기초 [슬라이드]](https://www.slideshare.net/mobile/JiHoLee4/postgresql-sql-121859670?fbclid=IwAR35t9ZqcON_2EXBu-xUuVhbQTHNNbqYWeArGWUh-IKKctotkXoQoKQtkKY)


## 관계형DB

### PostgreSQL
- [Node.js 와 PostgreSQL로 RESTful API 만들기](https://blog.logrocket.com/setting-up-a-restful-api-with-node-js-and-postgresql-d96d6fc892d8)

### MySQL
- [MySQL Workbench의 VISUAL EXPLAIN으로 인덱스 동작 확인하기](https://engineering.linecorp.com/ko/blog/mysql-workbench-visual-explain-index/)
- [Mysql Explain](https://cheese10yun.github.io/mysql-explian/)
- [MySQL Ascending index vs Descending index](https://tech.kakao.com/2018/06/19/mysql-ascending-index-vs-descending-index/)
- [Mysql 인덱스 정리 및 팁](https://jojoldu.tistory.com/243)
- [JDBC를 사용한 MySQL SSL 연결](https://medium.com/p/1c5da86cc2c5)
- [MySQL Lock 상황 문제 해결](https://www.popit.kr/mysql-lock-%EC%83%81%ED%99%A9-%EB%AC%B8%EC%A0%9C-%ED%95%B4%EA%B2%B0/)
- [MySQL ‘a’ = ‘a ‘가 true 인가? (PostgreSQL과 비교)](http://woowabros.github.io/study/2018/02/26/mysql-char-comparison.html)


### AWS/Azure/GCP


### Supabase/Firebase


### 그 외 관계형DB


## NoSQL


### MongoDB
- [MongoDB Index 설계 전략](https://blog.ull.im/engineering/2019/04/05/mongodb-indexing-strategy.html)


### Redis


### AWS/Azure/GCP


### 그 외 NoSQL


## 성능 최적화
- [쿼리 최적화: 빠른 쿼리를 위한 7가지 체크리스트](https://medium.com/watcha/%EC%BF%BC%EB%A6%AC-%EC%B5%9C%EC%A0%81%ED%99%94-%EC%B2%AB%EA%B1%B8%EC%9D%8C-%EB%B3%B4%EB%8B%A4-%EB%B9%A0%EB%A5%B8-%EC%BF%BC%EB%A6%AC%EB%A5%BC-%EC%9C%84%ED%95%9C-7%EA%B0%80%EC%A7%80-%EC%B2%B4%ED%81%AC-%EB%A6%AC%EC%8A%A4%ED%8A%B8-bafec9d2c073)
- [Scaling to 100M: NoSQL보다 나은 MySQL [번역] [슬라이드]](https://docs.google.com/presentation/d/1OOxTLIgAWKpRD29RuG0ERn9iuPxIlcpQL0-iLcd3HS8/edit?fbclid=IwAR1aDGUZdCT3F6XP6GHby_cCIY0fEGst7SDB9MLtAPaf24YKVO6PGgT2iN8#slide=id.p2)
- [MySQL performance-schema-instruments 사용에 따른 성능 영향 실험](https://engineering.linecorp.com/ko/blog/mysql-research-performance-schema-instruments/)
- [200만 동접 게임을 위한 MySQL 샤딩 [영상]](https://youtube.com/watch?v=8Eb_n7JA1yA&feature=youtu.be)
- [MySQL 성능 죽이는 잘못된 쿼리 습관](http://gywn.net/2012/05/mysql-bad-sql-type/)
- [DB분산처리를 위한 sharding](https://woowabros.github.io/experience/2020/07/06/db-sharding.html)

## 그 외
