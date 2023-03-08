# ms-calendar-for-backend
1. 회원 기반
2. 팔로잉/팔로워 관계
3. 개인/공유 캘린더
4. 멤버 검색
5. 메이플스토리 큐브 확률 검증(개인 아이템별 분석 가능)
6. 데이터 자동 수집

# swagger
1. run springboot
2. http://localhost:8080/swagger-ui/index.html

# how to deploy

```
$ ssh 34.64.59.204
$ cd ms-calendar-for-backend
$ git pull origin master

## If the server instance is newly started (for dabatase server)
$ sudo docker-compose up -d 

$ ./gradlew clean build -x test
$ java -jar -Dspring.profiles.active=.{env} build/libs/hero-for-backend-0.0.1-SNAPSHOT.jar 

## background start 
## $ nohup java -jar -Dspring.profiles.active=.{env} build/libs/hero-for-backend-0.0.1-SNAPSHOT.jar &
```
