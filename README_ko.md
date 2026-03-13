# 🎬 Awesome Seedance 2.0 — ByteDance의 시네마급 AI 비디오 모델 완전 가이드

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)
[![Atlas Cloud](https://img.shields.io/badge/API-Atlas%20Cloud-blue)](https://www.atlascloud.ai?ref=JPM683&utm_source=github&utm_campaign=awesome-seedance-2)
[![Seedance Version](https://img.shields.io/badge/Seedance-v2.0-red)](https://github.com/thoughtincode/awesome-seedance-2)

**🌐 언어:** [English](README.md) | [中文](README_zh-CN.md) | [日本語](README_ja.md) | **한국어**

> **Seedance 2.0**의 가장 포괄적인 커뮤니티 주도 가이드 — ByteDance의 혁신적인 시네마급 AI 비디오 생성 모델. 단일 생성 패스에서 동기화된 오디오-비주얼 콘텐츠를 생성합니다.

**⭐ 도움이 되셨다면 Star를 눌러주세요!**

---

## 📢 빠른 액세스 — Atlas Cloud에서 Seedance 체험하기

> **Seedance v1.5 Pro가 Atlas Cloud에서 지금 바로 사용 가능** — **$0.044/초부터**.
> Seedance 2.0 API 액세스 **곧 출시** — 지금 가입하여 먼저 경험하세요!

| | |
|---|---|
| 🚀 **지금 체험** | [**Atlas Cloud API 플랫폼 →**](https://www.atlascloud.ai?ref=JPM683&utm_source=github&utm_campaign=awesome-seedance-2) |
| 🎁 **신규 사용자 보너스** | 첫 입금 시 **25% 보너스 크레딧 (최대 $100)** |
| 🔒 **신뢰성** | SOC I & II 인증 · HIPAA 준수 · 미국 기업 |

---

## 📑 목차

- [Seedance 2.0이란?](#seedance-20이란)
- [1.5 대비 변경 사항](#15-대비-변경-사항)
- [핵심 기능 상세 분석](#핵심-기능-상세-분석)
  - [오디오-비주얼 동시 생성](#1-오디오-비주얼-동시-생성)
  - [멀티샷 네이티브 스토리텔링](#2-멀티샷-네이티브-스토리텔링)
  - [@ 레퍼런스 태그 시스템](#3--레퍼런스-태그-시스템)
  - [다국어 립싱크](#4-다국어-립싱크)
  - [물리 시뮬레이션 엔진](#5-물리-시뮬레이션-엔진)
  - [사실적인 인체 모션](#6-사실적인-인체-모션)
- [기술 사양](#기술-사양)
- [모델 비교](#모델-비교)
- [요금제](#요금제)
- [Atlas Cloud 출시 예정](#atlas-cloud-출시-예정)
- [API 빠른 시작](#api-빠른-시작)
- [프롬프트 엔지니어링 팁](#프롬프트-엔지니어링-팁)
- [활용 사례](#활용-사례)
- [자주 묻는 질문](#자주-묻는-질문)
- [커뮤니티 및 리소스](#커뮤니티-및-리소스)
- [기여하기](#기여하기)

---

## Seedance 2.0이란?

**Seedance 2.0**은 ByteDance의 차세대 AI 비디오 생성 모델로, **2026년 2월 8일~12일**에 중국 국내 즈멍(Jimeng) AI 플랫폼에서 출시되었습니다. 이것은 AI 비디오 생성의 패러다임 전환을 나타냅니다 — 단순한 텍스트-투-비디오 클립에서 **시네마급 프로덕션**으로, **동일한 생성 과정에서 동기화된 오디오를 함께 생성**합니다.

이전 세대와 대부분의 경쟁 모델이 비디오와 오디오를 별도의 생성 작업으로 처리하는 것과 달리, Seedance 2.0은 **오디오-비주얼 동시 생성 파이프라인**을 도입했습니다. 시각 콘텐츠를 생성하면서 자연스럽게 동기화된 효과음, 환경음, 대화, 음악을 함께 만들어냅니다. 이 단일 패스 접근 방식은 AI 생성 멀티미디어에서 흔히 나타나는 부자연스러운 시간적 불일치를 해소합니다.

### 비전

ByteDance는 명확한 목표를 가지고 Seedance 2.0을 개발했습니다: **AI 생성 비디오를 전문 제작 콘텐츠와 구분할 수 없는 수준으로 만들기**. 다음 기능들을 통해:

- **단일 생성으로 최대 20초** 클립
- **480p에서 2K까지의 해상도 범위**
- **네이티브 멀티샷 스토리텔링** — 더 이상 개별 클립을 이어붙일 필요 없음
- **8개 이상 언어의 립싱크**
- **물리적으로 정확한 시뮬레이션**
- **최대 12개 레퍼런스 파일**과 직관적인 @ 태그 시스템

Seedance 2.0은 점진적 업데이트가 아닌 세대적 도약이며, ByteDance를 AI 비디오 생성의 절대적 선두에 올려놓습니다.

### 출시 타임라인

| 날짜 | 이벤트 |
|------|--------|
| 2026년 2월 8일 | 즈멍 AI 플랫폼 프리뷰 (중국) |
| 2026년 2월 12일 | 중국 국내 정식 출시 |
| 2026년 Q1~Q2 (예상) | 글로벌 API 액세스 (지연 중) |
| 미정 | Atlas Cloud에서 이용 가능 |

> **참고:** 글로벌 API 출시는 지연되고 있지만, [Atlas Cloud](https://www.atlascloud.ai?ref=JPM683&utm_source=github&utm_campaign=awesome-seedance-2)에서 **Seedance v1.5 Pro**를 $0.044/초부터로 지금 바로 사용할 수 있습니다.

---

## 1.5 대비 변경 사항

Seedance 2.0은 1.5에서 대폭 진화했습니다:

| 기능 | Seedance 1.5 | Seedance 2.0 |
|------|-------------|--------------|
| **오디오 생성** | ❌ 비디오만 | ✅ 오디오-비주얼 동시 생성 |
| **최대 길이** | ~5초/클립 | **최대 20초/클립** |
| **해상도** | 최대 1080p | **480p~2K** |
| **멀티샷** | ❌ 싱글샷만 | ✅ 네이티브 멀티샷 |
| **레퍼런스 파일** | 제한적 | **최대 12개 + @ 태그** |
| **립싱크** | 기본, 영어 중심 | **8개 이상 언어** |
| **물리 시뮬레이션** | 기본적 | **고급 물리 시뮬레이션** |
| **인체 모션** | 때때로 부자연스러움 | **사실적이고 자연스러운 동작** |
| **효과음** | ❌ 없음 | ✅ 동기화된 효과음 |
| **환경음** | ❌ 없음 | ✅ 환경 매칭 오디오 |
| **API 이용 가능성** | ✅ 글로벌 (Atlas Cloud) | 🟡 중국만 (글로벌 곧 출시) |
| **가격 (예상)** | $0.044/초부터 | $0.10~$0.80/분 |

### 주요 개선 사항

1. **4배 긴 클립** — ~5초에서 최대 20초로
2. **오디오 혁명** — 오디오와 비디오를 동시에 동기 생성하는 최초의 주요 모델
3. **스토리 대응** — 네이티브 멀티샷으로 내러티브 제작 가능
4. **범용 립싱크** — 한국어 포함 8개 이상 언어 지원
5. **레퍼런스 파워** — 12개 파일의 @ 태그로 캐릭터와 스타일 일관성 보장
6. **리얼 물리** — 물이 흐르고, 천이 드리워지고, 물체가 실제 물리법칙 따름

---

## 핵심 기능 상세 분석

### 1. 오디오-비주얼 동시 생성

Seedance 2.0의 플래그십 기능이자 시장의 모든 다른 모델과의 차별화 포인트입니다.

**작동 방식:**
- 비디오와 오디오가 모델의 **단일 포워드 패스**에서 동시에 생성
- 오디오는 비디오 생성 후 "추가"되는 것이 아님 — 동시에 생성
- 시각 이벤트와 사운드 간의 완벽한 시간적 동기화 보장

**생성되는 오디오 종류:**
- **효과음** — 문이 닫히는 프레임에서 정확히 문 닫히는 소리가 남
- **환경음** — 숲 장면에는 새소리와 바람에 나뭇잎 흔들리는 소리
- **대화 오디오** — 자연스러운 음성 합성으로 캐릭터의 대사
- **BGM** — 비주얼의 분위기와 페이스에 맞는 배경 음악

**이것이 중요한 이유:**
이전 접근 방식:
1. 비디오 생성
2. 비디오 내용 분석
3. 오디오 별도 생성
4. 오디오를 비디오에 맞춤 (종종 불완전)

Seedance 2.0은 2~4단계를 제거하여 처음부터 자연스러운 시네마틱 콘텐츠를 생성합니다.

```
프롬프트 예시:
"바리스타가 바쁜 카페에서 우유를 스팀하고 있다. 에스프레소 머신이
쉬익 소리를 내고, 컵이 소서 위에서 딸깍거리며, 부드러운 재즈가
배경에서 흐른다. 카메라가 바리스타의 손에서 고객의 미소로 천천히
패닝한다."

결과: 비디오 + 완벽하게 동기화된 카페 환경음, 머신 소리, BGM — 모두 한 번에 생성.
```

### 2. 멀티샷 네이티브 스토리텔링

이전 AI 비디오 모델은 단일 연속 샷만 생성할 수 있었습니다. 스토리를 만들려면 여러 개별 클립을 생성하고 수동으로 편집해야 했으며, 캐릭터, 조명, 스타일의 불일치가 빈번했습니다.

**Seedance 2.0은 이를 근본적으로 변경합니다:**

- **단일 프롬프트에서 여러 샷 정의** — 모델이 "컷 투", "디졸브 투", "다음 장면" 등의 영화 용어를 이해
- **자동 일관성** — 샷 간 캐릭터 외모 유지
- **조명 연속성** — 장면 간 조명이 자연스럽게 변화
- **페이싱 제어** — 모델이 내러티브 리듬을 이해

**멀티샷 프롬프트 예시:**
```
샷 1: 밤, 네온 불빛으로 빛나는 도쿄 거리의 와이드 이스태블리싱
샷, 비가 내린다. 3초.

샷 2: 젊은 여성이 우산을 펴고 네온 사인을 올려다보는 미디엄 샷.
웅덩이에 그녀의 반사가 보인다. 4초.

샷 3: 미소 짓는 그녀의 얼굴 클로즈업. 뺨에 빗방울,
동공에 네온 색상이 반사. 3초.

샷 4: 뒤에서 본 와이드 샷. 우산을 들고 거리를 걸으며
군중 속으로 사라진다. 5초.
```

이것은 일관된 캐릭터 외모, 자연스러운 트랜지션, 전편에 걸쳐 동기화된 비 소리를 가진 **15초 미니 필름**을 생성합니다.

### 3. @ 레퍼런스 태그 시스템

Seedance 2.0에서 가장 실용적인 혁신 중 하나인 레퍼런스 파일용 **@ 태그 시스템**입니다.

**작동 방식:**
- 최대 **12개 레퍼런스 파일** 업로드 (이미지, 비디오 클립, 스타일 레퍼런스)
- 프롬프트에서 각 레퍼런스에 **@ 식별자** 태그
- 모델이 지정한 위치에서 각 레퍼런스를 정확하게 적용

**지원되는 레퍼런스 유형:**
| 레퍼런스 유형 | 용도 | 예시 |
|-------------|------|------|
| 캐릭터 얼굴 | 장면 간 캐릭터 일관성 | @character_mina |
| 스타일 레퍼런스 | 비주얼 스타일 매칭 | @style_noir |
| 환경 | 로케이션 일관성 | @location_office |
| 오브젝트 | 특정 오브젝트 포함 | @object_vintage_car |
| 모션 | 움직임 스타일 레퍼런스 | @motion_dance |
| 의상 | 의상 일관성 | @outfit_hanbok |

### 4. 다국어 립싱크

Seedance 2.0은 **8개 이상 언어**의 자연스러운 립싱크를 지원합니다:

| 언어 | 품질 | 비고 |
|------|------|------|
| 🇨🇳 중국어 (보통화) | ⭐⭐⭐⭐⭐ | 네이티브 수준 |
| 🇺🇸 영어 | ⭐⭐⭐⭐⭐ | 우수 |
| 🇯🇵 일본어 | ⭐⭐⭐⭐ | 매우 좋음 |
| 🇰🇷 한국어 | ⭐⭐⭐⭐ | 매우 좋음 |
| 🇪🇸 스페인어 | ⭐⭐⭐⭐ | 매우 좋음 |
| 🇫🇷 프랑스어 | ⭐⭐⭐⭐ | 매우 좋음 |
| 🇩🇪 독일어 | ⭐⭐⭐⭐ | 매우 좋음 |
| 🇧🇷 포르투갈어 | ⭐⭐⭐⭐ | 매우 좋음 |

**주요 기능:**
- 각 언어에 대한 정확한 음소-비점 매핑
- 자연스러운 턱, 입술, 혀 움직임
- 발화 중 감정 표현 지원
- 생성된 오디오 트랙과 제공된 오디오 트랙 모두 호환

### 5. 물리 시뮬레이션 엔진

Seedance 2.0에는 AI 생성 비디오에 사실적인 물리적 상호작용을 제공하는 물리 시뮬레이션 엔진이 내장되어 있습니다:

**지원되는 물리 시뮬레이션:**
- **유체 역학** — 물튀김, 액체 따르기, 비, 파도
- **천 시뮬레이션** — 천의 드레이프, 바람에 의한 의복 효과, 커튼
- **강체 물리** — 물체의 낙하, 충돌, 바운스
- **소프트 바디 물리** — 변형 가능한 오브젝트, 젤리, 고무
- **파티클 시스템** — 연기, 불, 불꽃, 먼지
- **머리카락과 모피** — 자연스러운 움직임과 바람 상호작용

### 6. 사실적인 인체 모션

Seedance 2.0에서 가장 눈에 띄는 개선은 인체 움직임 처리입니다:

- **해부학적으로 정확한** 관절 움직임
- **자연스러운 보행** — 걷기, 달리기, 회전이 인간다움
- **손 디테일** — 손가락이 자연스럽게 움직임 (AI 비디오의 약점)
- **얼굴 미세 표정** — 미묘한 감정 변화가 가시적
- **전신 조화** — 걸을 때 자연스러운 팔 흔들림, 회전 시 무게 중심 이동
- **그룹 다이내믹스** — 같은 장면에서 여러 인물이 자연스럽게 상호작용

---

## 기술 사양

| 사양 | 상세 |
|------|------|
| **모델명** | Seedance 2.0 |
| **개발사** | ByteDance |
| **출시일** | 2026년 2월 8일~12일 |
| **플랫폼** | 즈멍 AI (중국 국내) |
| **생성 모드** | 텍스트→비디오, 이미지→비디오, 비디오→비디오 |
| **오디오** | 오디오-비주얼 동시 생성 |
| **최대 길이** | 클립당 최대 20초 |
| **해상도 범위** | 480p, 720p, 1080p, 2K |
| **화면비** | 16:9, 9:16, 1:1, 4:3, 3:4, 21:9 |
| **멀티샷** | 네이티브 지원 |
| **레퍼런스 파일** | 최대 12개 + @ 태그 |
| **립싱크 언어** | 8+ (중, 영, 일, 한, 서, 불, 독, 포) |
| **물리 엔진** | 내장 시뮬레이션 |
| **출력 형식** | MP4 (비디오), WAV/AAC (오디오) |
| **API 상태** | 중국 국내만 (글로벌 지연 중) |

---

## 모델 비교

### Seedance 2.0 vs 1.5 vs Kling 3.0 vs Wan 2.6 vs Sora 2

| 기능 | Seedance 2.0 | Seedance 1.5 | Kling 3.0 | Wan 2.6 | Sora 2 |
|------|-------------|--------------|-----------|---------|--------|
| **개발사** | ByteDance | ByteDance | Kuaishou | Alibaba | OpenAI |
| **오디오-비디오 동시** | ✅ | ❌ | ❌ | ❌ | 🟡 제한적 |
| **최대 길이** | 20초 | ~5초 | 10초 | 8초 | 20초 |
| **최고 해상도** | 2K | 1080p | 2K | 1080p | 1080p |
| **멀티샷** | ✅ 네이티브 | ❌ | 🟡 기본적 | ❌ | 🟡 기본적 |
| **레퍼런스** | 12 (@ 태그) | 제한적 | 3~5 | 2~3 | 5 |
| **립싱크** | 8개 이상 | 영어 | 5개 이상 | 3개 이상 | 6개 이상 |
| **물리** | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐⭐ |
| **인체 모션** | ⭐⭐⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐⭐ | ⭐⭐⭐ | ⭐⭐⭐⭐ |
| **글로벌 API** | 🟡 곧 출시 | ✅ | ✅ | ✅ | ✅ |
| **가격** | $0.10~$0.80/분 | $0.044/초부터 | ~$0.30/초부터 | ~$0.15/초부터 | ~$0.50/초부터 |

### 핵심 포인트

1. **오디오-비주얼 동시 생성 리더** — 진정한 단일 패스 오디오-비디오 생성을 제공하는 유일한 모델
2. **최다 레퍼런스 파일** — 12개 파일 + @ 태그
3. **최고의 멀티샷** — 네이티브 스토리텔링
4. **가장 넓은 립싱크** — 8개 이상 언어
5. **최상위 물리** — 모든 모델 중 가장 사실적인 물리
6. **글로벌 API 대기 중** — 현재 중국만 이용 가능이 주요 단점

> **팁:** Seedance 2.0 글로벌 API를 기다리는 동안 [Atlas Cloud](https://www.atlascloud.ai?ref=JPM683&utm_source=github&utm_campaign=awesome-seedance-2)에서 **Seedance v1.5 Pro**를 **$0.044/초부터**로 지금 바로 이용하세요.

---

## 요금제

### Seedance 2.0 예상 가격

| 해상도 | 예상 가격 | 비고 |
|--------|---------|------|
| 480p | ~$0.05/분 | 드래프트용 저예산 옵션 |
| 720p | **~$0.10/분** | 대부분의 사용 사례에 최적 |
| 1080p | ~$0.30/분 | 표준 프로덕션 품질 |
| 2K | **~$0.80/분** | 시네마급 출력 |

*가격은 예상치이며, 글로벌 출시 시 변경될 수 있습니다.*

### Seedance 1.5 Pro — Atlas Cloud에서 지금 이용 가능

| 플랜 | 가격 | 내용 |
|------|------|------|
| **종량제** | **$0.044/초부터** | 약정 없음, 비디오당 과금 |
| **첫 입금 보너스** | **25% 추가 크레딧** | 최대 $100 보너스 |

### Atlas Cloud를 선택하는 이유

| 장점 | 상세 |
|------|------|
| 🚀 **즉시 액세스** | 대기 없이 바로 생성 시작 |
| 💰 **경쟁력 있는 가격** | Seedance v1.5 Pro $0.044/초부터 |
| 🎁 **신규 사용자 보너스** | 첫 입금 25% 보너스 (최대 $100) |
| 🔌 **간단한 API** | OpenAI 호환 포맷 |
| 🔒 **SOC I & II 인증** | 엔터프라이즈급 보안 |
| 🏥 **HIPAA 준수** | 의료 애플리케이션에 안전 |
| 🇺🇸 **미국 기업** | 미국 데이터 센터 |

> **[지금 가입 →](https://www.atlascloud.ai?ref=JPM683&utm_source=github&utm_campaign=awesome-seedance-2)** 첫 입금 시 **25% 보너스 크레딧 (최대 $100)**!

---

## Atlas Cloud 출시 예정

### Seedance 2.0 — 곧 출시!

Atlas Cloud는 Seedance 2.0을 글로벌 API 플랫폼에 도입하기 위해 적극적으로 준비하고 있습니다.

**현재 상태:**
- ✅ **Seedance v1.5 Pro** — 이용 가능, $0.044/초부터
- 🔜 **Seedance 2.0** — 글로벌 API 출시 후 대응 예정

**지금 가입해야 하는 이유:**

1. **선행 액세스** — 조기 가입자가 Seedance 2.0 우선 액세스
2. **v1.5로 준비** — Seedance 1.5 Pro로 API에 익숙해지기
3. **보너스 확보** — 첫 입금 25% 보너스 지금 이용 가능
4. **동일 API 포맷** — v1.5 코드가 v2.0에서도 거의 그대로 작동

### 가입 절차

| 단계 | 액션 |
|------|------|
| 1 | [Atlas Cloud](https://www.atlascloud.ai?ref=JPM683&utm_source=github&utm_campaign=awesome-seedance-2) 방문 |
| 2 | 무료 계정 생성 |
| 3 | 크레딧 입금 (25% 보너스, 최대 $100) |
| 4 | Seedance v1.5 Pro 바로 사용 시작 |
| 5 | Seedance 2.0 출시 알림 받기 |

---

## API 빠른 시작

Seedance 2.0의 글로벌 API가 준비 중인 동안, Atlas Cloud에서 **Seedance v1.5 Pro**로 지금 바로 개발을 시작할 수 있습니다.

### 사전 준비

```bash
pip install requests
```

### 인증

```python
import requests

# Atlas Cloud API 키
API_KEY = "your_atlas_cloud_api_key"
BASE_URL = "https://api.atlascloud.ai/v1"

headers = {
    "Authorization": f"Bearer {API_KEY}",
    "Content-Type": "application/json"
}
```

### 텍스트-투-비디오 (Seedance v1.5 Pro)

```python
import requests
import time

def generate_video(prompt, aspect_ratio="16:9"):
    """
    Atlas Cloud의 Seedance v1.5 Pro로 비디오 생성.
    Seedance 2.0 출시 시 audio_enabled, multi_shot,
    reference_files 등의 파라미터가 추가될 예정.
    """
    url = f"{BASE_URL}/video/generations"

    payload = {
        "model": "seedance-v1.5-pro",
        "prompt": prompt,
        "aspect_ratio": aspect_ratio,
    }

    response = requests.post(url, json=payload, headers=headers)
    result = response.json()

    prediction_id = result["id"]
    print(f"생성 시작: {prediction_id}")

    # 완료까지 폴링
    while True:
        status_response = requests.get(
            f"{BASE_URL}/predictions/{prediction_id}",
            headers=headers
        )
        status = status_response.json()

        if status["status"] == "succeeded":
            print(f"비디오 완성: {status['output']['video_url']}")
            return status["output"]["video_url"]
        elif status["status"] == "failed":
            print(f"생성 실패: {status.get('error', '알 수 없는 오류')}")
            return None

        time.sleep(5)

# 사용 예시
video_url = generate_video(
    "골든 리트리버가 햇살 가득한 초원을 달리고 있다, "
    "야생화가 바람에 흔들린다, 시네마틱 조명, "
    "슬로우 모션, 4K 품질"
)
```

### 이미지-투-비디오 (Seedance v1.5 Pro)

```python
def image_to_video(image_url, prompt, aspect_ratio="16:9"):
    """
    Seedance v1.5 Pro로 이미지에서 비디오 생성.
    """
    url = f"{BASE_URL}/video/generations"

    payload = {
        "model": "seedance-v1.5-pro",
        "prompt": prompt,
        "image_url": image_url,
        "aspect_ratio": aspect_ratio,
    }

    response = requests.post(url, json=payload, headers=headers)
    result = response.json()

    prediction_id = result["id"]
    print(f"생성 시작: {prediction_id}")

    while True:
        status_response = requests.get(
            f"{BASE_URL}/predictions/{prediction_id}",
            headers=headers
        )
        status = status_response.json()

        if status["status"] == "succeeded":
            print(f"비디오 완성: {status['output']['video_url']}")
            return status["output"]["video_url"]
        elif status["status"] == "failed":
            print(f"생성 실패: {status.get('error', '알 수 없는 오류')}")
            return None

        time.sleep(5)

# 사용 예시
video_url = image_to_video(
    image_url="https://example.com/portrait.jpg",
    prompt="인물이 천천히 고개를 돌려 미소 짓는다, "
           "부드러운 자연광, 머리카락이 미풍에 나부낀다"
)
```

### 예상되는 Seedance 2.0 API 포맷

```python
# 예상되는 Seedance 2.0 API 포맷 (아직 이용 불가)
payload = {
    "model": "seedance-v2.0",
    "prompt": "샷 1: 비 내리는 도쿄 거리의 와이드 샷...",
    "aspect_ratio": "16:9",
    "resolution": "2k",          # 신규: 480p, 720p, 1080p, 2k
    "duration": 15,              # 신규: 최대 20초
    "audio_enabled": True,       # 신규: 오디오-비주얼 동시 생성
    "multi_shot": True,          # 신규: 멀티샷
    "reference_files": [         # 신규: @ 태그 시스템
        {
            "tag": "@hero",
            "url": "https://example.com/hero_face.jpg"
        },
        {
            "tag": "@style",
            "url": "https://example.com/noir_style.jpg"
        }
    ],
    "lip_sync": {                # 신규: 다국어 립싱크
        "enabled": True,
        "language": "ko"
    }
}
```

> **참고:** 위 v2.0 포맷은 기능 발표를 기반으로 한 예상이며, 실제 API 파라미터는 다를 수 있습니다.

---

## 프롬프트 엔지니어링 팁

### 1. 프롬프트 구조화

```
[피사체] + [액션] + [설정] + [조명] + [카메라] + [스타일] + [무드]
```

**예시:**
```
젊은 여성 (피사체)이 버려진 무도회장에서 우아하게 춤춘다 (액션),
깨진 창문으로 금빛 햇살이 들어온다 (조명),
느린 돌리 인 (카메라), 시네마틱 필름 그레인 (스타일),
우울하면서도 아름다운 (무드)
```

### 2. 영화 용어 사용

| 용어 | 효과 |
|------|------|
| "돌리 인/아웃" | 카메라가 피사체에 접근/이동 |
| "트래킹 샷" | 움직이는 피사체를 추적 |
| "크레인 샷" | 카메라가 상승/하강 |
| "더치 앵글" | 기울어진 카메라로 긴장감 |
| "랙 포커스" | 피사체 간 포커스 전환 |
| "슬로우 모션" | 재생 속도 감소 |
| "타임랩스" | 시간 가속 |
| "아나모픽" | 와이드 시네마틱 |
| "얕은 피사계 심도" | 배경 블러 |

### 3. 조명 구체적으로 지정

```
좋음: "골든 아워 역광, 렌즈 플레어, 따뜻한 색온도"
나쁨: "예쁜 조명"

좋음: "위에서 내리쬐는 형광등, 그린 틴트, 클리니컬한 느낌"
나쁨: "밝은 빛"
```

### 4. 멀티샷 프롬프트 구조

```
샷 1: [시간] [샷 타입] [설명]
샷 2: [시간] [샷 타입] [설명]
샷 3: [시간] [샷 타입] [설명]
```

### 5. 오디오 프롬프팅 (Seedance 2.0)

```
좋음: "양철 지붕에 비가 두드리고, 멀리서 천둥이 구르며, 고양이가
창턱에서 조용히 그르릉거린다. 실내는 따뜻하고 아늑하다."
```

---

## 활용 사례

### 🎬 영화 & 엔터테인먼트

- **프리비주얼라이제이션** — 촬영 전 장면 시각화
- **콘셉트 트레일러** — 피치 프레젠테이션용 콘셉트 트레일러
- **VFX 프리비즈** — 예산 투입 전 시각 효과 콘셉트 테스트
- **단편 영화** — 멀티샷으로 완전한 단편 영화 제작
- **뮤직 비디오** — 음악에 동기화된 비주얼 콘텐츠

### 📱 소셜 미디어 & 마케팅

- **제품 쇼케이스** — 이커머스용 동적 제품 비디오
- **광고 크리에이티브 테스트** — 여러 광고 변형을 빠르게 생성
- **SNS 콘텐츠** — TikTok/Reels용 9:16, YouTube용 16:9
- **브랜드 스토리텔링** — 멀티샷 브랜드 내러티브 비디오

### 🏢 엔터프라이즈

- **교육 비디오** — 일관된 캐릭터의 교육 콘텐츠
- **사내 커뮤니케이션** — 회사 업데이트용 비주얼
- **프레젠테이션** — 키노트의 다이내믹 비주얼

### 🎓 교육

- **역사 재현** — 역사적 사건의 시각화
- **과학적 시각화** — 복잡한 과학 과정을 시각적으로
- **언어 학습** — 8개 이상 언어의 립싱크로 발음 연습

### 🛍️ 이커머스

- **제품 비디오** — 제품 이미지에서 쇼케이스 비디오 생성
- **라이프스타일 콘텐츠** — 열망적인 생활 장면에서의 제품 전시
- **360° 뷰** — 동적 제품 회전 비디오

---

## 자주 묻는 질문

**Q1: Seedance 2.0이란 무엇인가요?**

ByteDance의 최신 AI 비디오 생성 모델로 2026년 2월에 출시되었습니다. 시네마급 비디오와 동기화된 오디오를 단일 생성 패스에서 생성하는 최초의 주요 모델입니다.

**Q2: 글로벌에서 이용할 수 있나요?**

아직 아닙니다. 2026년 3월 현재 중국 즈멍 AI 플랫폼에서만 이용 가능합니다. [Atlas Cloud](https://www.atlascloud.ai?ref=JPM683&utm_source=github&utm_campaign=awesome-seedance-2)에서 **Seedance v1.5 Pro**는 지금 바로 사용할 수 있습니다.

**Q3: Seedance 2.0은 언제 Atlas Cloud에서 이용 가능한가요?**

ByteDance가 글로벌 API를 출시하는 즉시 Atlas Cloud가 통합합니다. 지금 가입하여 알림과 우선 액세스를 받으세요.

**Q4: 최대 비디오 길이는?**

1회 생성으로 최대 **20초**. 멀티샷 스토리텔링으로 해당 시간 내에 여러 샷을 포함한 내러티브 생성 가능.

**Q5: 립싱크는 몇 개 언어를 지원하나요?**

8개 이상: 중국어, 영어, 일본어, 한국어, 스페인어, 프랑스어, 독일어, 포르투갈어.

**Q6: @ 레퍼런스 태그 사용법은?**

레퍼런스 파일(이미지나 비디오 클립)을 업로드하고 각 파일에 @ 태그를 지정합니다. 프롬프트에서 태그를 참조하면 모델이 해당 레퍼런스를 적용합니다. 1회 생성당 최대 12개 파일.

**Q7: Atlas Cloud는 안전한가요?**

네. SOC I & II 인증, HIPAA 준수, 미국 기반 기업입니다.

**Q8: v1.5 코드가 v2.0에서도 작동하나요?**

API 포맷이 매우 유사할 것으로 예상됩니다. 기존 v1.5 코드는 오디오 생성, 멀티샷 등 새 기능용 파라미터 추가 정도의 수정으로 작동할 것입니다.

**Q9: 요금은 얼마인가요?**

Seedance v1.5 Pro는 $0.044/초부터로 Atlas Cloud에서 지금 이용 가능. 2.0은 720p에서 ~$0.10/분~2K에서 ~$0.80/분으로 예상됩니다.

*표시된 가격은 시작 가격입니다. 더 높은 해상도나 긴 영상은 추가 비용이 발생할 수 있습니다.*

**Q10: 추천 보너스는 어떻게 사용하나요?**

[추천 링크](https://www.atlascloud.ai?ref=JPM683&utm_source=github&utm_campaign=awesome-seedance-2)로 가입하면 첫 입금 시 **25% 보너스 (최대 $100)**를 받을 수 있습니다.

---

## 커뮤니티 및 리소스

### 공식 리소스

- [즈멍 AI 플랫폼](https://www.jimeng.jianying.com/) — 공식 플랫폼 (중국)
- [ByteDance Research](https://research.bytedance.com/) — 연구 논문 및 공지
- [Atlas Cloud](https://www.atlascloud.ai?ref=JPM683&utm_source=github&utm_campaign=awesome-seedance-2) — Seedance 글로벌 API 액세스

### 커뮤니티

- [GitHub Discussions](https://github.com/thoughtincode/awesome-seedance-2/discussions) — 질문, 결과 공유
- [Issues](https://github.com/thoughtincode/awesome-seedance-2/issues) — 문제 보고 또는 추가 제안

---

## 기여하기

기여를 환영합니다! 다음 절차를 따라주세요:

1. 이 저장소를 **Fork**
2. 기능 브랜치 **생성** (`git checkout -b feature/amazing-addition`)
3. 변경 사항 **커밋** (`git commit -m 'Add amazing addition'`)
4. 브랜치에 **푸시** (`git push origin feature/amazing-addition`)
5. **Pull Request** 생성

---

## 🚀 지금 바로 Seedance로 제작을 시작하세요!

| | |
|---|---|
| 🎬 **모델** | Seedance v1.5 Pro (v2.0 곧 출시) |
| 💰 **가격** | $0.044/초부터 |
| 🎁 **보너스** | 첫 입금 25% 추가 크레딧 (최대 $100) |
| 🔗 **가입** | [**atlascloud.ai →**](https://www.atlascloud.ai?ref=JPM683&utm_source=github&utm_campaign=awesome-seedance-2) |

> **[지금 시작하기 → atlascloud.ai](https://www.atlascloud.ai?ref=JPM683&utm_source=github&utm_campaign=awesome-seedance-2)**

---

<div align="center">

### 신뢰 & 보안

🔒 **SOC I & II 인증** | 🏥 **HIPAA 준수** | 🇺🇸 **미국 기업**

---

**[Atlas Cloud](https://www.atlascloud.ai?ref=JPM683&utm_source=github&utm_campaign=awesome-seedance-2)** — 세계 최고의 AI 모델로 향하는 게이트웨이

[![가입하기](https://img.shields.io/badge/가입하기-Atlas%20Cloud-blue?style=for-the-badge)](https://www.atlascloud.ai?ref=JPM683&utm_source=github&utm_campaign=awesome-seedance-2)

---

AI 비디오 커뮤니티가 ❤️을 담아 제작

[⬆ 맨 위로 돌아가기](#-awesome-seedance-20--bytedance의-시네마급-ai-비디오-모델-완전-가이드)

</div>
