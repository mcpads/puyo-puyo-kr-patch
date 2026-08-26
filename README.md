# 뿌요뿌요 시리즈 한글 번역 프로젝트

컴파일사의 대표작 뿌요뿌요(ぷよぷよ) 시리즈의 한글 번역 패치를 배포하는 프로젝트입니다.

Claude Code / Codex를 활용하여 리버싱/번역하고, 사람이 기초 검수를 진행한 프로젝트입니다.

더 많은 게임의 번역에 대한 기여를 위해, 모든 패치에 사용된 코드는 기기별로 공개됩니다.

> 자매 프로젝트 - [마도물어 시리즈 한글 번역 프로젝트](https://github.com/mcpads/madou-monogatari-kr-patch)

## 목차

- [뿌요뿌욘 (드림캐스트)](#뿌요뿌욘-드림캐스트)
- [뿌요뿌요 DA! (드림캐스트, 베타)](#뿌요뿌요-da-드림캐스트-베타)
- [슈퍼 뿌요뿌요 2 (SNES)](#슈퍼-뿌요뿌요-2-snes)
- [슈퍼 나조 뿌요 1 (SNES)](#슈퍼-나조-뿌요-1-snes)
- [슈퍼 나조 뿌요 2 (SNES)](#슈퍼-나조-뿌요-2-snes)
- [번역 예정 작품](#번역-예정-작품)
- [이슈 제보 및 피드백](#이슈-제보-및-피드백)
- [업데이트 기록](#업데이트-기록)
- [라이선스](#라이선스)

## 뿌요뿌욘 (드림캐스트)

드림캐스트 **뿌요뿌욘 (ぷよぷよ~ん, Puyo Puyo 4)** 한글 번역 패치입니다.

참고: [뿌요뿌욘 - 나무위키](https://namu.wiki/w/%EB%BF%8C%EC%9A%94%EB%BF%8C%EC%9A%98)

![dc-puyo-puyo-screenshot-1](/img/dc-puyo-puyo-screenshot-1.png)

![dc-puyo-puyo-screenshot-2](/img/dc-puyo-puyo-screenshot-2.png)

![dc-puyo-puyo-screenshot-3](/img/dc-puyo-puyo-screenshot-3.png)

### 적용 방법

1. **일본판 원본 GDI ROM**을 준비합니다
2. [Puyo Puyo 4 (Dreamcast) KR v1.0.1.dcp](https://raw.githubusercontent.com/mcpads/puyo-puyo-kr-patch/main/Puyo%20Puyo%204%20(Dreamcast)%20KR%20v1.0.1.dcp)를 다운로드합니다
3. [Universal Dreamcast Patcher](https://github.com/DerekPascarella/UniversalDreamcastPatcher)로 원본 GDI에 DCP 패치를 적용합니다

### v1.0.1 변경 사항

- 빈 세이브 첫 부팅 시 저장 파일 생성 중 발생하던 크래시 수정
- OPTION/CONTINUE 문자 스프라이트 테이블을 원본 실행 코드와 겹치지 않는 영역으로 재배치
- GDEMU 비호환 가능성이 있던 오프닝 자막 배경 텍스처 참조 제거
- 오프닝 자막 외곽선 제거

### 체크섬

#### 배포 패치 v1.0.1

**Puyo Puyo 4 (Dreamcast) KR v1.0.1.dcp**

| 알고리즘 | 해시                                                               |
| -------- | ------------------------------------------------------------------ |
| SHA-256  | `a90c4c3c995193954194920c01769397c6dde0ebfa01843db662c74ca0fb3ac4` |
| 크기     | 3,773,297 bytes                                                    |

#### 원본 ROM (GDI, 27트랙)

데이터 트랙 체크섬:

**track03.bin** (메인 데이터)

| 알고리즘 | 해시                                                               |
| -------- | ------------------------------------------------------------------ |
| MD5      | `a0fadb90f60aae1b5b5cd1d9ceffb018`                                 |
| SHA-1    | `6e5515fcc8e35e0c45083e9de9b9880d6c918420`                         |
| SHA-256  | `50f6f59f5a53a72e13bda9631d2ed86f31a1ac02907bd3e480e5d99c3fa16af9` |
| 크기     | 278,413,296 bytes                                                  |

**track27.bin** (파일 데이터)

| 알고리즘 | 해시                                                               |
| -------- | ------------------------------------------------------------------ |
| MD5      | `95694f7b0957660c165ef8b6b25fd579`                                 |
| SHA-1    | `27ee0d7ac17a917f5b0287c5d70ac7721e215ced`                         |
| SHA-256  | `fdcece61e384e865bcc1d5ee5af812b021bafb30009ebe35ba87a6b925e767ce` |
| 크기     | 205,661,232 bytes                                                  |

**track01.bin** (IP.BIN)

| 알고리즘 | 해시                                                               |
| -------- | ------------------------------------------------------------------ |
| MD5      | `6ef4f836257a40ef0d7480946d6f9bc4`                                 |
| SHA-1    | `40de748625a511e321d05f6f0feee0427a90924f`                         |
| SHA-256  | `ae8b5cad18af0670d811dffe978d0c608c52f80e46fb8249766abc21a3a5e5ff` |
| 크기     | 1,157,184 bytes                                                    |

### 패치 정보

- 한글 폰트: [Maplestory Light/Bold](https://maplestory.nexon.com/Media/Font), [BMJUA](http://font.woowahan.com/jua/)
- [패쳐 코드베이스](https://github.com/mcpads/dc-puyo-puyon-kr-patcher)

### 크레딧

- **패치 제작자**: mcpads
- **리버싱**: mcpads (with Claude Code, Codex)
- **한글 번역**: Claude Code (Opus 4.6) 및 Codex (GPT 5.4)
- **이미지 번역**: Gemini Nano Banana 2
- **QA**: mcpads
- **원작**: Sega / Compile (1999)

---

## 뿌요뿌요 DA! (드림캐스트, 베타)

드림캐스트 **뿌요뿌요 DA! (ぷよぷよDA! -featuring ELLENA System-)** 한글 번역 베타 패치입니다.

> ⚠️ **베타 배포 (v0.1.0)**: 번역·표기·그래픽과 패치 내용은 추후 변경될 수 있으며, 게임 진행 중 오류가 발생할 수 있습니다.

![뿌요뿌요 DA! 한글 메인 메뉴](/img/dc-puyo-puyo-da-main-menu.png)

![뿌요뿌요 DA! 한글 게임 화면](/img/dc-puyo-puyo-da-stage1-gameplay.png)

### 적용 방법

1. 아래 체크섬과 일치하는 일본판 원본 GDI를 준비합니다
2. [Puyo Puyo DA! (Dreamcast) KR v0.1.0.dcp](https://raw.githubusercontent.com/mcpads/puyo-puyo-kr-patch/main/Puyo%20Puyo%20DA%21%20%28Dreamcast%29%20KR%20v0.1.0.dcp)를 다운로드합니다
3. [Universal Dreamcast Patcher](https://github.com/DerekPascarella/UniversalDreamcastPatcher)로 원본 GDI에 DCP 패치를 적용합니다

### 체크섬

#### 배포 패치 v0.1.0

**Puyo Puyo DA! (Dreamcast) KR v0.1.0.dcp**

| 알고리즘 | 해시                                                               |
| -------- | ------------------------------------------------------------------ |
| SHA-256  | `5b44de72d187ba2aa789c6ce9baa0e0e1b6d6d2488d89eeb79d69599956a054a` |
| 크기     | 1,211,579 bytes                                                    |

#### 원본 ROM (GDI, 3트랙)

제품 번호 `T6601M`, 버전 `V1.003`입니다.

| 파일          | SHA-256                                                           | 크기            |
| ------------- | ----------------------------------------------------------------- | --------------- |
| `disc.gdi`    | `70b7e0c8a0d0b8554a3056c16726b85412d20f3398f2dce6cda5483265d89a3e` | 87 bytes        |
| `track01.bin` | `c61e3ee701f17e55a62444c5f22b1d2e47dc5f287d38280015b97703be3ccc77` | 1,914,528 bytes |
| `track02.raw` | `8364bc87848527f027fa6a9d13cae778c0132f3704dff6978173d92df1d71e06` | 1,735,776 bytes |
| `track03.bin` | `ac07913d7179a2d8f1df9f198dc3e6cceb0d78518402f169472453870cc6440b` | 1,185,760,800 bytes |

### 패치 정보

- 게임 내 그래픽 텍스트 한글화

### 크레딧

- **패치 제작자**: mcpads
- **리버싱**: mcpads (with Claude Code, Codex)
- **한글 번역**: Claude Code 및 Codex
- **이미지 제작 지원**: ImageGen
- **원작**: Compile / Sega (1999)

---

## 슈퍼 뿌요뿌요 2 (SNES)

SFC **슈퍼 뿌요뿌요 2 (す〜ぱ〜ぷよぷよ通, Super Puyo Puyo 2)** 한글 번역 패치입니다.

![sfc-puyo-puyo2-screenshot-1](/img/sfc-puyo-puyo2-screenshot-1.png)

![sfc-puyo-puyo2-screenshot-2](/img/sfc-puyo-puyo2-screenshot-2.png)

### 적용 방법

1. **일본판 원본 ROM** (`Super Puyo Puyo Tsuu (Japan).sfc`, 헤더 없는 LoROM, 2MB)을 준비합니다
2. [Super Puyo Puyo 2 (SNES) KR v1.1.0.bps](https://raw.githubusercontent.com/mcpads/puyo-puyo-kr-patch/main/Super%20Puyo%20Puyo%202%20(SNES)%20KR%20v1.1.0.bps)를 다운로드합니다
3. [Floating IPS (Flips)](https://github.com/Alcaro/Flips) 등 BPS 패처로 원본 ROM에 적용합니다

### v1.1.0 변경 사항

- 메뉴·게임 설명과 게임·엔딩 그래픽 추가 번역
- 대사창 넘침과 진엔딩 표시 오류 수정

### 체크섬

#### 배포 패치 v1.1.0

**Super Puyo Puyo 2 (SNES) KR v1.1.0.bps**

| 알고리즘 | 해시                                                               |
| -------- | ------------------------------------------------------------------ |
| SHA-256  | `2969595b9d7505078c0af98b6c1fed0b8f12e7b4514916b409d36c9f5736f3c0` |
| 크기     | 92,376 bytes                                                       |

#### 원본 ROM (SFC, 헤더 없음)

| 알고리즘 | 해시                                                               |
| -------- | ------------------------------------------------------------------ |
| MD5      | `d19486b22c8a4f11aa969671ae1967b2`                                 |
| SHA-1    | `b4004cffcc2f7d36cefbf0db89c64572a5b3ce8e`                         |
| SHA-256  | `5b7ba076d62b0221df270e3a78e2f73ef0efa4dca54354d5207c38283a9dd45c` |
| 크기     | 2,097,152 bytes                                                    |

### 패치 정보

- 한글 폰트: Galmuri11, BMJUA, Maplestory Light/Bold, dalmoori
- [패처 코드베이스](https://github.com/mcpads/sfc-puyopuyo2-kr-patcher)

### 크레딧

- **패치 제작자**: mcpads
- **리버싱**: mcpads (with Codex)
- **한글 번역**: Codex
- **QA**: mcpads
- **원작**: Compile (1995)

---

## 슈퍼 나조 뿌요 1 (SNES)

SFC **슈퍼 퍼즐뿌요 1 (す～ぱ～なぞぷよ ルルーのルー, Super Nazo Puyo: Lulu no Lu)** 한글 번역 패치입니다.

참고: [슈퍼 퍼즐뿌요 - 나무위키](https://namu.wiki/w/%ED%8D%BC%EC%A6%90%EB%BF%8C%EC%9A%94%20%EC%8B%9C%EB%A6%AC%EC%A6%88#s-6)

![sfc-nazo-puyo-screenshot-1](/img/sfc-nazo-puyo-screenshot-1.png)

![sfc-nazo-puyo-screenshot-2](/img/sfc-nazo-puyo-screenshot-2.png)

![sfc-nazo-puyo-screenshot-3](/img/sfc-nazo-puyo-screenshot-3.png)

### 적용 방법

1. **일본판 원본 ROM** (`Super Nazo Puyo - Lulu no Lu (Japan).sfc`, 헤더 없는 LoROM, 1MB)을 준비합니다
2. [Super Nazo Puyo - Lulu no Lu (SNES) KR v1.0.0.bps](https://raw.githubusercontent.com/mcpads/puyo-puyo-kr-patch/main/Super%20Nazo%20Puyo%20-%20Lulu%20no%20Lu%20(SNES)%20KR%20v1.0.0.bps)를 다운로드합니다
3. [Floating IPS (Flips)](https://github.com/Alcaro/Flips) 등 BPS 패처로 원본 ROM에 적용합니다

### 체크섬

#### 배포 패치 v1.0.0

**Super Nazo Puyo - Lulu no Lu (SNES) KR v1.0.0.bps**

| 알고리즘 | 해시                                                               |
| -------- | ------------------------------------------------------------------ |
| SHA-256  | `040c4b426bcc6b37638c5c981c7219157e310ce18b33779e30f6ae2a65c936eb` |
| 크기     | 183,470 bytes                                                      |

#### 원본 ROM (SFC, 헤더 없음)

| 알고리즘 | 해시                                                               |
| -------- | ------------------------------------------------------------------ |
| MD5      | `bf4658e6ab66ec4f5388e17d63b33157`                                 |
| SHA-1    | `00b56744af9b5147ff38e72f12206ee0ea06ed67`                         |
| SHA-256  | `2c481008cffe2e0636762baf7e8a529a0246a3669be93bdce7efa8c13bdf7837` |
| 크기     | 1,048,576 bytes                                                    |

### 패치 정보

- 한글 폰트: neodgm, dalmoori
- [패쳐 코드베이스](https://github.com/mcpads/sfc-nazo-rulue1-kr-patcher)

### 크레딧

- **패치 제작자**: mcpads
- **리버싱**: mcpads (with Claude Code, Codex)
- **한글 번역**: Claude Code (Opus 4.8) 및 Codex
- **QA**: mcpads
- **원작**: Compile (1996)

---

## 슈퍼 나조 뿌요 2 (SNES)

SFC **슈퍼 퍼즐뿌요 2 (すーぱーなぞぷよ通 ルルーの鉄腕繁盛記)** 한글 번역 패치입니다.

참고: [슈퍼 퍼즐뿌요 - 나무위키](https://namu.wiki/w/%ED%8D%BC%EC%A6%90%EB%BF%8C%EC%9A%94%20%EC%8B%9C%EB%A6%AC%EC%A6%88#s-6)

![sfc-nzao-puyo2-screenshot-1](/img/sfc-nazo-puyo2-screenshot-1.png)

![sfc-nzao-puyo2-screenshot-2](/img/sfc-nazo-puyo2-screenshot-2.png)

### 적용 방법

1. **일본판 원본 ROM** (`Super Nazo Puyo Tsuu - Lulu no Tetsuwan Hanjouki (Japan).sfc`, 헤더 없는 LoROM, 1.5MB)을 준비합니다
2. [Super Nazo Puyo Tsuu - Lulu no Tetsuwan Hanjouki (SNES) KR v1.0.0.bps](https://raw.githubusercontent.com/mcpads/puyo-puyo-kr-patch/main/Super%20Nazo%20Puyo%20Tsuu%20-%20Lulu%20no%20Tetsuwan%20Hanjouki%20(SNES)%20KR%20v1.0.0.bps)를 다운로드합니다
3. [Floating IPS (Flips)](https://github.com/Alcaro/Flips) 등 BPS 패처로 원본 ROM에 적용합니다

### 체크섬

#### 배포 패치 v1.0.0

**Super Nazo Puyo Tsuu - Lulu no Tetsuwan Hanjouki (SNES) KR v1.0.0.bps**

| 알고리즘 | 해시                                                               |
| -------- | ------------------------------------------------------------------ |
| SHA-256  | `b11f1251e7efd19bb4a3d2b5429a2101a31c48912fbabc7bcb100a5066f3b332` |
| 크기     | 283,037 bytes                                                      |

#### 원본 ROM (SFC, 헤더 없음)

| 알고리즘 | 해시                                                               |
| -------- | ------------------------------------------------------------------ |
| MD5      | `68a7f453ddee511365ccbb62c25a125f`                                 |
| SHA-1    | `dc3bdace7f7587788cb72b9c3475b7c6335a5450`                         |
| SHA-256  | `1680dc92038da22f62a7c92c956b26a0356f35b34c43bb932636b1840ff43fc9` |
| 크기     | 1,572,864 bytes                                                    |

### 패치 정보

- 한글 폰트: neodgm, dalmoori, Maplestory Bold, Galmuri11/14
- [패처 코드베이스](https://github.com/mcpads/sfc-nazo-rulue2-kr-patcher)

### 크레딧

- **패치 제작자**: mcpads
- **리버싱**: mcpads (with Claude Code, Codex)
- **한글 번역**: Claude Code (Opus 4.8) 및 Codex
- **QA**: mcpads
- **원작**: Compile (1996)

---

## 번역 예정 작품

### 뿌요뿌요 BOX! (PS1)

- [x] 일본어 폰트 추출 및 테이블 완성
- [x] 시나리오 텍스트 추출
- [x] 시나리오 및 이벤트 대사 번역
- [x] 한글 폰트 통합 및 적용
- [ ] 시스템 UI
- [ ] 시스템 안정성
- [ ] 플레이 테스트 및 최종 검수

### 뿌요뿌요 2 퍼펙트 셋 (PS2)

- [x] 일본어 폰트 추출 및 테이블 완성
- [ ] 시나리오 텍스트 추출
- [ ] 시나리오 및 이벤트 대사 번역
- [ ] 한글 폰트 통합 및 적용
- [ ] 시스템 UI
- [ ] 시스템 안정성
- [ ] 플레이 테스트 및 최종 검수

---

## 이슈 제보 및 피드백

어색한 번역, 번역 오타, 심각한 그래픽 깨짐, 게임 멈춤 등의 문제는 아래 방법으로 제보해 주세요.

- **GitHub Issue**: [이슈 트래커 링크](https://github.com/mcpads/puyo-puyo-kr-patch/issues)에 새 이슈를 등록해 주세요.
- **제보 시 포함할 내용**:
  - 문제가 발생한 위치 (예: 아르르 스토리 3번째 만담)
  - 문제 현상 (예: 대사가 대사창 밖으로 넘침)
  - 사용 중인 에뮬레이터 및 버전
  - (가능하다면) 스크린샷

## 업데이트 기록

| 버전   | 날짜       | 대상                  | 내용                                                                     |
| ------ | ---------- | --------------------- | ------------------------------------------------------------------------ |
| v0.1.0 | 2026-03-28 | 뿌요뿌욘 (드림캐스트) | 베타 배포                                                                |
| v0.2.0 | 2026-03-29 | 뿌요뿌욘 (드림캐스트) | 룰 설명 번역, 오프닝 자막 2번째부터 안나오는 문제 수정, 대사 타이밍 조정 |
| v1.0.0 | 2026-04-26 | 뿌요뿌욘 (드림캐스트) | 캐릭터 포트레이트가 깨지는 버그 수정                                     |
| v0.1.0 | 2026-06-30 | 슈퍼 나조 뿌요 1 (SNES) | 베타 배포                                                              |
| v0.2.0 | 2026-07-01 | 슈퍼 나조 뿌요 1 (SNES) | 데이터 삭제/복사 확인창(예/아니오) 표시 문제 수정                      |
| v1.0.1 | 2026-07-10 | 뿌요뿌욘 (드림캐스트) | 빈 세이브 첫 부팅 크래시 수정, 오프닝 자막 배경·외곽선 제거              |
| v1.0.0 | 2026-07-11 | 슈퍼 나조 뿌요 1 (SNES) | 정식 배포      |
| v0.1.0 | 2026-07-11 | 슈퍼 나조 뿌요 2 (SNES) | 베타 배포      |
| v0.2.0 | 2026-07-12 | 슈퍼 나조 뿌요 2 (SNES) | 몇몇 버그 수정 |
| v1.0.0 | 2026-07-12 | 슈퍼 뿌요뿌요 2 (SNES) | 정식 배포      |
| v1.0.0 | 2026-07-15 | 슈퍼 나조 뿌요 2 (SNES) | 정식 배포      |
| v1.1.0 | 2026-08-09 | 슈퍼 뿌요뿌요 2 (SNES) | 추가 번역 및 표시 오류 수정 |
| v0.1.0 | 2026-08-26 | 뿌요뿌요 DA! (드림캐스트) | 베타 배포 |

## 라이선스

- 본 패치 파일은 개인적, 비상업적 용도로 제공됩니다. 원작 게임의 저작권은 해당 권리자에게 있습니다.
- 본 한글패치 파일 자체를 제작자에 허가없이 타 사이트에 재배포하지 말아 주시고, 재배포를 원하실 경우 패치원본 게시물의 링크를 공유해 주시기 바랍니다.
- 본 한글패치 파일을 이용하여 금전적 이득을 취하는 모든 행위를 일절 금합니다. 해당 행위로 발생하는 모든 책임은 이용 당사자에게 있으며, 패치 제작자는 어떠한 책임도 지지 않습니다.
