# 우리 주변 인사이트, 우주인

<img width="862" height="368" alt="image" src="https://github.com/user-attachments/assets/d591c630-ec18-4cc0-985c-ba0b5060eda6" />

<br>

## 핵심 기능


![KakaoTalk_Photo_2024-11-15-18-16-08 002](https://github.com/user-attachments/assets/4ebf209c-293d-4a56-8450-07c99ebca4ac)
![KakaoTalk_Photo_2024-11-15-18-16-08 003](https://github.com/user-attachments/assets/d5562835-c4e8-47fa-9e66-127185a19fb9)
![KakaoTalk_Photo_2024-11-15-18-16-08 004](https://github.com/user-attachments/assets/2f87c050-8be4-4c55-8c94-044679c431e5)
![KakaoTalk_Photo_2024-11-15-18-16-08 005](https://github.com/user-attachments/assets/0650aa88-358f-4725-a5e2-df86bfe6bf8b)
![KakaoTalk_Photo_2024-11-15-18-16-14](https://github.com/user-attachments/assets/6a8c374e-c45e-4930-beed-92260ad55d6f)
![KakaoTalk_Photo_2024-11-15-18-16-17](https://github.com/user-attachments/assets/977c8961-2640-4ca4-85ae-db2cb4826d01)
![KakaoTalk_Photo_2024-11-15-18-16-20](https://github.com/user-attachments/assets/323d36f2-e3de-46bf-a1aa-d21cd2cbc3fe)


<br>

## 구현 기능 설명

### 🔙 BE

#### **1. Spring Security**

- Spring Security를 활용해 애플리케이션의 인증 및 권한 관리를 구현하였습니다. JWT 기반 토큰 인증과 커스터마이징된 필터를 통해 보안을 강화하였습니다.


#### 2. OAuth(구글 로그인, 카카오 로그인)

- 구글과 카카오의 OAuth 인증을 통합하여 사용자가 간편하게 소셜 로그인 기능을 이용할 수 있도록 구현하였습니다.
- 각 플랫폼의 사용자 정보를 통해 회원가입 없이 서비  스를 바로 이용할 수 있게 했습니다.


#### 3. 카카오페이 결제

- 카카오페이 API를 활용하여 사용자가 앱 내에서도 편하게 결제를 할 수 있도록 구현했습니다.


#### 4. AOP 로깅

- AOP(Aspect-Oriented Programming)를 활용하여 공통적으로 필요한 로깅 기능을 분리하였습니다.
- 주요 서비스의 요청, 응답 및 실행 시간을 효과적으로 추적하고, 디버깅 및 모니터링에 활용하였습니다.


#### 5. N+1 문제 해결 (페치 조인 및 배치 사이즈)

- JPA의 N+1 문제를 방지하기 위해 페치 조인을 적극 활용하고, @BatchSize를 적용하여 필요한 데이터만 효율적으로 조회할 수 있도록 최적화하였습니다.


#### 6. 썸네일 이미지 생성

- 사용자가 업로드한 이미지를 기반으로 썸네일 이미지를 자동으로 생성하여, 서버 저장 공간과 전송 속도를 최적화하였습니다. 이를 통해 사용자 경험을 개선하였습니다.

#### 7. CI/CD (Docker, GitHub Actions)
   
- Docker와 GitHub Actions를 사용하여 CI/CD 파이프라인을 구축하였습니다.
- 코드 변경 사항이 자동으로 빌드, 테스트, 배포되는 환경을 구성하여 개발 및 배포의 효율성을 높였습니다.

#### 8. Certificate Manager, Route 53, Gabia를 이용한 https 도메인 구현

- Gabia를 이용해 도메인을 구입한 뒤, Certificate Manager로 https 인증서를 발급하고 Route 53으로 라우팅을 설정하여 https 도메인 접속을 구현하였습니다.

#### 9. RDS를 이용한 데이터베이스 구축

- AWS의 RDS를 이용하여 MySQL 데이터베이스 환경을 구축하고, 백엔드 서버가 돌아가는 EC2와 연동하였습니다.

<br>

## ERD 다이어그램

![KakaoTalk_Photo_2024-11-15-17-58-55](https://github.com/user-attachments/assets/246353a7-d8e9-49f6-970e-23a23729f7bd)

<br>

## 📖 API 명세서

https://www.notion.so/e8d71c13017844de97303da3c73d0840?v=8432c86ed8114eb1943ff861399fe6c1

<br>

## ⚒️ 기능 명세서

https://www.notion.so/67925a6cfccb412191c1e50e958e87f4

<br>

## 🚨 에러코드 정의서

https://www.notion.so/fba45247c95d4a129f60a8afddd1228f
