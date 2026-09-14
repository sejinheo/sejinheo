![header](https://capsule-render.vercel.app/api?type=waving&height=100&width=1000&color=0:4e73df,100:1a237e)

## 허세진 | Backend Engineer

<b>고른 이유와 남은 한계를 함께 기록하는 백엔드 개발자입니다.</b>
여러 대안을 재보고 그 조건에서 무엇이 필요하고 무엇이 필요 없는지 판단합니다.

<br>

## Project

### LM#

> 실시간 라이브 방송으로 상품을 판매하는 서비스
- 재고 100개 상품에 동시 주문이 몰려 초과 판매되던 문제 → 원자적 쿼리로 묶어 **0건** 달성
- 특가 코너 오픈 순간 주문이 밀려 방송 종료 후에 결과를 알 수 있던 문제 → 캐시가 1차로 거르고 DB가 최종 확정하는 구조로 전환, **초당 3,000건** 무지연 처리
- 결제가 PG 응답을 기다리는 동안 다른 주문, 재고 처리까지 멈추던 문제 → 외부 호출을 트랜잭션 밖으로 분리해 커넥션 점유 최소화


### 포켓픽
> 포켓몬 카드 중고거래 서비스
- 취소된 주문이 재판매 대기로 되살아나던 문제 → 발행 순번 게이팅으로 순서 역전 **3건 → 0건**
- 품절로 취소됐다는 안내를 받았는데 카드엔 결제가 찍히던 문제 → 짧은 락과 사후 보정(환불 API 호출)으로 이중 승인 위험 제거
- 인기 거래글 캐시가 한꺼번에 만료돼 DB 부하가 주문 기능까지 번지던 문제 → 캐시 만료 시점을 분산해 해결
  
<br>

## Skill

**Backend**
<p align="left">
  <img src="https://img.shields.io/badge/JAVA-007396?style=for-the-badge&logo=Java&logoColor=white"/>
  <img src="https://img.shields.io/badge/SPRINGBOOT-6DB33F?style=for-the-badge&logo=SpringBoot&logoColor=white"/>
  <img src="https://img.shields.io/badge/JPA-59666C?style=for-the-badge&logo=hibernate&logoColor=white"/>
  <img src="https://img.shields.io/badge/gRPC-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white"/>
  <img src="https://img.shields.io/badge/Resilience4j-6DB33F?style=for-the-badge"/>
</p>

**Data & Messaging**
<p align="left">
  <img src="https://img.shields.io/badge/MYSQL-4479A1?style=for-the-badge&logo=MySQL&logoColor=white"/>
  <img src="https://img.shields.io/badge/MONGODB-47A248?style=for-the-badge&logo=MongoDB&logoColor=white"/>
  <img src="https://img.shields.io/badge/REDIS-DC382D?style=for-the-badge&logo=Redis&logoColor=white"/>
  <img src="https://img.shields.io/badge/KAFKA-231F20?style=for-the-badge&logo=ApacheKafka&logoColor=white"/>
  <img src="https://img.shields.io/badge/Debezium-FCC624?style=for-the-badge"/>
</p>

**Infra & Observability**
<p align="left">
  <img src="https://img.shields.io/badge/DOCKER-2496ED?style=for-the-badge&logo=Docker&logoColor=white"/>
  <img src="https://img.shields.io/badge/GITHUB%20ACTIONS-2088FF?style=for-the-badge&logo=githubactions&logoColor=white"/>
  <img src="https://img.shields.io/badge/PROMETHEUS-E6522C?style=for-the-badge&logo=Prometheus&logoColor=white"/>
  <img src="https://img.shields.io/badge/GRAFANA-F46800?style=for-the-badge&logo=Grafana&logoColor=white"/>
  <img src="https://img.shields.io/badge/Alertmanager-E6522C?style=for-the-badge"/>
</p>

**Test & Performance**
<p align="left">
  <img src="https://img.shields.io/badge/k6-7D64FF?style=for-the-badge&logo=k6&logoColor=white"/>
  <img src="https://img.shields.io/badge/JUnit5-25A162?style=for-the-badge&logo=junit5&logoColor=white"/>
  <img src="https://img.shields.io/badge/Mockito-DD4B39?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/TestContainers-2496ED?style=for-the-badge"/>
</p>

**Collaboration**
<p align="left">
  <img src="https://img.shields.io/badge/JIRA-0052CC?style=for-the-badge&logo=jira&logoColor=white"/>
  <img src="https://img.shields.io/badge/CONFLUENCE-172B4D?style=for-the-badge&logo=confluence&logoColor=white"/>
  <img src="https://img.shields.io/badge/NOTION-000000?style=for-the-badge&logo=Notion&logoColor=white"/>
  <img src="https://img.shields.io/badge/SLACK-4A154B?style=for-the-badge&logo=slack&logoColor=white"/>
</p>

<br>

## Contact

<a href="mailto:heosejin222@gmail.com"><img src="https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=Gmail&logoColor=white"></a>
<a href="https://velog.io/@heosejin/posts"><img src="https://img.shields.io/badge/Velog-20C997?style=for-the-badge&logo=velog&logoColor=white"></a>
---

<br>

작은 결정도 이유와 트레이드오프를 기록해두고, 다음 프로젝트에서 다시 꺼내 봅니다.


<img src="https://capsule-render.vercel.app/api?type=waving&color=0:4e73df,100:1a237e&height=100&section=footer"/>
