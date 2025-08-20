# Cake-Quake-back
<hr>
> AI 추천과 발주 기능을 갖춘 맞춤형 레터링 케이크 예약 플랫폼
> Spring Boot 기반 **Backend 레포지토리**

---

## 📌 프로젝트 개요
레터링 케이크 프로젝트는 구매자와 판매자가 소통하며 맞춤형 케이크를 주문·판매할 수 있도록 지원하는 서비스입니다.  
본 레포지토리는 **백엔드(Spring Boot)** 구현을 담당하며, API 설계 및 데이터베이스 관리, 비즈니스 로직을 제공합니다.

---

## 🛠️ 기술 스택
- **Language**: Java 17  
- **Framework**: Spring Boot 3.4.5, Spring Data JPA  
- **Database**: PostgreSQL  
- **Build Tool**: Gradle  
- **Infra**: AWS EC2, RDS, S3  
- **CI/CD**: GitHub Actions  

---


## 📖 주요 기능
- 🛒 **구매자**
  - 케이크 옵션 선택 및 주문 API
  - AI 추천
  - 알림 발송 (주문 상태, 승인, 배송 등)
  - 뱃지 & 포인트 시스템

- 🧑‍🍳 **판매자**
  - 상품 등록/수정/삭제 API
  - 옵션 타입 및 값 관리
  - 주문 내역 관리
  - 노쇼 방지용 온도 시스템

- 👨‍💻 **관리자**
  - 회원/상품 관리
  - 신고 접수 및 제재 처리

---

## ⚙️ 프로젝트 구조
```bash
📦 cake-quake-back
├─ src/main/java
│  └─ com.cakequake/cakequakeback
│     ├─ controller/      # REST API 컨트롤러
│     ├─ dto/             # 데이터 전송 객체
│     ├─ entities/        # 엔티티 클래스
│     ├─ repository/      # JPA 리포지토리
│     └─ service/         # 비즈니스 로직
├─ src/main/resources
│  ├─ fonts/              # 폰트 파일
│  ├─ prompts/            # AI 프롬프트 파일
│  └─ application.yml     # 환경 변수 설정
├─ env.                   # 환경 변수 관련 파일
└─ build.gradle
```

---

## 🐞 트러블슈팅

문제: 상품 옵션 조합 제한
→ 해결: 옵션 테이블을 조합형 구조로 리팩토링하여 유연하게 대응

문제: AWS S3 이미지 업로드 권한 오류
→ 해결: 버킷 정책 재설정

문제: AI 답변 오류
→ 해결: 프롬프트 수정 개선

---

## 👤 본인 역할

- 상품 관리 및 옵션 설정
- AI 추천 기능 구현
- 지도 기능 개발
- 뱃지 & 포인트 시스템 구현
- 알림 기능 (SSE 기반) 개발
- AWS EC2, RDS, S3를 활용한 배포

---

## 📅 개발 기간
2025.05.08 ~ 2025.07.11

