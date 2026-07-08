# 🕵️‍♂️ 은밀하게 위대하게 (Secretly & Greatly)

> **“가장 완벽한 보호색, 모니터 뒤에서 당당하게 확인하는 나만의 시크릿 포트폴리오”**
> 개발자를 위한 VS Code 위장형 주식 모니터링 & 실시간 커뮤니티 서비스

<br />

## 💻 프로젝트 개요 (What is Secretly & Greatly?)
개발자가 온종일 띄워두는 **VS Code 화면으로 완벽하게 위장**하여 주변 시선 신경 쓰지 않고 당당하게 주식 시세와 포트폴리오를 관리할 수 있는 웹 서비스입니다. 일반적인 주식 앱의 노출 위험을 원천 차단하고, 오직 개발자들만을 위한 UI/UX와 실시간 소통 공간을 제공합니다.

* **Target**: 주변 시선이 신경 쓰이는 프론트엔드·백엔드·데이터 엔지니어 및 DevOps, 코드 화면을 선호하는 직장인 투자자
* **Key Point**: 차트 중심의 일반 주식 앱이나 셀 기반의 엑셀 주식창과 달리, 개발자에게 가장 익숙한 **파일 트리, 시스템 로그, Git, 에이전트 패널** 형태로 네이티브하게 구현되었습니다.

<br />

## 🌟 핵심 기능 (Core Features)

1. **VS Code 위장 UI (IDE Disguise)**
   * VS Code 다크 테마 완벽 재현.
   * Explorer 파일 트리 구조(`stocks.sheet`, `positions.json`)로 관심 종목 및 자산 관리.
   * 시세 데이터는 스프레드시트 그리드와 캔들 차트로 본문에 출력.

2. **패닉 핫키 (Boss Key)**
   * 위급 상황 시 **`Esc` 키를 빠르게 2회 입력**하면 단 0.1초 만에 모든 자산 화면을 가리고 **소스 제어(Git) 화면으로 전환**.
   * 가짜 커밋 변경 목록과 Git Graph를 띄워 평범하게 형상 관리를 하고 있는 것처럼 완벽 위장.

3. **시세 & 터미널 시스템 로그 알림**
   * 한국투자증권(KIS) API 연동을 통한 국내(KRX)·해외(NASDAQ/NYSE) 준실시간 시세 제공 (30초 폴링).
   * 실시간 주가 변동성 알림을 하단 TERMINAL 탭에 `[INFO]`, `[WARN]`, `[ALERT]` 형태의 시스템 로그 포맷으로 위장 출력.

4. **실시간 채팅 (Real-time Chat)**
   * VS Code 우측의 AI 에이전트 패널(Claude Code 패널)로 위장한 실시간 전체 채팅 지원.
   * 도배 방지 쿨타임, 금칙어 필터, 신고 누적 자동 블라인드 등 모더레이션 기능 포함.

5. **물타기 시뮬레이터**
   * 내 포트폴리오에서 평단가와 수량을 자동 주입받아 매수 시뮬레이션 진행.
   * 계산 결과를 `[Optimizer Info]` 최적화 로그 형식으로 위장하여 출력.

6. **뉴스 수집 & AI 요약 브리핑**
   * 매시간 정각 백그라운드에서 뉴스를 수집하여, **Google Gemini API**를 통해 한 줄 요약 및 5종 태그 분류 처리.
   * 개발 환경의 코드 주석 스타일(`// 뉴스 내용`)로 News Feed 탭에 자연스럽게 노출.

<br />

## 🛠 기술 스택 (Tech Stack)

### Frontend
- **Framework & Library**: Next.js, React, TanStack Query, Zustand, Axios, socket.io-client
- **Styling & Architecture**: Tailwind CSS, FSD (Feature-Sliced Design) 구조
- **Development Tools**: MSW, Orval (Mocking & Code Generation)

### Backend & Infrastructure
- **Runtime & Framework**: Node.js, NestJS, Express
- **Database & ORM**: PostgreSQL, Prisma ORM, Supabase (News 전용)
- **Caching & Real-time**: Redis (ioredis), Socket.IO
- **DevOps**: AWS EC2, Docker, Nginx, GitHub Actions (CI/CD)
- **Automation / AI**: Cheerio (Scraping), node-cron, Google Gemini API
