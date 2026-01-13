# Eunjung's Github Profile


**안정적이고 지속 가능한 시스템 구조를 고민하는 경험을 쌓아온 백엔드 개발자입니다.**

[![Email](https://img.shields.io/badge/Email-Contact_Me-O?style=flat-square&logo=gmail&logoColor=white)](mailto:dlqnfdl2610@naver.com)

---

## 기술 스택

### Backend & Languages
![Java](https://img.shields.io/badge/Java_17-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot_3.x-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![JPA](https://img.shields.io/badge/Spring_Data_JPA-6DB33F?style=for-the-badge&logo=spring&logoColor=white)

### Infrastructure & Database
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![MariaDB](https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)

### Tools & Collaboration
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black)

---

## 주요 프로젝트

### 1. Code Crash Arena (실시간 1:1 알고리즘 대결 서비스)
**`Solo Project`** | **`2025.11 ~ 2025.12`** Docker 기반의 독립된 코드 실행 환경과 Redis를 활용한 실시간 매칭 시스템을 구축했습니다.

![CodeCrashArena_아키텍처](./images/CodeCreashArena.png)

* **Key Tech**: Java 17, Spring Boot, WebSocket, Redis, Docker
    * **Race Condition 해결**: DB 기반 매칭의 병목 현상을 해결하기 위해 Redis ZSET(Sorted Set)과 Atomic Operation으로 동시성 이슈 없는 논블로킹 매칭 큐 구현
    * **안전한 코드 실행**: 사용자 코드가 서버에 영향을 주지 않도록 **Docker Container** 격리 환경에서 컴파일 및 실행되도록 파이프라인 구축
    * **좀비 세션 관리**: 네트워크 불안정 시 세션 유실 문제를 방지하기 위해 **Redis Scope(Lobby/Game)** 분리 전략 적용 및 자동 기권 처리 로직 구현

<br>

### 2. 한컷여행 (여행 경로 추천 및 공유 서비스)
**`(3명) Team Leader`** | **`2025.07 ~ 2025.09`** 한국관광공사 Open API를 활용하여 맞춤형 여행 경로를 생성하고 공유하는 플랫폼입니다.

![사진_한컷여행_메인화면_이미지](./images/OneCutTrip.png)

* **Key Tech**: Spring Boot, JPA, MariaDB, AWS (EC2/RDS), Docker
* **My Contribution**:
    * **데이터 정규화**: API 별로 상이한 비정형 필드 구조를 분석하여 확장 가능한 통합 데이터 모델링 및 정규화 수행
    * **데이터 매칭 정확도 향상**: 관광지 식별 코드가 API마다 다른 문제를 해결하기 위해, 명칭 기반 1차 매칭 후 **위/경도 좌표 거리 알고리즘**을 적용한 검증 로직 구현
    * **인프라 구축**: AWS 환경에서 Docker 컨테이너 기반으로 배포 파이프라인 구축 및 HTTPS(Route53) 적용

<br>

### 3. 위드유 (AI 활용 주식 모의투자 플랫폼)
**`(4명) Team Leader`** | **`2025.03 ~ 2025.06`** 실시간 주식 시세 API와 AI 챗봇을 결합한 모의투자 서비스입니다.

![사진_위드유_화면](./images/WithYou.png)

* **Key Tech**: Spring Boot, Redis, GCP, Flutter
* **My Contribution**:
    * **조회 성능 최적화**: RDB(회원/거래내역)와 **Redis(실시간 시세)**로 데이터 저장소를 분리하는 **Read-Through/Write-Back** 전략 설계로 병목 현상 해소
    * **API 과부하 방지**: 증권사 API의 Rate Limit 제한(초당 20회 미만 등)을 준수하기 위해 `synchronized` 블록과 **요청 큐(Queue)**를 활용한 재요청 로직 구현
    * **AI 챗봇 파이프라인**: LLM이 JSON 포맷으로 의도(Intent)를 반환하도록 프롬프트 엔지니어링 수행, 내부 API와 연동하여 실시간 주가 정보를 답변하도록 구현

---

## GitHub Analytics

<div align="center">
  <a href="https://github.com/Urasica">
    <img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FUrasica&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false"/>
  </a>
  <br><br>

  <img src="https://github-readme-stats.vercel.app/api?username=Urasica&show_icons=true&theme=radical&bg_color=151515&title_color=E94560&text_color=ffffff&v=1" height="150" alt="stats" />
  
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Urasica&layout=compact&theme=radical&bg_color=151515&title_color=E94560&text_color=ffffff&v=1" height="150" alt="languages" />
</div>