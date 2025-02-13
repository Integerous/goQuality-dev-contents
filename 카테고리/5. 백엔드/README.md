# 5. 백엔드

> 📌 목차
>- [시스템 설계/구현](#시스템-설계구현)
>   - [아키텍처](#아키텍처)
>   - [기능/서비스 개발](#기능서비스-개발)
>   - [성능 최적화](#성능-최적화)
>   - [장애/디버깅](#장애디버깅)
>   - [로깅/알람](#로깅알람)
>   - [캐시](#캐시)
>   - [메시지 큐](#메시지-큐)
>   - [마이그레이션](#마이그레이션)
>   - [보안](#보안)
>   - [API](#API)
>   - [웹소켓](#웹소켓)


## 시스템 설계/구현
- [CloudWatch 메트릭 그래프 스냅샷 만들기](https://brunch.co.kr/@alden/53)
- [카카오 개발자가 본 ‘요즘 클라우드 흐름’ 세 가지](http://m.zdnet.co.kr/news_view.asp?article_id=20190721085551&re=zdk#imadnews)
- [아파치 로드밸런싱으로 여러 WAS 운영하기](https://taetaetae.github.io/2019/08/04/apache-load-balancing/)
- [리디북스 서비스 장애 복구 후기](https://www.ridicorp.com/blog/2016/09/02/idc-outage/)
- [가장 쉽게 AWS VPC 개념잡기](https://medium.com/harrythegreat/aws-%EA%B0%80%EC%9E%A5%EC%89%BD%EA%B2%8C-vpc-%EA%B0%9C%EB%85%90%EC%9E%A1%EA%B8%B0-71eef95a7098)
- [AWS로 토이프로젝트 운영삽질기](https://medium.com/harrythegreat/aws%EB%A1%9C-%ED%86%A0%EC%9D%B4%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8-%EC%9A%B4%EC%98%81%ED%95%98%EA%B8%B0-5a77f7e13521)
- [쿠키런 1년, 서버개발 분투기 [슬라이드]](https://www.slideshare.net/mobile/serialxnet/1-35304689)
- [콘퍼런스 참가 신청 기능 개발기](https://d2.naver.com/helloworld/5048491)
- [스파게티 조인을 피하고 경계안에서 캐시 구현하기](https://www.popit.kr/%ec%8a%a4%ed%8c%8c%ea%b2%8c%ed%8b%b0-%ec%a1%b0%ec%9d%b8%ec%9d%84-%ed%94%bc%ed%95%98%ea%b3%a0-%ea%b2%bd%ea%b3%84%ec%95%88%ec%97%90%ec%84%9c-%ec%ba%90%ec%8b%9c-%ea%b5%ac%ed%98%84%ed%95%98%ea%b8%b0/)
- [웹서버 부하테스트 실전 노하우 [슬라이드]](https://www.slideshare.net/IMQAGroup/ss-183469952)
- [Cloudflare 도입 후기](https://www.ridicorp.com/blog/2019/10/14/cloudflare-dos-and-donts/)
- [엔터프라이즈 어플리케이션을 위한 효과적인 프로세싱 전략 [영상]](https://youtu.be/IafgrRB2quY)
- [Serverless와 기술도입, Backend Application의 미래](https://medium.com/vingle-tech-blog/serverless%EC%99%80-%EA%B8%B0%EC%88%A0%EB%8F%84%EC%9E%85-backend-application%EC%9D%98-%EB%AF%B8%EB%9E%98-8f114a8b00d5)
- [타다 (TADA) 서비스의 데이터 웨어하우스 : 태초부터 현재까지 [슬라이드]](https://speakerdeck.com/vcnc/tada-tada-seobiseuyi-deiteo-weeohauseu-taecobuteo-hyeonjaeggaji)
- [푸시 데몬 메모리 누수 디버깅하기](https://mingrammer.com/debug-memory-leak-with-node-heapdump/)
- [멀티클라우드를 이용한 로그 분석 플랫폼 개발하기](https://link.medium.com/yuZDbtqcp1)
- [웹서비스 백엔드 애플리케이션 아키텍처](https://brunch.co.kr/@springboot/228#comment)
- [EC2, Fargate 약정 할인 AWS Savings Plans 발표](https://www.44bits.io/ko/post/aws-introducing-savings-plans)
- [글로벌 서비스를 위한 멀티 리전 프록시 도입기](https://medium.com/benx-tech-blog/%EA%B8%80%EB%A1%9C%EB%B2%8C-%EC%84%9C%EB%B9%84%EC%8A%A4%EB%A5%BC-%EC%9C%84%ED%95%9C-%EB%A9%80%ED%8B%B0-%EB%A6%AC%EC%A0%84-%ED%94%84%EB%A1%9D%EC%8B%9C-%EB%8F%84%EC%9E%85%EA%B8%B0-87eda1bd8d55#gaerae.com)
- [AWS S3 정적호스팅 SPA에 동적 메타태그 적용하기](https://urbanbase.github.io/dev/2019/11/25/AWS-S3-SPA.html)
- [라즈베리파이4로 토이프로젝트용 서버 만들기 - 1편](https://ryan-han.com/post/server/raspberry_server_1/)
- [스케일아웃없이 순간 급증하는 주문 처리하기 [영상]](https://tv.naver.com/v/11212897)
- [ActiveMQ의 Virtual Destinations를 활용한 메세지 로드밸런싱](https://ryan-han.com/post/server/activemq_virtual_destinations/)
- [Multi CDN 트래픽 모니터링을 위한 클러스터 구축기](https://engineering.linecorp.com/ko/blog/build-cluster-for-multi-cdn-traffic-monitoring/)
- [데이터 기반으로 지속적인 CI/CD 개선 환경 만들기](https://engineering.linecorp.com/ko/blog/build-a-continuous-cicd-environment-based-on-data/)
- [주니어 개발자의 CI/CD 도입기](http://bit.ly/34JfNJ2)
- [10가지 소프트웨어 아키텍처 패턴 요약 [번역]](https://mingrammer.com/translation-10-common-software-architectural-patterns-in-a-nutshell/)
- [ELK 셋팅부터 알람까지️](http://woowabros.github.io/experience/2020/01/16/set-elk-with-alarm.html)
- [하둡 총정리](http://www.incodom.kr/hadoop_%EC%B4%9D%EC%A0%95%EB%A6%AC)
- [우아한 모노리스 [영상]](https://youtube.com/watch?feature=youtu.be&v=SrQeIz3gXZg)
- [캐치딜 백엔드 개발이야기 : 좌충우돌 서버운영 이야기](https://kbs4674.tistory.com/114)
- [awesome-scalability](https://github.com/binhnguyennus/awesome-scalability)
- [Scaling to 100k Users [영문]](https://alexpareto.com/scalability/systems/2020/02/03/scaling-100k.html)
- [Scaling to 100k Users [번역]](https://brunch.co.kr/@jowlee/102)
- [AWS 람다(AWS Lambda)란?](https://www.44bits.io/ko/keyword/aws-lambda)
- [온디맨드 이미지 리사이징 (Ondemand Image Resizing) 원리 및 예제](https://roka88.dev/m/102)
- [LINE LIVE 채팅 기능의 기반이 되는 아키텍처](https://engineering.linecorp.com/ko/blog/the-architecture-behind-chatting-on-line-live/)
- [멀티 쓰레드 프로그램 설계를 위한 8가지 규칙 [번역]](https://brunch.co.kr/@chris-song/95)
- [LINE LIVE 채팅 기능의 기반이 되는 아키텍처](https://engineering.linecorp.com/ko/blog/the-architecture-behind-chatting-on-line-live/)
- [배달의민족 최전방 시스템! '가게노출 시스템'을 소개합니다.](https://woowabros.github.io/experience/2020/02/19/introduce-shop-display.html)
- [안심번호 마이크로서비스 개발하기](https://medium.com/daangn/%EC%95%88%EC%8B%AC%EB%B2%88%ED%98%B8-%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%EC%84%9C%EB%B9%84%EC%8A%A4-%EA%B0%9C%EB%B0%9C%ED%95%98%EA%B8%B0-fb1a8817b059)
- [LINE 메시징 서버가 새해 트래픽을 대비하는 과정](https://engineering.linecorp.com/ko/blog/how-line-messaging-servers-prepare-for-new-year-traffic/)
- [딥러닝 모델 Serving 간단 구축기](https://tech.socarcorp.kr/data/2020/03/10/ml-model-serving.html)
- [로드밸런서의 종류와 동작방식](https://deveric.tistory.com/m/91)
- [Spring Batch 관리 도구로서의 Jenkins](https://jojoldu.tistory.com/489)
- [AWS 비용을 줄이는 10가지 방법 [영문]](https://aws.amazon.com/ko/blogs/compute/10-things-you-can-do-today-to-reduce-aws-costs/)
- [서머타임과 배치작업](https://meetup.toast.com/posts/232)
- [CDN과 로드밸런서를 활용한 부하 분산](https://blog.naver.com/n_cloudplatform/221918957658)
- [쿠팡 추천 시스템 2년간의 변천사 (상품추천에서 실시간 개인화로) [영상]](https://tv.naver.com/v/11212875)
- [서버리스는 서버가 없는걸까? 8분 개념 설명! [영상]](https://www.youtube.com/watch?v=ufLmReluPww)
- [LINE 트랜스코딩 서버 아키텍처 개선기 – 1](https://engineering.linecorp.com/ko/blog/line-transcoding-server-architecture-improvement-1/)
- [주니어 개발자의 클린 아키텍처 맛보기](http://woowabros.github.io/tools/2019/10/02/clean-architecture-experience.html)
- [서버리스를 활용한 분산 처리 [슬라이드]](https://www.slideshare.net/MinJunKim5/masocon-2019-serverless-kimminjun)
- [MySQL을 이용한 분산락으로 여러 서버에 걸친 동시성 관리](https://woowabros.github.io/experience/2019/05/30/mysql-user-level-lock.html)


### 아키텍처
- [Introducing Domain-Oriented Microservice Architecture](https://eng.uber.com/microservice-architecture/)
- [네이버 메인 페이지의 트래픽 처리](https://d2.naver.com/helloworld/6070967)
- [실시간 댓글 개발기(part.1) - DAU 60만 Alex 댓글의 실시간 댓글을 위한 이벤트 기반 아키텍처](https://tech.kakao.com/2020/06/08/websocket-part1/)
- [신규 포인트 시스템 전환기 #1 – 개발 단계](https://techblog.woowahan.com/2587/)
- [대규모 분산 스토리지(Kage)의 발전과정](http://tech.kakao.com/2017/01/12/kage/)
- [단방향 사용자 인터페이스 아키텍쳐](https://pilgwon.github.io/blog/2018/12/12/Unidirectional-User-Interface-Architectures.html)
- [타다 시스템 아키텍처](https://blog-tech.tadatada.com/2019-01-28-tada-system-architecture)

- [마이크로서비스 아키텍처 (MSA) [번역]](https://medium.com/wematch/마이크로서비스-아키텍처-msa-359b7973ba79)
- [마이크로서비스 아키텍쳐. 그것이 뭣이 중헌디?](http://guruble.com/마이크로서비스microservice-아키텍처-그것이-뭣이-중헌디/)
- [MSA (Microservice Architecture) 마이크로서비스 아키텍처 회고](https://bebong.tistory.com/m/entry/MSA-Microservice-Architecture-%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%EC%84%9C%EB%B9%84%EC%8A%A4-%EC%95%84%ED%82%A4%ED%85%8D%EC%B2%98-%ED%9A%8C%EA%B3%A0)
- [마이크로서비스 아키텍처(MSA) - 기본적인 개념과 우버적용 사례 [번역]](https://brunch.co.kr/@yesjun/2)
- [마틴 파울러가 설명하는 마이크로서비스 [번역]](http://channy.creation.net/articles/microservices-by-james_lewes-martin_fowler)
- ["마이크로서비스는 답이 아니었다" 세그먼트가 모놀리틱으로 돌아온 이유](http://www.ciokorea.com/news/39258)
- [마이크로서비스, 어디까지 해봤니? [영상]](https://youtu.be/F7EnW8dfetU)
- [잘 키운 모노리스 하나 열 마이크로서비스 안 부럽다 [슬라이드]](https://www.slideshare.net/arawnkr/ss-195979955)
- [쿠팡의 MSA 적용기, 행복을 찾기위한 우리의 여정](https://medium.com/coupang-tech/%ED%96%89%EB%B3%B5%EC%9D%84-%EC%B0%BE%EA%B8%B0-%EC%9C%84%ED%95%9C-%EC%9A%B0%EB%A6%AC%EC%9D%98-%EC%97%AC%EC%A0%95-94678fe9eb61)
- [MSA, K8S를 이용한 대륙의 서비스 개발 사례 [슬라이드]](https://www.slideshare.net/mobile/babokim/open-infradays-2019msak8s)
- [MSA에서 동시에 여러 API 호출로 응답 시간 줄이기](https://www.popit.kr/msa%EC%97%90%EC%84%9C-%EB%8F%99%EC%8B%9C%EC%97%90-%EC%97%AC%EB%9F%AC-api-%ED%98%B8%EC%B6%9C%EB%A1%9C-%EC%9D%91%EB%8B%B5-%EC%8B%9C%EA%B0%84-%EC%A4%84%EC%9D%B4%EA%B8%B0)
- [마이크로 서비스 관련 글 총정리](https://www.popit.kr/%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C-%EC%84%9C%EB%B9%84%EC%8A%A4-%EA%B4%80%EB%A0%A8-%EA%B8%80-%EC%B4%9D%EC%A0%95%EB%A6%AC/)
- [WATCHA PLAY 서비스 MSA 적용하기](https://medium.com/watcha/watcha-play-%EC%84%9C%EB%B9%84%EC%8A%A4-msa-%EC%A0%81%EC%9A%A9%ED%95%98%EA%B8%B0-31e06fe039a0)
- [휴면 계정 처리 – 배치에서 온라인 시스템으로](http://www.chidoo.me/index.php/2019/09/14/from-batch-to-online-processing-in-msa/)
- [Mastering Chaos - A Netflix Guide to Microservices [영상]](https://www.youtube.com/watch?v=CZ3wIuvmHeM)
- [마이크로 서비스 아키텍쳐와 컨테이너 환경](http://bit.ly/2J7YgRz)
- [Go RESTful API(gRPC Client) + Python gRPC server](https://medium.com/cloudbric-tech-leaders/go-restful-api-grpc-client-python-grpc-server-15e95386e90d)


### 기능/서비스 개발
- [배민라이더스 배달 경로와 거리 계산 개발 과정](https://techblog.woowahan.com/2608/)
- [AWS Lambda@Edge에서 실시간 이미지 리사이즈 & WebP 형식으로 변환](https://medium.com/daangn/lambda-edge로-구현하는-on-the-fly-이미지-리사이징-f4e5052d49f3)
- [Go와 함께하는 전화망 서비스 구축 1편](https://d2.naver.com/helloworld/5827706)
- [Go와 함께하는 전화망 서비스 구축 2편](https://d2.naver.com/helloworld/0814313)
- [리모트 컨피그 서버 구축기](https://techblog.woowahan.com/2611/)
- [선착순 이벤트 서버 생존기! 47만 RPM에서 살아남다?!](https://www.youtube.com/watch?v=MTSn93rNPPE)


### 성능 최적화


### 장애/디버깅
- [빌링 시스템 장애, 이러지 말란 Maria~](https://techblog.woowahan.com/2517/)
- [서버에 걸리는 부하, 추측하지 말고 계측하자](https://injae-kim.github.io/dev/2020/07/09/how-to-check-single-server-load-average.html)

### 로깅/알람


### 캐시
- [레디스 사망일기](https://perfectacle.github.io/2019/05/29/redis-monitoring/)
- [캐시 성능 향상기 (Improving Cache Speed at Scale)](https://meetup.toast.com/posts/251)
- [레디스와 분산 락(1/2) - 레디스를 활용한 분산 락과 안전하고 빠른 락의 구현](https://hyperconnect.github.io/2019/11/15/redis-distributed-lock-1.html)
- [개발자를 위한 레디스 튜토리얼](https://meetup.toast.com/posts/224)
- [Jedis 보다 Lettuce를 쓰자](https://jojoldu.tistory.com/418)
- [Redis in Action [영문]](https://redislabs.com/community/ebook)
- [IDC에서 AWS로 Redis 데이터 이전하기](https://mingrammer.com/redis-migration/)
- [우아한테크세미나 - 우아한 레디스 [영상]](https://youtu.be/mPB2CZiAkKM)  
- [우아한 Redis 세미나 후기](https://ict-nroo.tistory.com/133)
- [우아한 Redis 발표자료 [슬라이드]](https://www.slideshare.net/charsyam2/redis-196314086)
- [Redis 6.0 – ThreadedIO를 알아보자.](https://charsyam.wordpress.com/2020/05/05/입-개발-redis-6-0-threadedio를-알아보자/)


### 메시지 큐
- [이벤트 기반 분산 시스템을 향한 여정](https://www.slideshare.net/arawnkr/ss-94475606)
- [아파치 카프카 레퍼런스 한글 번역](https://godekdls.github.io/Apache%20Kafka/design/)
- [Kafka 운영자가 말하는 처음 접하는 Kafka](https://www.popit.kr/kafka-%EC%9A%B4%EC%98%81%EC%9E%90%EA%B0%80-%EB%A7%90%ED%95%98%EB%8A%94-%EC%B2%98%EC%9D%8C-%EC%A0%91%ED%95%98%EB%8A%94-kafka/)
- [LINE에서 Kafka를 사용하는 방법](https://engineering.linecorp.com/ko/blog/how-to-use-kafka-in-line-1/)


### 마이그레이션


### 보안

### API
- [REST API에서 Put 과 Post 의 차이](http://bit.ly/2CFGzIM)
- [REST API의 이해와 설계  1편 - 개념 소개](http://bit.ly/2QX4lD8)
- [Restful API를 설계하기 위한 디자인 팁](https://spoqa.github.io/2013/06/11/more-restful-interface.html)
- [REST API 제대로 알고 사용하기](https://meetup.toast.com/posts/92)
- [그런 REST API로 괜찮은가 [영상]](https://www.youtube.com/watch?v=RP_f5dMoHFc)
- [REST API 튜토리얼 [영문]](https://restapitutorial.com/)
- [REST API 설명 [영상]](https://www.youtube.com/watch?v=LooL6_chvN4)
- [REST FULL 한 웹서비스 > Stateless와 HATEOAS 개념](http://anster.tistory.com/163)
- [REST의 representation이란 무엇인가](https://blog.npcode.com/2017/04/03/rest의-representation이란-무엇인가/)
- [REST API가 뭔가요? [영상]](https://youtu.be/iOueE9AXDQQ)
- [RESTful API 설계 가이드](https://sanghaklee.tistory.com/57)
- [조금 더 괜찮은 Rest Template 1부 - Retryable](https://taetaetae.github.io/2020/03/22/better-rest-template-1-retryable/)
- [프론트엔드와 백엔드가 소통하는 엔드포인트, RESTful API](https://evan-moon.github.io/2020/04/07/about-restful-api/)
- [프로듀스48과 함께하는 GraphQL(그래프큐엘)](http://bit.ly/2qkVjVh)
- [GraphQL과 RESTful API](http://bit.ly/2Q3ZK1H)
- [GraphQL 개념잡기](https://tech.kakao.com/2019/08/01/graphql-basic/)
- [코딩 없이 10분 만에 REST API/Graphql 서버 개발하기](https://medium.com/@khwsc1/js%EB%A1%9C-10%EB%B6%84%EB%A7%8C%EC%97%90-rest-api-graphql-%EC%84%9C%EB%B2%84-%EA%B0%9C%EB%B0%9C%ED%95%98%EA%B8%B0-d28148dbdef2)
- [GraphQl을 오해하다](https://medium.com/@FourwingsY/graphql%EC%9D%84-%EC%98%A4%ED%95%B4%ED%95%98%EB%8B%A4-3216f404134)


### 웹소켓
- [실시간 댓글 개발기(part.2) -  험난했지만 유익했던 웹소켓 스트레스 테스트 및 안정화 작업](https://tech.kakao.com/posts/391)