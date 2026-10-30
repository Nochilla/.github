<div align="center">

# MIXIT (믹스잇)

**리뷰가 쌓일수록, 취향에 가까워지다.**

편의점 상품과 식재료 사진을 올리면 AI가 레시피를 제안하고,
직접 만들어 먹은 사람들의 후기로 나에게 맞는 조합을 추천하는 AI 기반 레시피 커뮤니티

</div>

---

## 무엇을 하는 서비스인가요

AI 레시피 생성만으로는 맛을 알 수 없습니다. **실제로 만들어 먹은 사람의 경험**이 있어야 합니다.
MIXIT은 사진 한 장으로 레시피를 만들고, 직접 먹어 본 후기를 쉽게 남기게 하고,
쌓인 저장·평가·리뷰를 바탕으로 사용자마다 다른 취향에 맞는 조합을 추천합니다.

| 단계 | 사용자가 하는 일 | 시스템이 하는 일 |
|---|---|---|
| 1 | 재료·상품 사진 업로드 | 이미지 검증, AI가 재료 후보 인식 |
| 2 | 인식된 재료 확인·수정 | 확정된 재료로 레시피 생성 (재료·순서·시간·난이도) |
| 3 | AI와 대화하며 레시피 조정 | 대화 기록과 레시피를 계정에 저장 |
| 4 | 만들어 먹고 리뷰 작성 | AI 대화 기록에서 재료·레시피를 불러와 리뷰 입력란 자동 채움 |
| 5 | 홈에서 랭킹·추천 확인 | 저장·평점·리뷰로 인기 랭킹과 개인화 추천 + 추천 이유 제공 |

## 핵심 설계 원칙

1. **AI 생성 레시피와 실제 시식 리뷰를 구분해 표시합니다.** 리뷰 없는 레시피를 검증된 것처럼 보여 주지 않습니다.
2. **AI가 인식·추출한 정보는 사용자가 확인하고 수정한 뒤에만 저장됩니다.**
3. **추천은 규칙 기반 취향 분석으로 후보를 고르고, AI는 분석과 추천 이유 설명에 씁니다.**
   리뷰가 AI 모델을 재학습시키지 않으며, MIXIT DB에 쌓인 데이터만 추천에 활용합니다.
4. **이메일 인증을 마친 회원만 핵심 기능을 씁니다.** 실명 대신 닉네임, 이메일은 공개하지 않습니다.

## 리포지토리

| 리포 | 역할 |
|---|---|
| [mixit-frontend](https://github.com/Nochilla/mixit-frontend) | React · TypeScript 모바일 중심 반응형 웹 |
| [mixit-backend](https://github.com/Nochilla/mixit-backend) | FastAPI REST API · 인증 · AI 연동 · 추천 |
| [mixit-data](https://github.com/Nochilla/mixit-data) | 재료·상품 사전 · 시드 레시피 · 추천 분석용 데이터 |
| [mixit-docs](https://github.com/Nochilla/mixit-docs) | 요구사항 · API 명세 · DB 설계 · 설계 결정 기록 |

## 기술 스택

`React` `TypeScript` `FastAPI` `PostgreSQL` `생성형 AI API` `AWS`

## 팀

5인 팀 프로젝트 · 개발 기간 2026.10.28 ~ 11.23

> 본 서비스는 학습 목적의 **비공식 프로젝트**입니다.
> AI가 제안한 레시피는 맛과 안전을 보장하지 않습니다. 알레르기 재료는 직접 확인해 주세요.

---

<details>
<summary><b>이전 프로젝트 · 놓칠라 (Nochilla)</b></summary>

<br>

**받을 수 있는 혜택, 놓치지 않게.**

성남시와 경기도의 지원 제도를 AI가 분석하고, 사용자의 조건에 맞는 혜택과 신청 서류 및 기간을 안내하는 AI 기반 웹 서비스입니다.
2026.10.28 회의에서 팀 프로젝트가 MIXIT 으로 변경되었습니다. 놓칠라 코드와 문서는 그대로 남겨 둡니다.

| 리포 | 역할 |
|---|---|
| [nochilla-frontend](https://github.com/Nochilla/nochilla-frontend) | React 모바일 반응형 웹 |
| [nochilla-backend](https://github.com/Nochilla/nochilla-backend) | REST API · 규칙 엔진 · LLM 연동 |
| [nochilla-data](https://github.com/Nochilla/nochilla-data) | 제도 원문 수집 · LLM 추출 · 검수 완료 데이터 |
| [nochilla-docs](https://github.com/Nochilla/nochilla-docs) | 요구사항 · API 명세 · 설계 결정 기록 |

당시 조직 소개·규칙·템플릿 원문은 [`archive/nochilla/`](https://github.com/Nochilla/.github/tree/main/archive/nochilla) 에 있습니다.

</details>
