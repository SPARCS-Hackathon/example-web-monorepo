# [ TEAM Z ] Example Web Monorepo
 
이 Repository는 "예시 해커톤 제출 프로젝트" 의 웹 프론트, 백엔드를 담당하는 Monorepo 입니다. 

다음과 같은 기능이 포함되어 있습니다. 

- 해커톤을 전국 대학(원)생들에게 홍보
- 참가자 문의하기

## 프로젝트에서 사용한 기술 

본 Repository는 `pacakge.json` 에 있는 오픈소스 패키지를 사용하였습니다.

또 다음 Code Snippet 이 포함되어 있습니다.

- [JS Modal 만들기](https://www.w3schools.com/howto/howto_css_modals.asp)
- [JS 쿠키 설정 방법](https://yj-code.tistory.com/7)

[참고] 위 오픈소스 및 Code Snippet 첨부는 부정행위 방지를 위한 것이며, 개발에 있어 유의미한 소스만 첨부해 주셔도 괜찮습니다.


## Dev Server 실행 방법

1. 본 Repository를 로컬 환경에 Clone 받습니다.
2. `yarn install` 로 필요한 패키지를 설치 합니다.
3. `.env.example` 을 `.env` 로 복사한 다음, 아래 [환경 변수 및 시크릿] 규약에 따라 작성합니다.
4. MySQL 8.0 Docker 컨테이너를 실행합니다.
5. `prisma migrate` 를 이용하여 DB 스키마를 설정해 줍니다.
6. `yarn dev` 로 HMR 서버를 실행하여 개발환경을 실행합니다.


[참고] Dev Server 실행 방법은 부정행위 방지를 위한 사후 발표 자료와의 대조를 위한 것이며, 임원진이 검증 가능한 정도로 작성해 주셔도 괜찮습니다.

## Production 배포 방법

1. Ubuntu 20.04 환경의 서버를 준비합니다.
2. 본 Repository를 로컬 환경에 Clone 받습니다.
3. `docker compose -f=.docker/production-compose.yml up -d` 을 이용하여 실행해 줍니다.

[참고] Dev Server 실행 방법은 부정행위 방지를 위한 사후 발표 자료와의 대조를 위한 것이며, 임원진이 검증 가능한 정도로 작성해 주셔도 괜찮습니다. 또한, 이후 해커톤 홍보를 위한 데모의 목적으로 활용될 수 있습니다.


## 환경 변수 및 시크릿
1. 필요한 환경 변수는 `.env.example` 에 명시되어 있습니다.
    1. JWT_SECRET 은 18-24자리 이내 a-Z,0-9 로 설정되어야 합니다.
2. `config/settings.js` 파일에서 `AWS_CLIENT_ID` 를 설정합니다.

## 기타
이 프로젝트 만드는데 커피 100잔 마셨어요

해커톤 너무 멋져요 짱짱
