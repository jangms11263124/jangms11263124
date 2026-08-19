<div align="center">

# 안녕하세요, 매일 기록하며 성장하는 개발자 장민석입니다.

실시간 인터랙션이 있는 웹을 만듭니다. 문제를 덮지 않고, 구조부터 고칩니다.

<a href="https://blog.naver.com/jangms1126"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/btn-blog-dark.svg"><img src="assets/btn-blog-light.svg" height="36" alt="Blog"></picture></a>&nbsp;<a href="mailto:jangms11263124@gmail.com"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/btn-email-dark.svg"><img src="assets/btn-email-light.svg" height="36" alt="Email"></picture></a>&nbsp;<a href="https://github.com/jangms11263124/TIL"><picture><source media="(prefers-color-scheme: dark)" srcset="assets/btn-til-dark.svg"><img src="assets/btn-til-light.svg" height="36" alt="TIL"></picture></a>

</div>

---

## About Me

**소리와 영상이 실시간으로 오가는 웹**, 사용자가 만지는 순간 반응하는 경험을 만드는 일에 강점이 있습니다. Web Audio 오디오 파이프라인 설계부터 WebRTC 화상 스트림, 제스처 인터랙션까지 — 실시간 미디어를 다루는 프론트엔드가 저의 무기입니다.

삼성 청년 SW·AI 아카데미(**SSAFY 15기**)에서 개발 역량을 쌓고 있고, React/Next.js와 Vue 3 프로젝트를 모두 완주해 프레임워크에 매이지 않습니다. 배운 것은 [TIL](https://github.com/jangms11263124/TIL)에 **매일** 기록합니다.

실시간 화상 노래방 **'싸스케'** 에서 보컬 오디오 엔진과 제스처 인터랙션을 주도적으로 개발해 **SSAFY 공통 프로젝트 우수상**을 받았습니다.

---

## 일하는 방식

- **꾸준함이 실력** — 하루도 빠짐없이 쓰는 TIL처럼, 매일의 축적이 성장을 만든다고 믿습니다.
- **함께의 힘** — 반장·CA로 학급을 운영하며, 동료의 문제를 함께 풀 때 팀 전체가 빨라진다는 걸 배웠습니다.
- **끝까지 파고들기** — 임시방편 대신 구조를 다시 설계합니다. 오디오 엔진 라우팅을 직렬에서 병렬로 갈아엎은 것처럼요.

---

## Tech Stack

**Frontend**

<img src="https://skillicons.dev/icons?i=html,css,js,ts,react,nextjs,vue,pinia,tailwind,vite" alt="HTML, CSS, JavaScript, TypeScript, React, Next.js, Vue, Pinia, Tailwind CSS, Vite" />

**Backend**

<img src="https://skillicons.dev/icons?i=py,django,sqlite" alt="Python, Django, SQLite" />

**AI**

**OpenAI API**(GPT·Whisper)와 **Gemini**를 활용합니다 — FinEdu에서 2단계 RAG 추천 파이프라인을 구현했고, 싸스케에서 STT + RAG 가창 피드백 파이프라인을 기획했습니다.

**Tools & Collaboration**

<img src="https://skillicons.dev/icons?i=git,github,gitlab,figma,vscode" alt="Git, GitHub, GitLab, Figma, VS Code" />

그 외 — **Jira**로 협업 이슈를 관리하고, **Google Stitch**로 화면을 설계합니다.

---

## Projects

### [싸스케 — 실시간 화상 노래방](https://github.com/jangms11263124/ssasukae)

SSAFY 15기 공통 프로젝트 **우수상** · 6인 팀 · 2026.07 ~ 2026.08

**어떤 서비스인가요**
친구들과 화상으로 만나 함께 부르고, 공격 카드로 서로를 방해하고, AI에게 가창 피드백을 받는 실시간 화상 노래방입니다. OpenVidu(WebRTC) 화상, 수성전 카드 배틀, 실시간 가창 채점, Whisper STT + RAG 기반 AI 피드백을 갖췄습니다.

**무엇을 맡았나요** — Frontend · AI 파트 기획
- Web Audio API 기반 **보컬 오디오 엔진** 설계·구현 — MR/마이크 채널을 분리하는 병렬 라우팅으로 반주 키와 목소리 이펙트를 독립 제어
- **RNNoise(WASM) 노이즈 억제**를 데모로 검증 후 서비스에 이식, SoundTouch AudioWorklet으로 실시간 템포·피치 시프트
- 손 제스처로 음정·템포를 조절하는 **제스처 DSP 인터랙션**, 수성전 카드 연출, 방 플로우, AI 피드백·마이페이지 화면
- AI 파트 기획, 결선 발표 자료 제작

**무엇을 배웠나요**
초기 직렬 오디오 구조에서 MR 키를 바꾸면 목소리까지 변조되는 문제를 만났고, 실제 믹싱 콘솔 원리를 학습해 병렬 라우팅으로 재설계했습니다. 문제를 덮지 않고 구조부터 고치는 법을 배웠습니다.

### FinEdu — 사회초년생 금융 교육 플랫폼

SSAFY 15기 관통 프로젝트 · 2인 팀 · 2026.06

**어떤 서비스인가요**
경제·금융 입문 콘텐츠를 모아 AI가 사용자 활동 기록 기반으로 맞춤 추천하는 금융 교육 서비스입니다. Gemini → GPT-4o-mini 2단계 RAG 추천, AI 오늘의 퀴즈, 커뮤니티, 카카오맵 교육 행사 지도를 담았습니다.

**무엇을 맡았나요**
Vue 3 + Pinia SPA 프론트엔드 전반을 담당했고, 2인 팀이라 Django REST Framework 백엔드 구현에도 참여했습니다.

---

## SSAFY에서

- **SSAFY 15기 (구미캠퍼스)** — 2026.01 ~ 재학 중 · 1학기 이수 · 공통 프로젝트 우수상
- **반장 · CA** — 학급 운영과 행사 진행을 이끌었습니다.
- **공식 기자단 '싸피셜'** — 캠퍼스 이야기를 취재해 [블로그](https://blog.naver.com/jangms1126)에 기록했습니다.
- **입과 자기소개 발표 1위** — 사람들 앞에서 저를 전달하는 일에 자신 있습니다.
