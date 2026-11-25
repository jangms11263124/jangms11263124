<div align="center">

# 안녕하세요, 배운 걸 기록하며 성장하는 개발자 장민석입니다.

실시간으로 반응하는 서비스를 만듭니다. 문제를 덮지 않고, 구조부터 고칩니다.

<a href="https://blog.naver.com/jangms1126"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/btn-blog-dark.svg"><img src="assets/btn-blog-light.svg" height="36" alt="Blog"></picture></a>&nbsp;<a href="mailto:jangms1126@naver.com"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/btn-email-dark.svg"><img src="assets/btn-email-light.svg" height="36" alt="Email"></picture></a>&nbsp;<a href="https://github.com/jangms11263124/TIL"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/btn-til-dark.svg"><img src="assets/btn-til-light.svg" height="36" alt="TIL"></picture></a>

</div>

---

## About Me

- **만드는 것**: 실시간으로 반응하는 서비스 — 브라우저 오디오 엔진·화상(싸스케), 검표 즉시 바뀌는 입장 QR(TIMO)
- **경험**: Next.js·Vue 3 웹부터 Flutter 모바일 앱까지 모두 완주 — 프레임워크에 매이지 않습니다
- **습관**: 배운 것은 [TIL](https://github.com/jangms11263124/TIL)에 기록
- **대표 성과**: SSAFY 관통·공통 프로젝트 **연속 우수상** — FinEdu, 싸스케

---

## Tech Stack

**Frontend**

<img src="https://skillicons.dev/icons?i=html,css,js,ts,react,nextjs,vue,tailwind,threejs,flutter,dart" alt="HTML, CSS, JavaScript, TypeScript, React, Next.js, Vue, Tailwind CSS, three.js, Flutter, Dart" />

**Backend**

<img src="https://skillicons.dev/icons?i=py,django,sqlite" alt="Python, Django, SQLite" />

**AI**

`LLM API` `RAG 파이프라인` `STT` `프롬프트 설계`

**Tools & Collaboration**

<img src="https://skillicons.dev/icons?i=git,github,gitlab,figma,postman,vscode" alt="Git, GitHub, GitLab, Figma, Postman, VS Code" />

`Jira` `Google Stitch`

---

## Projects

### [TIMO — 블록체인 기반 공연 티켓 예매·양도 앱](https://github.com/jangms11263124/TIMO)

- **서비스**: 공연 티켓을 예매하고, 입장 QR로 검표하고, 못 가게 된 티켓은 양도 마켓에 올리고, 다녀온 공연은 소장품으로 남기는 모바일 티켓 앱
- **팀 / 기간**: SSAFY 특화 프로젝트 · 6인 팀 · 2026.08 ~ 2026.09
- **역할**: Frontend (Flutter)
- **한 일**:
  - 예매 흐름 — 네이버 CAPTCHA · 44px 고정 칸으로 만든 사다리꼴 좌석표 · 포인트 결제 · 발행 대기 화면
  - 입장 QR — 30초 만료 후 새로고침 방식, 조용한 푸시와 2초 확인으로 입장 완료 전환
  - 내 티켓 상태별 카드·메뉴 잠금 규칙, 양도 마켓 등록/취소, 알림함
  - 타이머 화면 위젯 테스트, 326개 파일 코드·주석 정리
- **배운 것**: 326개 파일을 정리할 때 테스트 860개가 안전망이 되는 걸 겪어서, 다음 프로젝트부터는 첫 기능부터 테스트를 같이 쓰고 있습니다
- **기술**: `Flutter` `Dart` `dio` `Hive` `Firebase Cloud Messaging`

### [싸스케 — 실시간 화상 노래방](https://github.com/jangms11263124/ssasukae)

- **서비스**: 화상으로 함께 부르고, 공격 카드로 방해하고, AI 가창 피드백을 받는 실시간 노래방
- **팀 / 기간**: SSAFY 공통 프로젝트 · 6인 팀 · 2026.07 ~ 2026.08
- **성과**: **우수상** 수상
- **역할**: Frontend · AI 파트 기획
- **한 일**:
  - Web Audio API 기반 **보컬 오디오 엔진** 설계·구현 — MR/마이크 채널 분리 병렬 라우팅으로 반주 키·목소리 이펙트 독립 제어
  - **RNNoise(WASM) 노이즈 억제** 검증·이식, SoundTouch AudioWorklet 실시간 템포·피치 시프트
  - 손 제스처로 음정·템포를 조절하는 **제스처 DSP 인터랙션**
  - 수성전 카드 연출 · 방 플로우 · AI 피드백 · 마이페이지 화면
  - AI 파트(STT + RAG 가창 피드백) 기획 · 결선 발표 자료 제작
- **배운 것**: MR 키 변경 시 목소리까지 변조되는 직렬 구조 문제를 믹싱 콘솔 원리를 학습해 병렬 라우팅으로 재설계 — 문제를 덮지 않고 구조부터 고치는 법
- **기술**: `Next.js` `React` `TypeScript` `Tailwind CSS` `Web Audio API` `OpenVidu(WebRTC)`

### [FinEdu — 사회초년생 금융 교육 플랫폼](https://github.com/jangms11263124/finedu)

- **서비스**: 경제·금융 입문 콘텐츠를 AI가 사용자 활동 기록 기반으로 맞춤 추천하는 교육 서비스
- **팀 / 기간**: SSAFY 관통 프로젝트 · 2인 팀 · 2026.06
- **성과**: **우수상** 수상
- **역할**: Frontend 중심 (백엔드 구현 참여)
- **한 일**:
  - Vue 3 + Pinia SPA 프론트엔드 전반
  - **2단계 RAG 추천 파이프라인** 구현 (1차 필터링 → 맞춤 추천 생성)
  - AI 오늘의 퀴즈 · 커뮤니티(게시글·댓글·좋아요) · 카카오맵 교육 행사 지도
- **기술**: `Vue 3` `Pinia` `Django REST Framework` `SQLite`

---

## SSAFY에서

- **교육**: 삼성 청년 SW·AI 아카데미 15기 (구미캠퍼스) · 2026.01 ~ 재학 중 · 관통·공통·특화·자율 프로젝트 완료
- **수상**: 관통 프로젝트 **우수상** · 공통 프로젝트 **우수상**
