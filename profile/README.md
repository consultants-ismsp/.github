# consultants-ismsp

ISMS-P 인증 컨설팅을 주제로 한 학습/실습 프로젝트 모음입니다.
가상기업 **브릿지X**(온프레미스 망분리 + 선불 충전식 머니 서비스)를 대상으로,
컨설팅 산출물 작성과 이를 보조하는 도구들을 직접 만들어 봅니다.

## 프로젝트

만든 순서대로. 세 프로젝트 모두 **Next.js 14 + TypeScript**로 스택을 통일했습니다.

| 레포 | 설명 | 스택 |
|---|---|---|
| [ismsp-interview-bot](https://github.com/consultants-ismsp/ismsp-interview-bot) | AI 인터뷰 챗봇 — 보안담당자 페르소나로 현황 인터뷰에 응답 | Next.js / TypeScript |
| [risk-assessment-platform](https://github.com/consultants-ismsp/risk-assessment-platform) | 위험평가 플랫폼 — 위험도 산정·우선순위 대시보드 | Next.js / TypeScript |
| [doc-consistency-checker](https://github.com/consultants-ismsp/doc-consistency-checker) | 문서 정합성 검사기 — 여러 산출물의 용어·수치·판정 모순을 적발 | Next.js / TypeScript |

## 공통 원칙

- **역할 분담**: 숫자·연산·논리규칙 → 코드 / 텍스트 추출·의미 비교 → LLM.
  판정(Y/N)·계산·집계는 LLM에게 시키지 않는다.
- 모든 결과에 **출처(문서·항목)** 를 붙인다.
- API 키는 서버/환경변수로만. 코드·커밋에 하드코딩 금지.
- 과한 추상화 없이, 주니어 기준의 읽기 쉬운 코드.

> 학습 목적의 비상업 프로젝트입니다. 가상기업·시나리오는 실제와 무관합니다.
