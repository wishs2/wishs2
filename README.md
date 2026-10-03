# 안녕하세요, 백엔드 개발자 민소원입니다.

Java와 Spring Boot를 기반으로 백엔드 개발을 공부하고 있습니다.

단순히 기능을 구현하는 데 그치지 않고,
**데이터의 무결성, 외부 API 처리 구조, 테스트와 성능을 함께 고민하는 개발자**를 지향합니다.

프로젝트에서 OCR 데이터 처리 구조 개선, DB 제약조건을 활용한 데이터 무결성 설계,
Redis와 Scheduler를 활용한 LLM 호출 구조 개선 등을 경험했습니다.

---

## 🛠 Tech Stack

### Backend
- Java 17
- Spring Boot
- Spring Security
- MyBatis
- REST API

### Database & Data
- MySQL
- Redis

### Testing
- JUnit
- Mockito
- Postman
- Swagger
- Apache JMeter

### Collaboration
- Git / GitHub
- GitHub Branch / Pull Request / Code Review
- Notion
- WBS

---

## 📌 Main Project

### 언니어때 — 위치 및 영수증 기반 뷰티 업체 리뷰 플랫폼

영수증 인증을 통해 실제 이용자의 리뷰 작성을 지원하고,
위치 기반으로 주변 뷰티 업체를 탐색할 수 있는 웹 서비스입니다.

**Role — Backend Developer / Team Lead**

주요 담당 기능

- NCP OCR API 기반 영수증 인증 및 데이터 추출
- 리뷰 작성 · 조회 · 수정 · 삭제
- 영수증 및 리뷰 중복 방지를 위한 DB 무결성 설계
- LLM 기반 리뷰 요약 기능
- Redis Set + Scheduler 기반 리뷰 요약 처리 구조 개선
- JUnit / Mockito 기반 비즈니스 로직 테스트
- JMeter 기반 리뷰 조회 API 부하 테스트
- WBS 작성 및 프로젝트 일정 관리
- GitHub Branch / Pull Request / Code Review 기반 협업

### Problem Solving

**01. OCR 데이터 처리 구조 개선**  
Regex 중심 추출 방식에서  
`Token → Line → Field Extractor` 구조로 개선하여  
OCR 데이터의 형식 차이에 대응할 수 있도록 구조화했습니다.

**02. 데이터 무결성 설계**  
애플리케이션 로직에만 의존하지 않고  
복합 UNIQUE Constraint를 적용하여  
영수증 및 리뷰 중복 저장을 DB 단계에서 방지했습니다.

**03. LLM 리뷰 요약 호출 구조 개선**  
리뷰 작성마다 LLM을 호출하던 구조에서  
`Event → Redis Set → Scheduler` 구조로 변경하여  
동일 업체의 변경 요청을 하나의 처리 대상으로 통합했습니다.

**04. 리뷰 조회 API 부하 테스트**  
Apache JMeter로 30,000건의 요청을 수행하여  
이미지 처리 구조 변경 전후의 응답 시간과 처리량을 비교했습니다.

> 상세한 설계 과정과 문제 해결 내용은 Portfolio에서 확인할 수 있습니다.

👉 [Project Repository](https://github.com/wishs2/SSGINC_unnie.git)
<br>
👉 [Portfolio PDF](https://github.com/wishs2/SSGINC_unnie/blob/0fcd099186abb13648f10e1fb32d4b513312c361/backend-portfolio.pdf)

---

## 🎓 Education

**신세계아이앤씨**  
JAVA 기반 백엔드 개발자 양성과정  
2024.09 - 2025.03

**신안산대학교**  
호텔경영과  
2021.03 - 2023.02

---

## 📜 Certifications

- 정보처리산업기사
- SQLD

---

## 📫 Contact

- GitHub: https://github.com/wishs2
- Email: sowork02@gmail.com
