<div align="center">

# 안녕하세요, 매일 기록하며 성장하는 개발자 장민석입니다.

실시간 인터랙션이 있는 웹을 만듭니다. 문제를 덮지 않고, 구조부터 고칩니다.

<a href="https://blog.naver.com/jangms1126"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/btn-blog-dark.svg"><img src="assets/btn-blog-light.svg" height="36" alt="Blog"></picture></a>&nbsp;<a href="mailto:jangms11263124@gmail.com"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/btn-email-dark.svg"><img src="assets/btn-email-light.svg" height="36" alt="Email"></picture></a>&nbsp;<a href="https://github.com/jangms11263124/TIL"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/btn-til-dark.svg"><img src="assets/btn-til-light.svg" height="36" alt="TIL"></picture></a>

</div>

---

## About Me

- **만드는 것**: 실시간 인터랙션이 있는 웹 — Web Audio 오디오 파이프라인, WebRTC 화상, 제스처 인터랙션
- **경험**: React/Next.js와 Vue 3 프로젝트를 모두 완주 — 프레임워크에 매이지 않습니다
- **습관**: 배운 것은 [TIL](https://github.com/jangms11263124/TIL)에 매일 기록
- **대표 성과**: 실시간 화상 노래방 '싸스케'로 **SSAFY 공통 프로젝트 우수상**

---

## 일하는 방식

- **꾸준함이 실력**: 하루도 빠짐없이 쓰는 TIL처럼, 매일의 축적이 성장을 만든다고 믿습니다
- **함께의 힘**: 반장·CA로 학급을 운영하며, 동료의 문제를 함께 풀 때 팀 전체가 빨라진다는 걸 배웠습니다
- **끝까지 파고들기**: 임시방편 대신 구조를 다시 설계합니다 — 오디오 엔진 라우팅을 직렬에서 병렬로 갈아엎은 것처럼

---

## Tech Stack

**Frontend**

<img src="https://skillicons.dev/icons?i=html,css,js,ts,react,nextjs,vue,pinia,tailwind,vite" alt="HTML, CSS, JavaScript, TypeScript, React, Next.js, Vue, Pinia, Tailwind CSS, Vite" />

**Backend**

<img src="https://skillicons.dev/icons?i=py,django,sqlite" alt="Python, Django, SQLite" />

**AI**

`LLM API` `RAG 파이프라인` `STT` `프롬프트 설계`

**Tools & Collaboration**

<img src="https://skillicons.dev/icons?i=git,github,gitlab,figma,vscode" alt="Git, GitHub, GitLab, Figma, VS Code" />

`Jira` `Google Stitch`

---

## Projects

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

### FinEdu — 사회초년생 금융 교육 플랫폼

- **서비스**: 경제·금융 입문 콘텐츠를 AI가 사용자 활동 기록 기반으로 맞춤 추천하는 교육 서비스
- **팀 / 기간**: SSAFY 관통 프로젝트 · 2인 팀 · 2026.06
- **역할**: Frontend 중심 (백엔드 구현 참여)
- **한 일**:
  - Vue 3 + Pinia SPA 프론트엔드 전반
  - **2단계 RAG 추천 파이프라인** 구현 (1차 필터링 → 맞춤 추천 생성)
  - AI 오늘의 퀴즈 · 커뮤니티(게시글·댓글·좋아요) · 카카오맵 교육 행사 지도
- **기술**: `Vue 3` `Pinia` `Vite` `Django REST Framework` `SQLite`

---

## SSAFY에서

- **교육**: 삼성 청년 SW·AI 아카데미 15기 (구미캠퍼스) · 2026.01 ~ 재학 중 · 1학기 이수
- **수상**: 공통 프로젝트 **우수상** · 입과 자기소개 발표 **1위**
- **리더십**: 반장 · CA — 학급 운영과 행사 진행
- **기자단**: SSAFY 공식 기자단 '싸피셜' — 캠퍼스 이야기를 [블로그](https://blog.naver.com/jangms1126)에 기록
