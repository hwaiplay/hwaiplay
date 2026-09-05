<div align="center">
  <img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:0F172A,50:0369A1,100:22C55E&height=220&section=header&text=Seunghyeon%20Kang&fontSize=48&fontColor=FFFFFF&animation=fadeIn&fontAlignY=36&desc=Backend%20Developer%20%C2%B7%20Enterprise%20Integration&descAlignY=58&descSize=18" alt="Seunghyun Kang header" />
</div>

<div align="center">

### 안녕하세요, 백엔드 개발자 강승현입니다 👋

기업의 복잡한 업무 흐름을 **안정적인 API와 재사용 가능한 공통 모듈**로 연결합니다.  
ERP, 예약, 결제, 알림, 대외계 시스템을 하나의 서비스 흐름으로 통합해 온 경험이 있습니다.

</div>

## 💼 Experience

<table>
  <tr>
    <td width="23%" valign="top">
      <strong>삼구아이앤씨</strong><br />
      <sub>e-SEP ERP 유지보수 및 개발</sub>
    </td>
    <td valign="top">
      <ul>
        <li>자체 ERP인 <strong>e-SEP</strong>의 기능 개선과 운영 유지보수를 담당했습니다.</li>
        <li>기존 그룹웨어의 주요 기능을 e-SEP에 통합하여 분산된 업무 흐름을 하나의 ERP에서 처리할 수 있도록 개발했습니다.</li>
        <li><strong>eGovFrame · MSSQL · WebSquare SP4/SP5</strong> 환경에서 화면과 업무 로직을 구현했습니다.</li>
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
        <li>서비스 간 데이터 연계를 위한 <strong>RESTful API</strong>를 개발했습니다.</li>
        <li><strong>Spring Boot · JavaScript · Oracle</strong> 기반으로 백엔드 API와 연계 기능을 구현했습니다.</li>
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
        <li><strong>Opera ORS RESTful API</strong>를 연동하여 오프라인 객실 예약 시스템을 홈페이지 예약 흐름에 통합했습니다.</li>
        <li><strong>비즈톡</strong>을 이용해 온라인 객실, 오프라인 객실 예약의 알림톡 발송을 하나의 공통 기능으로 구축했습니다.</li>
        <li>객실 예약 결제 정보를 전송하는 <strong>EAI 전표 공통 메서드</strong>를 개발하여 채널별 중복 로직을 줄였습니다.</li>
      </ul>
    </td>
  </tr>
</table>

## 🎯 What I Do Best

| System Integration | Reusable Backend | Business Understanding |
|:---:|:---:|:---:|
| ERP·예약·결제·알림 시스템 연동 | 공통 API와 재사용 모듈 개발 | 복잡한 업무 흐름을 안정적인 로직으로 구현 |

## 🚀 Featured Project

### [Sadari](https://github.com/hwaiplay/sadari) — 독서 기록·목표·소셜 PWA

도서 검색, 독후감과 독서 목표, 소셜 활동, 독서 모임, 알림과 웹 푸시를 하나의 서비스 흐름으로 구현했습니다. 사용자용 React PWA와 Spring Boot API, 별도 관리자 서비스를 설계하며 기능 구현을 넘어 데이터 정합성, 보안, 운영 가능성을 함께 다루었습니다.

**이 프로젝트에서 확장한 역량**

- **인증 수명주기 설계** - Kakao OAuth 2.0, JWT HttpOnly Cookie, CSRF Token, Redis 세션 메타데이터와 로그아웃 블랙리스트를 결합했습니다.
- **데이터 정합성과 장애 경계** - 도서·독후감 등록을 하나의 트랜잭션으로 처리하고, FCM은 커밋 후 발송하며 관리자 상태 변경은 DB Outbox로 Redis 반영 실패를 재시도하도록 구성했습니다.
- **조회 최적화와 검증** - 마이페이지 SQL 왕복을 최대 19회에서 2회로 줄였습니다. 비로컬 MySQL 개발 DB의 단일 연결 JDBC 100회 측정에서 중앙값이 215.241ms에서 26.436ms로 감소했으며, 이는 API·운영 환경 지표와 구분합니다.
- **문제에 맞는 알고리즘과 보안** - Aho-Corasick 금칙어 탐지, CIELAB 표지 색상 매칭, 이미지 시그니처·해상도·EXIF 검증과 재인코딩을 적용했습니다.
- **운영과 배포 자동화** - 공통코드·알림 템플릿·메뉴·스케줄러를 관리자 서비스와 공유 테이블로 운영하고, Docker·GHCR·GitHub Actions·EC2 Docker Compose 배포 흐름을 구성했습니다.

[Repository](https://github.com/hwaiplay/sadari) · [Wiki](https://github.com/hwaiplay/sadari/wiki) · [성능 개선 근거](https://github.com/hwaiplay/sadari/blob/master/docs/performance/my-page-reading-summary-optimization.md) · [Admin](https://github.com/vellahw/sadari-admin)

## 🛠 Tech Stack

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

## 📊 GitHub

<div align="center">
  <img width="100%" src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=hwaiplay&theme=github_dark" alt="hwaiplay GitHub profile details" />
</div>

## 📫 Contact

<p>
  <a href="mailto:vs81702738@gmail.com"><img src="https://img.shields.io/badge/Gmail-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Gmail" /></a>
  <a href="https://www.instagram.com/kangsh0126/"><img src="https://img.shields.io/badge/Instagram-E4405F?style=flat-square&logo=instagram&logoColor=white" alt="Instagram" /></a>
</p>

<div align="center">
  <sub>기능을 만드는 데서 멈추지 않고, 여러 시스템이 안정적으로 함께 동작하도록 연결합니다.</sub>
  <img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:22C55E,50:0369A1,100:0F172A&height=110&section=footer" alt="footer" />
</div>
