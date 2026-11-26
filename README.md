<div align="center">

# 안녕하세요, 장민석입니다.

화상 노래방의 오디오 엔진과 공연 티켓 앱의 예매·입장 화면을 만들었습니다.

<a href="https://blog.naver.com/jangms1126"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/btn-blog-dark.svg"><img src="assets/btn-blog-light.svg" height="36" alt="Blog"></picture></a>&nbsp;<a href="mailto:jangms1126@naver.com"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/btn-email-dark.svg"><img src="assets/btn-email-light.svg" height="36" alt="Email"></picture></a>&nbsp;<a href="https://github.com/jangms11263124/TIL"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/btn-til-dark.svg"><img src="assets/btn-til-light.svg" height="36" alt="TIL"></picture></a>

</div>

---

## About Me

- **주로 만든 것**: 싸스케의 브라우저 오디오 엔진과 화상 화면, TIMO의 예매·입장 QR 화면
- **써 본 것**: 웹은 Next.js와 Vue 3, 모바일 앱은 Flutter로 만들어 봤습니다
- **기록**: 배운 것은 [TIL](https://github.com/jangms11263124/TIL)에 날짜별로 정리합니다
- **대표 성과**: SSAFY 관통·공통 프로젝트 연속 **우수상** (FinEdu, 싸스케)

---

## 일하는 방식

- **기록해 두기**: 수업과 프로젝트에서 막혔던 것, 새로 안 것을 TIL에 남겨 두고 다음에 다시 찾아봅니다
- **의견 모아 전하기**: 1학기 CA, 2학기 반장으로 사무국 공지를 반에 전하고, 반 의견을 모아 사무국에 전했습니다. 반 행사도 기획하고 진행했습니다
- **구조부터 다시 보기**: 싸스케에서 반주 키를 바꾸면 목소리까지 같이 바뀌는 문제가 있었는데, 이펙트를 덧대는 대신 오디오 라우팅을 직렬에서 병렬로 다시 짜서 해결했습니다

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
  - 예매 흐름: 네이버 CAPTCHA, 44px 고정 칸으로 만든 사다리꼴 좌석표, 포인트 결제, 발행 대기 화면
  - 입장 QR: 30초가 지나면 흐려지고 새로고침하는 방식, 검표되면 조용한 푸시와 2초 확인으로 입장 완료 화면 전환
  - 내 티켓 상태별 카드와 메뉴 잠금 규칙, 양도 마켓 등록·취소, 알림함
  - 타이머가 있는 화면의 위젯 테스트, 프론트엔드 326개 파일 코드·주석 정리
- **배운 것**: 326개 파일을 한꺼번에 정리할 수 있었던 건 테스트 860개가 있어서였습니다. 그 뒤로는 첫 기능부터 테스트를 같이 씁니다
- **기술**: `Flutter` `Dart` `dio` `Hive` `Firebase Cloud Messaging`

### [싸스케 — 실시간 화상 노래방](https://github.com/jangms11263124/ssasukae)

- **서비스**: 화상으로 함께 부르고, 공격 카드로 방해하고, AI 가창 피드백을 받는 실시간 노래방
- **팀 / 기간**: SSAFY 공통 프로젝트 · 6인 팀 · 2026.07 ~ 2026.08
- **성과**: **우수상** 수상
- **역할**: Frontend · AI 파트 기획
- **한 일**:
  - **보컬 오디오 엔진**(Web Audio API): 반주와 마이크 채널을 나눠 반주 키와 목소리 이펙트를 따로 조절
  - **RNNoise(WASM) 노이즈 억제** 검증·이식, SoundTouch AudioWorklet으로 실시간 템포·피치 변경
  - 손 제스처로 음정·템포를 바꾸는 **제스처 DSP 인터랙션**
  - 수성전 카드 연출, 방 입장부터 공연까지의 흐름, AI 피드백·마이페이지 화면
  - AI 파트(STT + RAG 가창 피드백) 기획, 결선 발표 자료 제작
- **배운 것**: 반주 키를 바꾸면 목소리까지 같이 바뀌던 문제를 믹싱 콘솔이 채널을 나누는 방식을 공부해서 병렬 라우팅으로 다시 짰습니다. 이펙트를 하나 더 붙여 덮기보다 신호 흐름부터 다시 그려야 한다는 걸 이때 배웠습니다
- **기술**: `Next.js` `React` `TypeScript` `Tailwind CSS` `Web Audio API` `OpenVidu(WebRTC)`

### [FinEdu — 사회초년생 금융 교육 플랫폼](https://github.com/jangms11263124/finedu)

- **서비스**: 사용자 활동 기록을 바탕으로 AI가 경제·금융 입문 콘텐츠를 골라 주는 교육 서비스
- **팀 / 기간**: SSAFY 관통 프로젝트 · 2인 팀 · 2026.06
- **성과**: **우수상** 수상
- **역할**: Frontend 중심 (백엔드 구현 참여)
- **한 일**:
  - Vue 3 + Pinia로 만든 프론트엔드 전체
  - **2단계 RAG 추천**: 1차로 후보를 거르고, 2차로 사용자에게 맞는 추천을 생성
  - AI 오늘의 퀴즈, 커뮤니티(게시글·댓글·좋아요), 카카오맵 교육 행사 지도
- **기술**: `Vue 3` `Pinia` `Django REST Framework` `SQLite`

---

## SSAFY에서

- **교육**: 삼성 청년 SW·AI 아카데미 15기 (구미캠퍼스) · 2026.01 ~ 재학 중 · 관통·공통·특화·자율 프로젝트 완료
- **수상**: 관통 프로젝트 **우수상** · 공통 프로젝트 **우수상** · 입과 자기소개 발표 **1위**
- **리더십**: 반장·CA로 학급 운영과 행사 진행, 자율 프로젝트 팀장
- **기자단**: SSAFY 공식 기자단 '싸피셜'로 캠퍼스 이야기를 [블로그](https://blog.naver.com/jangms1126)에 씀
