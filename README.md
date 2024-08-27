# 💫 OneulEun

|                                [이하얀](https://github.com/hayannn)                                |
|:-----------------------------------------------------------------------------------------------:
|                                      dlgkdis801@naver.com                                       |
![이하얀](https://github.com/user-attachments/assets/18c1ba87-523d-45a2-a4a1-1e76056b2d23)  |

<br>

## 📣 개요
- Online Judge 사이트 제작 Side Project
- 핵심 기능 및 초기 기능 : 온라인 코딩 및 채점 시스템 개발(Beakjoon, Programmers와 같은 시스템)

---

<br>

## 📣 주요 기능
| 기능                | 설명                                                            |
|---------------------|-----------------------------------------------------------------|
| 강의 등록 및 수강 기능    | 코딩과 관련된 기초 강의를 수강할 수 있는 기능을 제공합니다. |
| 퀴즈 및 과제 제출 기능      | 강의를 수강하며 퀴즈를 풀이하고, 과제가 있는 경우 과제를 제출할 수 있습니다. |
| 강의별 토론 게시판      | 강의별로 다양한 의견을 나눌 수 있는 토론 게시판을 운영하여, 강의자와 사용자만이 아닌 사용자 사이에서도 학습할 수 있도록 합니다.              |
| 랭킹 조회 | 온라인 저지 사이트의 랭킹처럼, 현재 사이트 내 본인의 순위를 확인할 수 있습니다.     |
| 실시간 방송 및 실시간 댓글 기능     | 녹화 강의뿐만 아니라, 실시간 스트리밍 서비스를 제공하여 특강을 진행하고, 실시간으로 소통할 수 있도록 댓글 기능도 제공합니다. |
| 관리자 | 강의 및 사용자 관련 전반적인 사이트 관리 권한을 통해 사이트가 원활히 운영될 수 있도록 하는 관리자 기능을 제공합니다. |

<br>

## 📣 최종 개발 목표
- 백엔드 중심 온라인 저지 플랫폼 API 개발 완료
- 배포 및 성능 테스트 진행
- 동영상 스트리밍 + 실시간 스트리밍 서비스 정상 작동

<br>

## 📣 아키텍쳐 및 ERD
<img width="950" alt="스크린샷 2024-08-26 오후 1 56 20" src="https://github.com/user-attachments/assets/40ceeec4-7ba4-4da4-8697-b3b0b6c4d6fb">
<img width="794" alt="스크린샷 2024-08-26 오후 2 32 22" src="https://github.com/user-attachments/assets/d2858f63-10f6-4916-aa00-9c3c1be12906">

<br>

## 📣 API 명세
- [oneulEun API 명세서](https://hayanlee.notion.site/oneulEun-API-624a1f93d0a6488a881af9788b3e134a?pvs=4)
  - 관리자 API의 경우, 추후 추가 예정
    <img width="1154" alt="스크린샷 2024-08-27 오후 3 30 30" src="https://github.com/user-attachments/assets/a072b4df-06ed-4d3c-b73f-d97bd2d96854">
    <img width="1110" alt="스크린샷 2024-08-27 오후 3 29 41" src="https://github.com/user-attachments/assets/0723ddca-de1c-4b59-a05a-ca5ff38d126d">
    <img width="1100" alt="스크린샷 2024-08-27 오후 3 29 58" src="https://github.com/user-attachments/assets/3b39d694-6f31-446e-a88b-20bcd3d33e48">
    <img width="1182" alt="스크린샷 2024-08-27 오후 3 30 09" src="https://github.com/user-attachments/assets/ac431e5b-6ba3-4281-af66-0ccc4b66d394">
    <img width="1142" alt="스크린샷 2024-08-27 오후 3 30 20" src="https://github.com/user-attachments/assets/f4f0d411-d5aa-4824-bb6b-c16313f62dbf">
    <img width="1117" alt="스크린샷 2024-08-27 오후 3 30 47" src="https://github.com/user-attachments/assets/d7ce7720-284e-48d9-91bc-8f6cdfe52c52">
  
<br>

## 📣 기술스택

- Backend
1. SpringBoot
2. MySQL
3. Redis
4. Kafka
5. Nginx-Rtmp

### 배포 가능 시 사용
1. AWS EC2
2. AWS RDS
3. Docker
4. Nginx
5. GitHub Actions

<br>

- Frontend
1. Bootstrap
2. thymeleaf

<br>

## 📣 라이브러리

- Backend
1. lombok
2. MySQL Connector
3. spring data jpa
4. spring web
5. spring kafka
6. oauth2 client
7. spring security
8. spring boot test
9. spring security test
10. spring session redis
11. swagger
12. jjwt

<br>

- Frontend
1. spring thymeleaf

<br>

---

## 📣 프로젝트 구조
```
└── 🗂 main
    ├── 🗂 java
    │   └── 🗂 com
    │       └── 🗂 devkkongha
    │           └── 🗂 oneulEun
    │               ├── 📑 oneulEunApplication.java
    │               ├── 🗂 common
    │               │   └── 🗂 exception 
    │               │       └── 📑 CustomException.java
    │               ├── 🗂 config
    │               │   ├── 📑 CorsConfig.java
    │               │   ├── 📑 JwtFilter.java
    │               │   ├── 📑 LoginSuccessHandler.java
    │               │   ├── 📑 RedisConfig.java
    │               │   ├── 📑 SecurityConfig.java
    │               │   └── 📑 SwaggerConfig.java
    |               |
    |               |
    │               ├── 🗂 controller
    │               │   ├── 📑 OauthController.java
    │               │   ├── 📑 UserController.java
    │               │   ├── 📑 LiveStreamingController.java
    │               │   ├── 📑 CodePostController.java
    │               │   ├── 📑 CodeGradingService.java
    │               │   ├── 📑 RankingController.java
    │               │   ├── 📑 CourseQuizController.java
    │               │   ├── 📑 CoursePostController.java
    │               │   ├── 📑 CourseController.java
    │               │   └── ... 추가 및 수정 예정
    │               │   
    │               │   
    │               ├── 🗂 dto
    │               │   ├── 📑 LoginResultDTO.java
    │               │   ├── 📑 SocialUserProfileDTO.java
    │               │   ├── 📑 LiveStreamingDTO.java
    │               │   ├── 📑 CodePostDTO.java
    │               │   ├── 📑 CodeGradingDTO.java
    │               │   ├── 📑 RankingDTO.java
    │               │   ├── 📑 CourseQuizDTO.java
    │               │   ├── 📑 CoursePostDTO.java
    │               │   ├── 📑 CourseDTO.java
    │               │   └── ... 추가 및 수정 예정
    │               │
    │               │
    │               ├── 🗂 exception
    │               │   ├── 📑 CustomException.java
    │               │   ├── 📑 ErrorCode.java
    │               │   ├── 📑 ErrorResponse.java
    │               │   ├── 📑 NotFoundException.java
    │               │   └── 📑 ResponseConstant.java
    │               │
    |               |
    │               ├── 🗂 model
    │               │   ├── 📑 LiveStreaming.java
    │               │   ├── 📑 CodePost.java
    │               │   ├── 📑 CodeGrading.java
    │               │   ├── 📑 Ranking.java
    │               │   ├── 📑 CourseQuiz.java
    │               │   ├── 📑 CoursePost.java
    │               │   ├── 📑 Course.java
    │               │   └── 📑 User.java
    │               │
    |               |
    │               ├── 🗂 repository
    │               │   ├── 📑 LiveStreamingRepository.java
    │               │   ├── 📑 CodePostRepository.java
    │               │   ├── 📑 CodeGradingRepository.java
    │               │   ├── 📑 RankingRepository.java
    │               │   ├── 📑 CourseQuizRepository.java
    │               │   ├── 📑 CoursePostRepository.java
    │               │   ├── 📑 CourseRepository.java
    │               │   ├── 📑 OAuthUserRepository.java
    │               │   └── 📑 UserRepository.java
    │               │
    |               |
    │               ├── 🗂 service
    │               │   ├── 🗂 kakao 
    │               │   │   ├── 📑 ExchangeKakaoAccessToken.java
    │               │   │   ├── 📑 ExchangeKakaoAccessTokenImpl.java
    │               │   │   ├── 📑 FetchKakaoUserProfile.java
    │               │   │   ├── 📑 FetchKakaoUserProfileImpl.java
    │               │   │   └── 📑 KakaoLoginService.java
    │               │   ├── 📑 LiveStreamingService.java
    │               │   ├── 📑 CodePostService.java
    │               │   ├── 📑 CodeGradingService.java
    │               │   ├── 📑 RankingService.java
    │               │   ├── 📑 CourseQuizService.java
    │               │   ├── 📑 CoursePostService.java
    │               │   ├── 📑 CourseService.java
    │               └── └── 📑 UserService.java
    │               
    └── 🗂 resources
        └── 📑 application.yml      
```
---

<br>


## 📣 commit message convention
- feat: 새로운 기능 추가
- fix: 버그 수정
- docs: 문서
- style: 포맷팅, 누락된 세미콜론 등
- refactor: 코드 리팩토링
- test: 테스트 관련
- chore: 기타 수정
- build: 빌드 시스템 또는 외부 의존성에 영향을 주는 변경
- remove: 파일을 삭제