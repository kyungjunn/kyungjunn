<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=F05650&height=300&section=header&text=Kyungjun%20Engine&fontSize=50&fontColor=FFFEC8" />
</div>

## 🎮 Hello, I'm Kyungjun Kim | 게임 클라이언트 엔지니어 김경준입니다

- 🕹️ **문제를 해결하고 기능을 완성해 가는 과정**에서 큰 성취감을 느끼는 개발자입니다.
- 🛠️ 객체지향 설계 원칙과 효율적인 데이터 구조를 게임 시스템에 녹여내는 데 관심이 많습니다.
- 🌐 클라이언트뿐 아니라 **서버-클라이언트 통신 구조**까지 직접 설계하며 범위를 넓혀가고 있습니다.

<br>

## ✨ Tech Stack

### 🎮 Game Engines & Languages

<div align="left">
  <img src="https://img.shields.io/badge/Unreal%20Engine%205.7-0E1128?style=for-the-badge&logo=unrealengine&logoColor=white" />
  <img src="https://img.shields.io/badge/Unity%206-FFFFFF?style=for-the-badge&logo=unity&logoColor=black" />
  <img src="https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white" />
  <img src="https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=csharp&logoColor=white" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" />
</div>

### 🌐 Network & Database

<div align="left">
  <img src="https://img.shields.io/badge/TCP%2FIP-005571?style=for-the-badge&logo=cisco&logoColor=white" />
  <img src="https://img.shields.io/badge/Photon%20PUN2-004488?style=for-the-badge&logo=photon&logoColor=white" />
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" />
  <img src="https://img.shields.io/badge/FlatBuffers-40C4FF?style=for-the-badge&logo=googlecloud&logoColor=white" />
</div>

### 🛠️ Tools & Collaboration

<div align="left">
  <img src="https://img.shields.io/badge/git-F05033.svg?style=for-the-badge&logo=git&logoColor=white" />
  <img src="https://img.shields.io/badge/github-181717.svg?style=for-the-badge&logo=github&logoColor=white" />
  <img src="https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=notion&logoColor=white" />
  <img src="https://img.shields.io/badge/SDL2-1F1F1F?style=for-the-badge&logo=sdl&logoColor=white" />
</div>

<br>

## 🚀 Projects

### 1. League of Legends 모작 프로젝트

> **UE5 클라이언트 + 자체 제작 C++ 인증 서버로 구성한 MOBA 프로젝트**
> `Unreal Engine 5.7` `C++` `TCP/IP` `MySQL` · 2026.04 ~ 2026.07

- **인증 서버:** TCP 기반 C++ 인증 서버 구축 및 `OnlineSubsystem` 연동 게임 서버 구조 설계
- **상점 시스템:** `DataTable` 기반 Data-Driven 아이템 데이터 관리
- **인벤토리 시스템:** 아이템 타입별 추가/삭제 로직 구현
- **스킬 시스템:** `DataAsset` 기반 스킬 정보 관리
- **전투 시스템:** Listen 서버 방식의 RPC 클라이언트 동기화 처리
- **미니언 AI:** Behavior Tree 기반 `정찰 → 추적 → 공격` 상태 구조

  [📂 Client](https://github.com/kyungjunn/MyLeagueOfLegends) · [📂 Server](https://github.com/kyungjunn/MyLOLServer) · [📝 Notion](https://app.notion.com/p/39e261fc4ea680c0aaadc9b489029cd5?source=copy_link) · [▶️ YouTube](https://youtu.be/46AnZYh7nmU)

<br>

### 2. UE5 계정 / 로비 시스템 프로젝트

> **JWT 인증 웹 서버와 UE5 클라이언트를 연동한 계정·세션 파이프라인**
> `Unreal Engine 5.7` `C++` `Python` `MySQL` · 2026.07

- **계정 시스템:** 회원가입 · 로그인 · 내 정보 조회 · 회원탈퇴(소프트 삭제), JWT 기반 인증
- **로그인/회원가입 UI:** UMG 위젯 + `GameInstanceSubsystem` 연동 및 화면 전환 처리
- **로비 / 세션 시스템:** 방 생성 · 방 목록 조회 · 방 참가(최대 4인), 방 안 플레이어 닉네임 실시간 동기화(RPC/Replication)
- **협업 포인트:** 서버-클라이언트 API 명세를 문서로 먼저 정의하고, 클라이언트 구현 시 그대로 참조하는 계약 기반 개발

  [📂 Server](https://github.com/kyungjunn/UE5_WebServer) · [📂 Client](https://github.com/kyungjunn/UE5_Client) · [📝 Notion](https://app.notion.com/p/UE5-39f261fc4ea680568db3e7578e403d3d?source=copy_link)

<br>

### 3. 서버 클라이언트 동기화 프로젝트

> **엔진 없이 Winsock2로 직접 구현한 실시간 멀티플레이 네트워크**
> `C++` `Winsock2(TCP)` `SDL2` `MySQL` `FlatBuffers` · 2026.04 ~ 2026.05

- **네트워크 아키텍처:** `select` 모델 기반 동기식 멀티플렉싱 서버 구조 설계
- **클라이언트 설계:** 멀티스레드 구조 + Windows Event 객체 신호 기반 동기화
- **핵심 기능:** 실시간 접속/해제 처리, 사용자 세션 관리, 패킷 직렬화 좌표 연동, SDL2 하드웨어 렌더링

  [📂 Repository](https://github.com/kyungjunn/CPP_Study/tree/main/L20260521_MultiPlayer) · [📝 Notion](https://app.notion.com/p/39f261fc4ea68048a89ce94f939957a4?source=copy_link)

<br>

### 4. Pain and Gain : 3D 로그라이크 증강 디펜스

> **적 처치와 증강 선택을 중심으로 성장하는 3D 로그라이크 증강 디펜스 게임**
> `Unity 6` `C#` `ScriptableObject` `Netcode for GameObjects`

- **캐릭터 전투 시스템:** 인터페이스 기반 근접·원거리 공격 분리 및 캐릭터별 전투 구조 모듈화
- **공용 스킬 시스템:** 데이터 기반 스킬 설계, 공용 발사체 및 입력 처리 구조 구현
- **증강 시스템:** ScriptableObject 기반 데이터 관리, 스탯·스킬 증강 분리, 등급별 선택 및 누적 관리
- **퀘스트 시스템:** 랜덤 퀘스트 진행·판정 및 실패 시 보유 증강 감소 페널티 구현
- **멀티플레이 확장:** Netcode for GameObjects(NGO) 적용 진행 중

  [📂 Repository](https://github.com/kyungjunn/Pain_and_Gain) · [📝 Notion](https://app.notion.com/p/3D-3e4261fc4ea6800cb779dfc10781379a?source=copy_link)

<br>

### 5. 로블록스 3D 훅 스윙 액션 게임

> **로비에서 장비를 고르고 개인 코스를 날아, 상승 타이밍에 손을 놓는 성장형 스윙 러너**
> `Roblox` `Luau` `DataStore` `RopeConstraint`

- **훅 스윙 시스템:** 훅 후보 가중 선택, RopeConstraint 기반 진자 운동, 카메라 조준축 조향, 상승 30° 릴리즈 판정
- **판정 파이프라인:** 클라이언트 예측 연출과 서버 관측 재평가 분리, PERFECT–MISS 등급 판정, 콤보 집계 및 훅당 1회 득점 처리
- **성장 루프:** 누적점수 기반 존 해금, 코인 상점, 최고점 랭킹 및 삼축 자원 분리

  [📂 Repository](https://github.com/kyungjunn/HookMan_Roblox) · [📝 Notion](https://app.notion.com/p/3D-408261fc4ea680df9221ff073fbc7944?source=copy_link)

<br>

### 6. Infinity Tank : 멀티플레이 탱크 디펜스

> **Photon PUN2 기반 협동 웨이브 디펜스 게임**
> `Unity 6` `C#` `Photon(PUN2)` · 2025.04 ~ 2025.06

- **멀티플레이 시스템:** Photon 기반 로비(닉네임 설정, 방 생성/입장), RPC를 활용한 체력·포격·사망 실시간 동기화
- **적 AI:** NavMesh 기반 순찰-추적형 탱크 AI
- **보스 기믹:** Wave 10 보스 드래곤 등장 — 시네마틱/BGM 전환, 브레스 패턴 및 SafeZone 기믹
- **랭킹 시스템:** Wave · 플레이 시간 기준 정렬 및 게임 종료 후 순위 출력
- **Troubleshooting:** 마스터 클라이언트 중심의 연산 구조로 설계하여 클라이언트 간 AI 및 데미지 상태 불일치 문제 해결

  [📝 Notion](https://app.notion.com/p/39f261fc4ea680dd88efd7ec5c9d9013?source=copy_link)

<br>

## 📜 Certificates & Education

- 🏆 **정보처리산업기사** (2025.09)
- 🎓 **동양미래대학교** 컴퓨터소프트웨어공학과 학사 (2026.03 ~ 2027.02 졸업 예정)
- 🎓 **명지전문대학교** 컴퓨터공학과 전문학사 (2021.03 ~ 2026.02 졸업)
- 🎖️ **몬스테라텍 K-Digital Training 부트캠프 수료** (2026.02 ~ 2026.08)
  - [NS 홈쇼핑] 디지털 콘텐츠 버추얼 프로덕션 전문가 과정(엔지니어)
  - 언리얼 엔진(UE5) 활용 및 멀티플레이 네트워킹 학습

<br>

## 📫 Contact

<div align="left">
  <a href="mailto:1124kyungjun@gmail.com">
    <img src="https://img.shields.io/badge/1124kyungjun@gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white"/>
  </a>
  <a href="https://github.com/kyungjunn">
    <img src="https://img.shields.io/badge/Github-181717?style=for-the-badge&logo=github&logoColor=white" />
  </a>
</div>

---

<div align="right">
  Last Updated: 2026.10.30
</div>
