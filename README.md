# ✏️ 스터디의 시작부터 관리까지, 모두의 스터디

<img src="https://github.com/MoDooS/MoDooS_Backend/assets/88308933/65c67302-ae18-443e-aba4-57daa1c9c30e"/>

## 프로젝트 소개 📝

💡 내가 바라던 🙏 스터디의 A부터 Z까지! 모두의 스터디 ❗
<br><br>

모두의 스터디는 “스터디 모집부터 관리까지 함께하는 **통합형** 스터디 관리 서비스”로서,<br>
여러분의 모든 스터디를 **똑똑하게** 운영할 수 있게 도와드려요!😉

<br><br>

## 팀원 👨‍👨‍👧‍👧👩‍👦‍👦

|                                           Frontend                                            |                                         Frontend                                          | 
|:--------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------:|
| <img src="https://avatars.githubusercontent.com/u/87124432?v=4" width=130px alt="박지수"/> | <img src="https://avatars.githubusercontent.com/u/69382168?v=4" width=130px alt="양채연"/> | 
|                              [박지수](https://github.com/jisupark123)                               |                          [양채연](https://github.com/chaeyeon-yang)                           | 

<br><br><br>

## 💡 설명

<p align="center">

<img width="1512" alt="홈 화면" src="https://github.com/MoDooS/MoDooS_Frontend/assets/69382168/3b8a838f-a0ef-465c-aa4a-3b28bffe8921">


**모두의 스터디**는 스터디 모집부터 모집 완료된 스터디의 관리까지 담당하는 기능을 모두 한번에 제공합니다. <br>
사용자가 입력한 규칙에 맞추어 불성실한 스터디원을 자동 퇴출시키고, 동기부여를 위해 서로 피드백을 익명으로 작성하도록 합니다.  <br>
이런 방식은 사용자가 스터디에만 오로지 집중할 수 있게 도울 수 있을 뿐더러 사용자의 성장의 양분을 지속적으로 제공합니다.
</p>
<br>

## 🛠️ 사용 기술 스택

### 프론트엔드

Next.js 13.4.7 Typescript 5.1.6 tailwindcss 3.3.2 react-query 3.39.3 axios 1.4.0 Recoil 0.7.7

### 아키텍쳐

<img width="670" alt="프론트 엔드 아키텍쳐" src="https://github.com/MoDooS/MoDooS_Frontend/assets/69382168/79b4014e-0e78-4b2a-b91f-2df29db8dd5b">

### 배포

Vercel

CI/CD - Github Action

### 협업 툴

Git, Discord, Notion

<br>



<br>

## 📝 설계내용

<details>
<summary>요구사항 명세서</summary>
<div markdown="1">       

| RQ-ID   | 서비스(메뉴)  | 요구사항 명        | 요구사항 내용                                                                                        | 진행사항 | 버전명   | 우선순위 |
|---------|----------|---------------|------------------------------------------------------------------------------------------------|------|-------|------|
| RQ-0001 | 회원가입     | 회원 가입         | 회원을 등록한다.  닉네임, 학교 이메일 인증, 캠퍼스, 학과 입력.                                                         | 반영   | 0.0.1 | 1    |
| RQ-0002 | 회원가입     | 이메일 본인 인증     | 가입 시 작성한 이메일로 본인인증을 진행한다.                                                                      | 반영   | 0.0.1 | 1    |
| RQ-0003 | 로그인/로그아웃 | 로그인           | 회원이 로그인을 한다. email은 학교 이메일(@mju.ac.kr) 형식이어야 한다.                                               | 반영   | 0.0.1 | 1    |
| RQ-0004 | 로그인/로그아웃 | 로그아웃          | 회원이 로그아웃을 한다.                                                                                  | 반영   | 0.0.1 | 2    |
| RQ-0005 | 로그인/로그아웃 | 비밀번호 변경       | 이메일 본인 인증을 통해 pwd를 변경한다.                                                                       | 반영   | 0.0.1 | 2    |
| RQ-0006 | 마이페이지    | 프로필 조회        | 회원 정보(랭킹, 점수, 스터디 태그, 관심있는 스터디 개수 등)를 조회한다.                                                    | 반영   |       | 3    |
| RQ-0007 | 마이페이지    | 나에 대한 피드백     | 스터디를 진행하며 받은 모든 피드백을 모아서 보여준다.                                                                 | 반영   | 0.0.1 | 2    |
| RQ-0008 | 마이페이지    | 내 스터디         | 회원이 속한/만든 스터디를 스터디의 상태(모집중/모집마감/진행중/졸료) 별로 조회한다.                                               | 반영   | 0.0.1 | 3    |
| RQ-0009 | 마이페이지    | 관심 스터디        | 회원이 찜하기 누른 관심 스터디를 조회한다.                                                                       | 반영   | 0.0.1 | 3    |
| RQ-0010 | 마이페이지    | 스터디 요청 조회     | 스터디 참가 요청에 대한 리스트를 확인할 수 있다. 스터디 신청에 대한 수락/거절은 스터디장만 접근 가능하다.                                  | 반영   | 0.0.1 | 3    |
| RQ-0011 | 마이페이지    | 알림            | 스터디 승인 요청, 수락, 거절/ 관심 스터디 마감 임박/내 스터디 댓글/대댓글/피드백 시간 시작/피드백 시간 종료 직전 알림을 보낸다.                   | 반영   | 0.0.1 | 4    |
| RQ-0012 | 마이페이지    | 계정            | 사용자의 회원 정보(닉네임, 캠퍼스, 학과 등)를 조회하고 변경할 수 있다. 비밀번호를 재설정 할 수 있다. 회원을 탈퇴할 수 있다.                     | 반영   | 0.0.1 | 3    |
| RQ-0013 | 모집공고     | 스터디 모집        | 스터디 모집 공고를 작성할 수 있다. 모집 글 생성 시, 체크리스트, 지각/결석/out에 대한 규칙 생성을 필수로 작성해야 한다.                       | 반영   | 0.0.1 | 1    |
| RQ-0014 | 모집공고     | 스터디 공고 리스트 조회 | 스터디 카테고리별 공고 조회가 가능하다. 최신순, 인기순, 마감일순 정렬이 가능하다.                                                | 반영   | 0.0.1 | 1    |
| RQ-0015 | 모집공고     | 스터디 공고 상세 조회  | 스터디 모집 공고에 대한 상세 내용을 조회할 수 있다.                                                                 | 반영   | 0.0.1 | 1    |
| RQ-0016 | 모집공고     | 찜하기           | 스터디 모집 공고에 대해 관심 스터디로 저장할 수 있다.                                                                | 반영   | 0.0.1 | 3    |
| RQ-0017 | 모집공고     | 댓글/대댓글        | 모집 공고 조회 시 댓글과 대댓글을 작성하고 수정하고 삭제할 수 있다.                                                        | 반영   | 0.0.1 | 2    |
| RQ-0018 | 스터디 관리   | 스터디 시작        | 스터디 모집 완료 시 스터디를 시작할 수 있다. 시작 시 기존 모집 공고의 내용을 변경할 수 있다.                                        | 반영   | 0.0.1 | 1    |
| RQ-0019 | 스터디 관리   | 회차별 출석 체크     | 진행 중인 스터디에 대해 스터디 리더는 스터디원의 출석체크(출석/지각/결석)를 해야 한다. 만약, 스터디 리더가 출석체크를 완료하지 않은 경우 전체 출석으로 간주한다.  | 반영   | 0.0.1 | 1    |
| RQ-0020 | 스터디 관리   | 회차별 피드백 작성    | 진행 중인 스터디에 대해 출석(혹은 지각)한 스터디원은 출석한 다른 스터디원들에 대해 피드백(체크리스트 수행 여부, 키워드 피드백 등) 작성을 시간 내에 진행한다.    | 반영   | 0.0.1 | 1    |
| RQ-0021 | 스터디 관리   | 회차별 출석 확인     | 진행 중인 스터디에 대해 모든 스터디원들의 지난 주차까지의 출석현황, out 수 등을 확인할 수 있다.                                      | 반영   | 0.0.1 | 1    |
| RQ-0022 | 스터디 관리   | 회차별 피드백 확인    | 진행 중인 스터디에 대해 지난 주차 자신이 받은 피드백을 확인할 수 있다.                                                      | 반영   | 0.0.1 | 1    |
| RQ-0023 | 스터디 관리   | 규칙 위반 회원 퇴출   | 진행 중인 스터디에 대해 정해진 out 수 제한을 넘은 회원은 자동으로 퇴출된다.                                                  | 반영   | 0.0.1 | 1    |
| RQ-0024 | 랭킹       | 등급            | 스터디 출석체크, 스터디 완주 여부, 피드백 평균 점수 등을 이용해 정립한 점수 기준에 따라 회원의 점수가 추가/감점된다. 이에 따른 회원별 등급(c~s+)이 부여된다. | 반영   | 0.01  | 3    |
| RQ-0025 | 랭킹       | 순위 조회         | 회원들의 점수별 랭킹을 조회한다.                                                                             | 반영   | 0.01  | 4    |

</div>
</details>

<details>
<summary>API 명세서</summary>
<div markdown="1">

[API명세서 보러가기](https://thin-shawl-994.notion.site/api-073c89f5900e496c8e0bf2c43b035cf9?pvs=4)

</div>
</details>

<details>
<summary>Git 컨벤션</summary>
<div markdown="1">    

### Git commit convention

- FEAT: 새로운 기능의 추가

- UPDATE: 있는 기능 업데이트

- FIX:버그 수정

- DOCS: 문서 수정

- STYLE: 스타일 관련 기능(코드 포맷팅, 세미콜론 누락, 코드 자체의 변경이 없는 경우)

- REFACTOR: 코드 리펙토링

- TEST: 테스트 코트, 리펙토링 테스트 코드 추가

- CHORE: 빌드 업무 수정, 패키지 매니저 수정(ex .gitignore 수정 같은 경우)

- RENAME : 파일 이동, 파일명 변경

- REMOVE : 삭제
  <br>

### 브랜치 컨벤션

기능 별로 브랜치 생성

브랜치 명 : **기능명/작업자깃허브아이디**

PR 생성 명 : **[Feat, Refactor, …] 작업 내용**

<br>

### ERD 설계도

![image](https://github.com/MoDooS/MoDooS_Backend/assets/88308933/5010d904-8e72-4ecc-ac88-d0e70329e617)

<br>

</div>
</details>

## ✅ 기능요약

- 회원가입/로그인
- 핵심 기능: **스터디 관리 기능**
- 알림 기능
- 마이페이지
    - 내 프로필
    - 내 피드백
    - 관심 스터디
    - 내 스터디
- 랭킹
- 스터디장일 경우
    - 스터디 모집 공고 등록, 수정, 삭제 / 스터디 시작 / 스터디 요청 수락, 거절 / 스터디 출석체크
- 일반 스터디원일 경우
    - 스터디 모집 공고 댓글, 대댓글 작성, 수정, 삭제 / 스터디 참여 요청 / 스터디 피드백 작성

<br>

