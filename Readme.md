# nodejs Mysql
### msyql에서 테이블 생성 후 node와 연결하기

1. 테이블 생성
mysql 워크벤치에서 테이블 만들기

>db생성
create database juhyeok;
>테이블 생성
create table juhyeok.`id_table`(
	`idx` INT UNSIGNED NOT NULL AUTO_INCREMENT,
    `id` varchar(50),
    `pw` varchar(50),
    primary key(`idx`)
);


2. nodejs, express 설치
> npm init --yes
-> npm 초기화. package.json 파일 생성

> npm install express
-> express 설치. node_modules 폴더, package-lock.json 파일 생성

> 서버 코드 작성
-> app.js 파일을 만들고 express사이트 - 시작하기 - hello world에 따라가서 코드 복사
![mysql 서버용 코드](https://github.com/Juhyeok0603/express_mysql/blob/main/img/mysql%EC%84%9C%EB%B2%84%EC%9A%A9%20%EC%BD%94%EB%93%9C.png?raw=true)

> 터미널
-> 터미널에서 node app.js를 치면 localhost:3000에서 서버가 돌아감.


3. mysql 연동
> msyql 설치
-> 터미널창에 npm install mysql2

> 테스트 파일
-> mysql을 테스트할 파일 mysql.js를 만듦

> 연동 코드
-> express 사이트 - 안내서 - 데이터베이스 통합 을 들어가 MySQL에 대한 연동 코드를 찾는다.