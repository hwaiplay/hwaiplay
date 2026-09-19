<div align="center">
  <img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0F172A,50:0369A1,100:22C55E&height=220&section=header&text=Seunghyeon%20Kang&fontSize=48&fontColor=FFFFFF&animation=fadeIn&fontAlignY=36&desc=Backend%20Developer%20%C2%B7%20Enterprise%20Integration&descAlignY=58&descSize=18" alt="Seunghyun Kang header" />
</div>

<div align="center">

### 백엔드 개발자 강승현입니다

</div>

## Experience

<table>
  <tr>
    <td width="23%" valign="top">
      <strong>삼구아이앤씨</strong><br />
      <sub>e-SEP ERP 유지보수 및 개발</sub>
    </td>
    <td valign="top">
      <ul>
        <li>자체 ERP <strong>e-SEP</strong> 개발 및 유지보수</li>
        <li>그룹웨어 주요 기능을 e-SEP에 통합</li>
        <li><strong>eGovFrame · MSSQL · WebSquare SP4/SP5</strong>로 화면과 업무 로직 개발</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td width="23%" valign="top">
      <strong>남양유업</strong><br />
      <sub>RESTful API 개발</sub>
    </td>
    <td valign="top">
      <ul>
        <li>서비스 간 데이터 연계용 <strong>RESTful API</strong> 개발</li>
        <li><strong>Spring Boot · JavaScript · Oracle</strong> 사용</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td width="23%" valign="top">
      <strong>신라호텔</strong><br />
      <sub>홈페이지 리뉴얼</sub>
    </td>
    <td valign="top">
      <ul>
        <li><strong>Opera ORS RESTful API</strong>로 오프라인 객실 예약을 홈페이지에 연동</li>
        <li><strong>비즈톡</strong>으로 온·오프라인 객실 예약 알림톡 발송 기능 공통화</li>
        <li>객실 예약 결제 전송용 <strong>EAI 전표 공통 메서드</strong>로 채널별 중복 로직 축소</li>
      </ul>
    </td>
  </tr>
</table>

## Focus

| System Integration | Reusable Backend | Business Understanding |
|:---:|:---:|:---:|
| ERP·예약·결제·알림 시스템 연동 | 공통 API와 재사용 모듈 개발 | 업무 흐름에 맞는 안정적인 로직 구현 |

## Project

### [Sadari](https://sadaribooks.com) · 독서 커뮤니티

도서 검색, 독후감, 독서 목표·모임, 소셜 활동, 알림·웹 푸시를 제공합니다.
React PWA, Spring Boot API와 별도 관리자 서비스를 개발했습니다.

- **인증**: Kakao OAuth 2.0, JWT HttpOnly Cookie, CSRF Token. Redis로 세션 메타데이터와 로그아웃 블랙리스트 관리.
- **데이터 정합성**: 도서·독후감 등록을 하나의 트랜잭션으로 처리. FCM은 커밋 후 발송하고, 관리자 상태의 Redis 반영 실패는 DB Outbox로 재시도.
- **조회 성능**: 마이페이지 SQL 왕복 최대 19회 → 2회. 중앙값 215.241ms → 26.436ms.¹
- **알고리즘·보안**: Aho-Corasick 금칙어 탐지, CIELAB 표지 색상 매칭. 이미지 시그니처·해상도·EXIF 검증 및 재인코딩.
- **운영·배포**: 관리자 서비스와 공유 테이블로 공통코드·알림 템플릿·메뉴·스케줄러 관리. Docker·GHCR·GitHub Actions·EC2 Docker Compose 배포 구성.

<sub>¹ 비로컬 MySQL 개발 DB, 단일 연결 JDBC 100회 측정. API·운영 환경 지표는 아닙니다.</sub>

[Repository](https://github.com/hwaiplay/sadari) · [Wiki](https://github.com/hwaiplay/sadari/wiki) · [성능 개선 근거](https://github.com/hwaiplay/sadari/blob/master/docs/performance/my-page-reading-summary-optimization.md) · [Admin](https://github.com/vellahw/sadari-admin)

## Tech Stack

### Backend & Security

<p>
  <img src="https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white" alt="Java" />
  <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white" alt="Spring Boot" />
  <img src="https://img.shields.io/badge/Spring%20Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white" alt="Spring Security" />
  <img src="https://img.shields.io/badge/MyBatis-DC382D?style=flat-square" alt="MyBatis" />
  <img src="https://img.shields.io/badge/eGovFrame-1F4E79?style=flat-square" alt="eGovFrame" />
  <img src="https://img.shields.io/badge/RESTful%20API-0284C7?style=flat-square&logo=fastapi&logoColor=white" alt="RESTful API" />
</p>

### Data & Infrastructure

<p>
  <img src="https://img.shields.io/badge/RDBMS-4479A1?style=flat-square" alt="RDBMS" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker" />
  <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions" />
  <img src="https://img.shields.io/badge/AWS%20EC2-FF9900?style=flat-square&logo=amazonec2&logoColor=white" alt="AWS EC2" />
  <img src="https://img.shields.io/badge/Firebase%20Cloud%20Messaging-DD2C00?style=flat-square&logo=firebase&logoColor=white" alt="Firebase Cloud Messaging" />
</p>

### Frontend

<p>
  <img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=20232A" alt="React" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white" alt="Vite" />
  <img src="https://img.shields.io/badge/Thymeleaf-005F0F?style=flat-square&logo=thymeleaf&logoColor=white" alt="Thymeleaf" />
  <img src="https://img.shields.io/badge/TanStack%20Query-FF4154?style=flat-square&logo=reactquery&logoColor=white" alt="TanStack Query" />
  <img src="https://img.shields.io/badge/Zustand-443E38?style=flat-square" alt="Zustand" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=000000" alt="JavaScript" />
  <img src="https://img.shields.io/badge/WebSquare-3B82F6?style=flat-square" alt="WebSquare" />
</p>

## GitHub

<div align="center">
  <img width="100%" src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=hwaiplay&theme=github_dark" alt="hwaiplay GitHub profile details" />
</div>

## Contact

<p>
  <a href="mailto:vs81702738@gmail.com"><img src="https://img.shields.io/badge/Gmail-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Gmail" /></a>
  <a href="https://www.instagram.com/kangsh0126/"><img src="https://img.shields.io/badge/Instagram-E4405F?style=flat-square&logo=instagram&logoColor=white" alt="Instagram" /></a>
</p>

<div align="center">
  <img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:22C55E,50:0369A1,100:0F172A&height=110&section=footer" alt="footer" />
</div>
