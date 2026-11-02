# FOOD & AI LAB 개인 웹사이트 구축 계획

> **문서 버전:** 1.0  
> **작성 기준일:** 2026-11-02  
> **프로젝트 유형:** 대학생 개인 학술·프로젝트 포트폴리오  
> **배포 플랫폼:** Netlify  
> **사이트 주소:** https://aismartwork20213514.netlify.app

---

## 1. 프로젝트 개요

### 1.1 구축 목적

FOOD & AI LAB은 식품영양학을 기반으로 AI 기술과 연구 역량을 결합해 성장하는 개인 학술·프로젝트 포트폴리오 웹사이트이다. 대학 재학 중 수행한 과제물, AI 스마트워크 결과물, 식품영양학 관련 학습·연구 자료와 대외활동을 체계적으로 기록하고, 향후 대학원 진학 및 연구 경력에 따라 지속적으로 확장하는 것을 목표로 한다.

단순한 파일 보관소가 아니라 방문자가 소유자의 학력·관심 분야·활동과 프로젝트의 목적·수행 과정·결과를 이해할 수 있는 개인 아카이브로 구축한다.

### 1.2 브랜드

- **브랜드명:** FOOD & AI LAB
- **영문 표기:** FOOD & NUTRITION × ARTIFICIAL INTELLIGENCE
- **사이트 성격:** Academic & Research Portfolio
- **표어:** `Explore. Research. Innovate.`
- **메인 소개 문구:** 영양학적 지식과 과학적 탐구를 바탕으로 새로운 가치를 만들어갑니다.
- **이름 표기:** 김형남 / Hyungnam Kim (영문 이름 철자는 실제 사용 표기에 맞춰 최종 확인 가능)

### 1.3 핵심 방향

1. 학술적 신뢰감과 정돈된 정보 구조를 기본으로 한다.
2. AI 이미지·영상 등 창작 결과물은 시각적으로 매력 있게 전시한다.
3. 프로젝트 등록·수정·공개를 관리자 페이지에서 직접 수행할 수 있게 한다.
4. 학력·활동·관심 분야와 프로젝트 정보를 향후에도 수정·확장할 수 있게 데이터 중심으로 설계한다.
5. 공개 웹사이트와 관리자 전용 기능·정보를 명확히 분리한다.

---

## 2. 디자인 시스템

### 2.1 메인 컬러 3종

| 역할 | 색상명 | HEX | 적용 영역 |
|---|---|---|---|
| Primary | Deep Navy | `#183B56` | 로고, 주요 제목, 헤더, 주요 버튼 |
| Secondary | Botanical Green | `#54836A` | 강조 요소, 아이콘, 상태 표시, 링크 포인트 |
| Base | Warm Ivory | `#F3F1E8` | 주요 배경, 콘텐츠 영역, 카드 주변 |

본문 텍스트는 가독성을 위해 짙은 회색 계열을 보조적으로 사용하고, 테두리·구분선은 저채도 중립색을 사용한다. 위의 3색이 전체 화면의 시각적 인상을 결정하는 핵심 팔레트가 된다.

### 2.2 전체 스타일

- **디자인 비율:** Modern Academic 70% + Creative Portfolio 30%
- 넓은 여백과 명확한 제목 위계, 깔끔한 그리드 기반 레이아웃
- 연구·학술 포트폴리오에 어울리는 단정한 타이포그래피
- 프로젝트와 영상 영역에는 큰 썸네일과 이미지 중심 카드 사용
- 장식보다 정보 구조와 콘텐츠 가독성을 우선

### 2.3 반응형 디자인

- **PC:** 넓은 콘텐츠 폭, 프로젝트 3열 또는 4열 카드, 충분한 여백
- **태블릿:** 2열 카드 중심, 사이드 간격 조정
- **모바일:** 1열 콘텐츠, 햄버거 메뉴, 세로형 미디어 카드
- 프로젝트 상세·관리자 페이지도 모바일에서 주요 작업이 가능하도록 설계
- 영상은 반응형 16:9 비율로 표시하고 문서는 기기에 맞춰 미리보기 또는 다운로드 제공

### 2.4 애니메이션 및 접근성

- 콘텐츠가 화면에 들어올 때 짧고 부드러운 페이드 인
- 프로젝트 카드 hover 시 작은 확대·그림자 변화
- 페이지 전환은 짧고 자연스럽게 적용
- 과도한 패럴랙스·배경 애니메이션은 사용하지 않음
- 운영체제의 `prefers-reduced-motion` 설정을 존중해 움직임을 줄이는 모드 제공
- 키보드 탐색, 이미지 대체 텍스트, 충분한 색상 대비를 고려

---

## 3. 사이트맵 및 상단 메뉴

상단 메뉴는 사용자가 선택한 4개로 구성한다.

| 메뉴 | 영문 | 주요 내용 |
|---|---|---|
| 홈 | HOME | 브랜드 소개, 메인 문구, 연구 관심 분야 요약, 대표 프로젝트 |
| 자기소개 | ABOUT ME | 프로필, 학력 타임라인, 활동·경력, 연구 관심 분야, 비전 |
| 프로젝트 | PROJECT ARCHIVE | 4개 카테고리, 통합 검색, 프로젝트 상세 페이지 |
| 연락하기 | CONTACT | 공개 이메일 및 이메일 보내기 링크 |

활동·경력과 연구 관심 분야는 별도 상단 메뉴로 분리하지 않고 ABOUT ME 페이지에 통합한다.

### 3.1 메인 페이지 구성

1. **Header:** FOOD & AI LAB 로고, 4개 메뉴
2. **Hero:** `Explore. Research. Innovate.` / 김형남 · Hyungnam Kim / 식품영양학 및 AI 융합 지향 소개
3. **Profile Snapshot:** 전공 및 현재 학업 상태 요약
4. **Research Interests:** 관심 분야 카드 3개 요약
5. **Featured Projects:** 대표 프로젝트 최대 3개
6. **Recent Projects:** 최근 등록 프로젝트 미리보기
7. **Footer:** 이메일, 저작권 문구

프로필 사진은 추후 업로드할 수 있도록 이미지 슬롯을 확보한다. 사진이 등록되기 전에는 이름과 브랜드 그래픽으로 화면을 구성한다.

### 3.2 ABOUT ME 페이지 구성

- Profile: 이름, 전공, 소속, 간단한 소개
- Education: 학력 및 전공 이력을 연월 기준 타임라인으로 표시
- Activities & Experience: 학회, 박람회, 인턴 등을 카드로 표시
- Research Interests: 현재 탐색 중인 관심 분야 카드
- Vision: 장기 연구 목표 및 진로 비전

---

## 4. 프로필 및 학력 데이터

### 4.1 기본 프로필

- 이름: 김형남 / Hyungnam Kim
- 전공: 식품영양학과
- 소속: 한림대학교
- 복수전공: 경영학과
- 향후 진학 계획: 한림대학교 일반대학원 식품영양학과 석사과정(2027년 3월 입학 예정)

### 4.2 학력 타임라인

| 시점 | 이력 | 표시 원칙 |
|---|---|---|
| 2021.03 | 한림대학교 생명과학과 입학 | 입학 이력 |
| 2022.03 | 한림대학교 식품영양학과 전과, 경영학과 복수전공 시작 | 전과 및 복수전공 이력 |
| 2022.03–2027.02 | 식품영양학과 및 경영학과 학부 과정 | 해당 기간에는 재학 상태 표시 |
| 2027.02 | 식품영양학과·경영학과 학부 졸업 예정 시점 | 2027년 2월까지 재학/졸업 예정, 이후 졸업으로 전환 |
| 2027.03 | 한림대학교 일반대학원 식품영양학과 석사과정 입학 예정 | 2027년 2월까지 입학 예정, 2027년 3월부터 재학으로 전환 |

### 4.3 연월 자동 상태 변경 규칙

학력 상태는 사이트 방문 시점의 날짜를 기준으로 자동 계산한다. 시간대는 `Asia/Seoul`을 사용하며, 날짜의 일(day)이 아니라 **연도·월(YYYY-MM)** 단위로 비교한다.

- 시작 월 이전: `입학 예정`
- 시작 월부터 종료 월까지: `재학`
- 종료 월 다음 달부터: `졸업` 또는 사용자가 지정한 종료 상태
- 학부 학력은 2027년 2월까지 재학/졸업 예정으로 표시하고, 2027년 3월부터 졸업으로 전환한다.
- 석사과정은 2027년 2월까지 입학 예정, 2027년 3월부터 재학으로 전환한다.
- 이력의 실제 시작·종료 월은 관리자 페이지에서 수정 가능하게 한다.

### 4.4 최근 활동 및 경력 초기 데이터

| 시점 | 활동 | 표시 유형 |
|---|---|---|
| 2025.01–2025.03 | 식품 R&D 인턴 과정 | Experience |
| 2025년 | 푸드위크 참여 | Activity |
| 2026년 | 한국영양학회 참여 | Academic Activity |
| 2026년 | 푸드위크 참여 | Activity |

각 항목은 행사명, 기간, 설명, 사진, 관련 링크를 관리자 페이지에서 추가·수정할 수 있도록 구성한다. 사용자가 제공하지 않은 세부 역할이나 수상·성과는 임의로 작성하지 않는다.

### 4.5 비전 문구

> 식품영양학에 특화된 AI 모델을 개발하고, 이를 활용한 실험·연구 모델을 제공하여 AI와 영양학의 융합 분야를 선도하는 전문 연구자로 성장하고자 합니다.

문구는 ABOUT ME 페이지의 Vision 영역에 표시하며 관리자 페이지에서 수정할 수 있게 한다.

---

## 5. Research Interests 구성

현재 연구 분야가 확정된 상태가 아니므로 확정된 연구 실적이나 전공 세부 분야로 표현하지 않는다. **관심 분야·탐색 방향**임을 분명하게 표시한다.

초기 등록할 3개 카드:

1. **Molecular Nutrition** — 분자영양학 및 영양소와 대사 과정에 대한 관심
2. **Food & Functional Nutrition** — 식품 기능성 소재와 생리활성 성분에 대한 관심
3. **AI-Based Nutrition Science** — AI를 활용한 영양 데이터 분석과 연구 방법론에 대한 관심

각 카드는 제목, 설명, 대표 이미지, 키워드, 표시 순서를 갖는다. 관리자 페이지에서 추가·수정·삭제, 설명 변경, 순서 변경이 가능해야 한다.

---

## 6. PROJECT ARCHIVE 자료실

### 6.1 최종 카테고리

| 카테고리 | 포함할 내용 |
|---|---|
| AI SMART WORK | AI 활용 과제, 프롬프트, AI 이미지·영상 제작, 업무 자동화 결과물 |
| FOOD & NUTRITION | 식품영양학 전공 과제, 식품·영양 관련 실험 및 연구 자료 |
| ACADEMIC WORK | 수업 과제, 보고서, PPT, 학술 자료 등 일반 학업 결과물 |
| ETC. | 위 범주에 해당하지 않는 개인 기록 및 기타 결과물 |

광고와 비즈니스 프로젝트는 독립 카테고리로 만들지 않는다. AI를 활용해 제작한 광고 영상 등은 AI SMART WORK의 AI 콘텐츠 결과물로만 분류할 수 있다. 별도의 비즈니스 프로젝트 메뉴나 전시 분류는 만들지 않는다.

### 6.2 자료실 기능

- 프로젝트 제목·설명·태그 통합 검색
- 카테고리 필터
- 연도별 필터
- 최신순·오래된순 정렬
- 검색 결과 수 표시
- 검색 결과가 없을 때 안내 문구 표시
- 카드 보기 및 프로젝트 상세 보기

초기 규모에서는 게시된 프로젝트 데이터를 읽어 브라우저에서 제목·설명·태그·연도·카테고리를 검색하는 방식으로 구현한다. Firestore는 자체적으로 전문 검색 엔진이 아니므로 자료가 크게 늘어나면 Algolia 또는 Typesense 같은 검색 서비스를 별도 검토한다.

### 6.3 프로젝트 카드

카드에 표시할 항목:

- 대표 이미지 또는 영상 썸네일
- 프로젝트 제목
- 카테고리
- 수행 연월 또는 연도
- 짧은 요약
- 주요 태그 2~4개

### 6.4 프로젝트 상세 페이지

각 프로젝트는 독립된 상세 페이지를 갖는다.

1. 프로젝트 제목 및 대표 이미지
2. 카테고리, 수행 날짜, 과목명
3. 담당 교수 및 공동 작업자(선택 입력)
4. 프로젝트 개요와 목적
5. 수행 과정
6. 활용 도구 및 AI 도구
7. 주요 결과와 성과
8. 이미지·영상 전시
9. 프롬프트·제작 기록(해당 프로젝트에 한함)
10. 첨부 자료 미리보기 및 다운로드
11. 연관 프로젝트 또는 자료실로 돌아가기

### 6.5 대표 프로젝트 노출 규칙

- 관리자가 대표 프로젝트를 최대 3개까지 지정한다.
- 지정된 프로젝트를 메인 화면 상단에 우선 노출한다.
- 대표 지정이 3개 미만이면 최신 공개 프로젝트로 남은 자리를 채운다.
- 대표 프로젝트와 자동 노출 프로젝트가 중복되지 않도록 한다.
- 관리자 페이지에서 대표 여부와 표시 순서를 언제든 변경할 수 있다.

---

## 7. 미디어 및 파일 관리

### 7.1 파일 저장소 역할 분리

| 자료 종류 | 저장 위치 | 사이트에서의 이용 |
|---|---|---|
| 대표 이미지·썸네일·본문 이미지 | Firebase Storage | 사이트에서 직접 표시 및 확대 |
| PDF·PPT·DOCX 및 문서 원본 | Google Drive | PDF 미리보기, 가능한 경우 Drive 미리보기, 다운로드 |
| 영상 | YouTube | 반응형 내장 플레이어로 재생 |
| 원본 영상 파일(선택) | Google Drive | 다운로드 링크 제공 여부 선택 |
| 프로젝트 메타데이터 | Cloud Firestore | 검색, 필터, 상세 페이지, 공개 상태 관리 |

### 7.2 이미지

- 관리자 페이지에서 이미지 직접 업로드
- 대표 썸네일과 본문 이미지를 구분
- 업로드 시 파일 크기·확장자·MIME 타입 검사
- 썸네일용 최적화 이미지 생성 또는 리사이즈 검토
- 이미지 대체 텍스트(alt text) 입력 지원
- 프로젝트 공개 전 이미지 공개 범위 검토

### 7.3 문서

- Google Drive에 PDF·PPT·DOCX 저장
- 각 파일의 제목, 설명, Drive file ID 또는 공유 링크를 Firestore에 기록
- PDF는 브라우저 내 미리보기를 우선 제공
- PPT·DOCX는 Drive 미리보기가 정상 동작할 때 내장 미리보기를 제공하고, 호환되지 않는 환경에서는 다운로드 버튼 제공
- 공개 파일만 방문자가 접근할 수 있도록 Drive 권한을 개별 설정

**중요한 연동 조건:** Firebase의 Google 로그인은 Google Drive 파일 권한을 자동으로 부여하지 않는다. Drive API를 통한 직접 업로드를 구현하려면 별도의 Google OAuth 동의 및 최소 권한 범위 설정이 필요하다. 업로드는 Drive API의 resumable upload를 검토하고, 장기 토큰이나 비밀 정보는 브라우저 코드가 아닌 안전한 서버 측 저장소에서 관리한다.

### 7.4 영상

- 초기 버전에서는 영상을 YouTube Studio에 업로드한 뒤 일부 공개(Unlisted) URL을 관리자 페이지에 입력하는 흐름을 기본으로 한다.
- 홈페이지는 YouTube 임베드 플레이어로 재생한다.
- YouTube 영상 ID, 제목, 설명, 썸네일, 재생 위치를 프로젝트 데이터에 연결한다.
- 실제 영상 파일을 관리자 페이지에서 YouTube로 직접 업로드하는 자동화는 YouTube Data API OAuth 연동이 추가로 필요하므로 후속 기능으로 분리한다.
- 일부 공개 영상은 링크를 가진 사람이 볼 수 있으므로 민감하거나 공개하면 안 되는 영상에는 사용하지 않는다.

### 7.5 미디어 통합 표시

- 이미지 클릭 시 확대 보기(lightbox)
- 영상은 페이지 내에서 재생
- 모든 미디어는 모바일 화면에 맞춰 크기 조정
- 프로젝트별 미디어 순서 및 캡션 편집 가능

---

## 8. 관리자 페이지

### 8.1 관리자 로그인

- 로그인 방식: Google 계정 로그인
- 허용 관리자 계정: `olleh08640@gmail.com`
- 로그인 이메일은 공개 페이지나 Footer에 표시하지 않는다.
- 관리자 페이지 경로 예시: `/admin`
- 일반 방문자는 로그인 화면 또는 접근 거부 화면만 볼 수 있다.

### 8.2 권한 보안 설계

- Firebase Authentication에서 Google provider 활성화
- 허용 이메일을 서버 측 allowlist로 확인
- 관리자 역할은 서버 측에서 검증하고 필요 시 Firebase custom claim으로 부여
- Firestore 및 Storage 보안 규칙에서도 관리자만 쓰기·수정·삭제할 수 있도록 설정
- 화면에서 관리자 버튼을 숨기는 것만으로 보안을 처리하지 않는다.
- Netlify Functions에서 요청의 Firebase ID token을 검증한 뒤 민감한 Drive API 작업 수행
- 서비스 계정 키, OAuth client secret, refresh token 등 비밀 정보는 Netlify 환경변수 또는 안전한 서버 측 비밀 저장소에 보관
- `.env` 파일, 비밀 키, refresh token을 GitHub 저장소에 올리지 않는다.

### 8.3 관리자 대시보드

대시보드에서 다음 정보를 확인할 수 있도록 한다.

- 전체 프로젝트 수
- 공개 프로젝트 수
- 임시 저장 프로젝트 수
- 카테고리별 프로젝트 수
- 최근 등록·수정 프로젝트
- 대표 프로젝트 설정 현황
- 파일 업로드 및 외부 링크 상태

### 8.4 프로젝트 등록 폼(확장형)

| 구분 | 입력 항목 | 필수 여부 |
|---|---|---|
| 기본 정보 | 제목, 카테고리, 수행 날짜 | 필수 |
| 수업 정보 | 과목명, 담당 교수 | 선택 |
| 참여 정보 | 공동 작업자 | 선택 |
| 개요 | 프로젝트 목적 및 개요 | 필수 |
| 수행 내용 | 수행 과정 및 주요 단계 | 선택 또는 권장 |
| 결과 | 주요 결과 및 성과 | 권장 |
| 기술 | 사용 도구, 사용 AI 도구 | 선택 |
| 검색 | 태그 및 키워드 | 권장 |
| 이미지 | 대표 썸네일, 본문 이미지 | 선택 |
| 미디어 | YouTube URL, Drive 파일, 외부 링크 | 선택 |
| 전시 설정 | 대표 프로젝트 여부, 표시 순서 | 선택 |
| 공개 상태 | 임시 저장 / 공개 | 필수 |

담당 교수·공동 작업자 등의 항목은 공개에 적절한지 검토할 수 있도록 선택 입력으로 둔다.

### 8.5 게시 절차

1. 프로젝트 신규 작성
2. 필요한 메타데이터와 파일 첨부
3. 임시 저장(Draft)
4. 공개 화면 미리보기
5. 내용·링크·개인정보·저작권 확인
6. 공개(Published)
7. 게시 후 수정, 비공개 전환 또는 삭제

공개 상태는 `draft`, `published`, `archived` 등으로 관리한다. 초안은 일반 방문자의 검색 결과와 공개 목록에 나타나지 않아야 한다.

---

## 9. 기술 아키텍처

### 9.1 권장 기술 구성

| 영역 | 기술 | 역할 |
|---|---|---|
| Frontend | React + Vite + TypeScript | 반응형 웹 UI 및 관리자 화면 |
| Styling | CSS Modules 또는 Tailwind CSS | 디자인 시스템 및 반응형 스타일 |
| Hosting | Netlify | 정적 사이트 배포 및 호스팅 |
| Server | Netlify Functions | 인증 검증, Drive API 연동 등 서버 작업 |
| Authentication | Firebase Authentication | Google 로그인 |
| Database | Cloud Firestore | 프로젝트·활동·학력·관심 분야 정보 |
| Image Storage | Firebase Storage | 이미지 파일 저장 |
| Document Storage | Google Drive API | 문서 업로드 및 연결 |
| Video | YouTube | 영상 저장·재생 |
| Source Control | GitHub | 소스 코드 버전 관리 및 배포 연동 |

React + Vite를 기본으로 하며, 공개 페이지의 검색 노출과 메타데이터 최적화를 위해 페이지별 title·description·Open Graph·sitemap을 설정한다.

### 9.2 데이터 구조 초안

#### `projects` 컬렉션

```ts
interface Project {
  id: string;
  title: string;
  category: "AI_SMART_WORK" | "FOOD_NUTRITION" | "ACADEMIC_WORK" | "ETC";
  performedAt: string; // YYYY-MM 또는 YYYY-MM-DD
  year: number;
  courseName?: string;
  professorName?: string;
  collaborators?: string[];
  summary: string;
  objective?: string;
  process?: string;
  outcomes?: string;
  tools?: string[];
  aiTools?: string[];
  tags: string[];
  thumbnailUrl?: string;
  media?: Array<{
    type: "image" | "youtube" | "drive" | "external";
    title: string;
    url: string;
    caption?: string;
    mimeType?: string;
  }>;
  isFeatured: boolean;
  featuredOrder?: number;
  status: "draft" | "published" | "archived";
  createdAt: string;
  updatedAt: string;
  publishedAt?: string;
}
```

#### `education` 컬렉션

- institution
- department
- programType (학부·복수전공·대학원 등)
- startMonth (`YYYY-MM`)
- endMonth (`YYYY-MM`, 종료 예정이 있는 경우)
- statusLabel 및 상태 계산 기준
- sortOrder

#### `activities` 컬렉션

- title
- activityType (학회·박람회·인턴 등)
- startDate / endDate
- description
- thumbnailUrl
- externalLink
- sortOrder

#### `researchInterests` 컬렉션

- title
- description
- keywords
- imageUrl
- sortOrder
- isVisible

#### `siteSettings` 문서

- brandName
- headline
- introduction
- vision
- publicContactEmail
- featuredProjectIds
- themeColors

### 9.3 검색 구현 방식

초기에는 공개 프로젝트 목록을 가져온 뒤 브라우저에서 다음 필드를 통합 검색한다.

- 제목(title)
- 요약(summary)
- 목적(objective)
- 카테고리(category)
- 수행 연도(year)
- 태그(tags)
- 과목명(courseName)

검색과 카테고리·연도 필터, 정렬 조건을 함께 적용한다. 데이터가 커져 클라이언트 검색이 느려지면 외부 전문 검색 서비스 도입을 검토한다.

---

## 10. 개인정보·공개 범위·보안

### 10.1 Footer 공개 정보

- **공개:** 개인 연락용 이메일 주소 `rlagudska08640@naver.com`
- **비공개:** 전화번호
- **비공개:** 상세 우편 주소
- 이메일은 `mailto:` 링크로 연결한다.
- 관리자 로그인 이메일은 공개 Footer에 표시하지 않는다.
- 비공개 연락처는 공개 사이트 데이터·소스 코드·검색 메타데이터에 넣지 않는다.

### 10.2 공개형 사이트 정책

- 공개 페이지와 `published` 프로젝트만 비로그인 방문자가 열람 가능
- 초안·관리자 데이터·인증 토큰은 일반 방문자에게 노출하지 않음
- 공개 파일은 개별 공개 권한을 확인한 뒤 링크 연결
- 공동 작업자의 이름·이미지·기여 내용은 게시 권한 또는 동의를 확인
- 수업·연구 자료에 개인정보, 연구 참여자 식별 정보, 미공개 데이터, 저작권 제한 자료가 포함되지 않도록 게시 전 검토

### 10.3 보안 필수 사항

- Firestore와 Storage는 처음부터 기본 거부(deny by default) 원칙으로 구성
- 공개 프로젝트 read와 관리자 write 권한을 분리
- 관리자의 UID 또는 서버에서 발급한 관리자 권한을 규칙으로 검증
- 업로드 파일의 크기와 허용 MIME type 제한
- 비밀키를 프런트엔드 번들에 포함하지 않음
- Netlify 환경변수는 Netlify UI/CLI 등 안전한 설정 경로로 등록하고 GitHub에 커밋하지 않음
- 정기적으로 보안 규칙 및 공개 파일 권한 테스트

---

## 11. Netlify 배포 계획

### 11.1 배포 대상

- **기존/목표 사이트 주소:** https://aismartwork20213514.netlify.app
- **플랫폼:** Netlify
- **소스 저장소:** GitHub 연동 권장
- **배포 흐름:** GitHub 저장소의 지정 브랜치에 반영 → Netlify build → 배포

사용자가 제공한 주소를 배포 대상으로 기록한다. 실제 사이트의 현재 배포 상태, 저장소 연결 상태, 주소 소유 상태는 구축·연동 시 Netlify 대시보드에서 확인한다.

### 11.2 환경변수 관리

예상 환경변수 항목(실제 키 이름은 구현 시 확정):

- Firebase public config (웹 앱 공개 설정값)
- Firebase Admin SDK credential 또는 workload/서비스 인증 설정
- 관리자 이메일 allowlist
- Google Drive OAuth client ID 및 secret
- Google Drive refresh token 또는 서버 측 OAuth credential
- 기타 서버 전용 API key

서버 전용 비밀 값은 프런트엔드에서 접근할 수 없는 Netlify Functions 환경에만 둔다. Netlify 문서에서 설명하는 환경변수 범위(Builds/Functions)를 목적에 맞게 설정한다.

### 11.3 배포 운영

- `main` 브랜치: 운영 사이트
- 개발 브랜치 또는 Deploy Preview: 디자인·기능 검토
- 배포 전 build 오류 및 링크 확인
- 환경변수 변경 후 재배포 필요 여부 확인
- Netlify Functions 로그를 통해 인증·업로드 오류 확인

---

## 12. 초기 업로드 자료 검토 및 분류

현재 확인 가능한 업로드 라이브러리에서 다음 자료를 확인했다. 파일 전체를 최종 공개 대상으로 확정한 것은 아니며, 실제 공개 전 관리자 미리보기와 소유자의 승인을 거친다.

| 확인된 자료 | 제안 분류 | 초기 처리 |
|---|---|---|
| `AI스마트워크 캐릭터.png` | AI SMART WORK | AI 콘텐츠 프로젝트의 대표 이미지 또는 참고 이미지 후보 |
| `20213514_중간고사_보고서.docx` | ACADEMIC WORK 후보 | 보고서 내용을 확인한 뒤 과제 소개와 함께 게시 여부 결정 |
| `TalkFile_MT_Mate_인터넷비즈니스.docx.docx` | 공개 보류 | 비즈니스 프로젝트 카테고리를 만들지 않기로 했으므로 자동 공개하지 않음 |
| AI 이미지·영상 프롬프트 관련 자료 | AI SMART WORK 후보 | 관련 결과물과 짝지어 수동 등록 |

기존 폴더 및 라이브러리 파일을 모두 자동 게시하지 않는다. 파일명만으로 내용·저작권·공개 가능 여부를 판단하지 않고, 관리자 검토 후 개별 등록한다.

---

## 13. 구현 단계 및 완료 기준

### Phase 1. 프로젝트 기반 구축

- React + Vite + TypeScript 프로젝트 설정
- GitHub 저장소 연결
- Netlify 배포 연결 및 기본 URL 확인
- 디자인 토큰과 반응형 레이아웃 구현

**완료 기준:** PC·모바일에서 홈 화면과 메뉴가 정상 표시되고 Netlify 배포가 성공한다.

### Phase 2. 공개 페이지

- HOME, ABOUT ME, PROJECT ARCHIVE, CONTACT 페이지 제작
- 프로필·학력 타임라인 및 월별 자동 상태 변경
- 활동 카드와 Research Interests 카드
- 프로젝트 카드·상세 페이지

**완료 기준:** 각 메뉴가 연결되고 학력 상태가 지정된 연월에 맞춰 자동 변경된다.

### Phase 3. Firebase 연동 및 관리자 인증

- Firebase Authentication Google provider 설정
- 관리자 계정 allowlist 및 관리자 역할 부여
- Firestore 데이터 구조 및 보안 규칙
- Firebase Storage 업로드 및 권한 규칙

**완료 기준:** 지정한 관리자만 로그인 후 데이터와 이미지를 수정할 수 있고, 일반 방문자의 쓰기 요청은 거부된다.

### Phase 4. 프로젝트 관리 기능

- 확장형 프로젝트 등록 폼
- 임시 저장·미리보기·공개·수정·비공개·삭제
- 대표 프로젝트 지정 및 자동 보충
- 통합 검색·필터·정렬

**완료 기준:** 관리자 등록 내용이 공개 자료실과 상세 페이지에 정확히 반영되고 초안은 공개되지 않는다.

### Phase 5. 외부 자료 연동

- Google Drive OAuth 및 파일 업로드/링크 연결
- 공개 파일 권한 처리 및 문서 미리보기
- YouTube 링크 등록 및 반응형 내장 플레이어
- 미디어 확대 보기

**완료 기준:** 관리자만 파일을 연결·수정할 수 있고 공개 승인된 자료만 방문자에게 표시된다.

### Phase 6. 품질 점검 및 정식 운영

- 모바일·태블릿·PC 반응형 점검
- 키보드 탐색 및 Reduced Motion 확인
- 로그인 우회·초안 노출·파일 권한 테스트
- 이메일 링크, 검색, 다운로드, 영상 재생 테스트
- 메타데이터·사이트맵·공유 미리보기 설정

**완료 기준:** 주요 화면과 관리 기능, 공개 권한, 첨부파일, 반응형 동작이 테스트를 통과한다.

---

## 14. 운영 시나리오

### 새 과제물 등록

1. `/admin` 접속 후 Google 계정 로그인
2. `New Project` 선택
3. 제목·카테고리·날짜·목적·과정·결과·태그 입력
4. 이미지 업로드, Drive 문서 연결 또는 YouTube URL 입력
5. 임시 저장
6. 미리보기 및 공개 가능 여부 확인
7. 공개 버튼 클릭
8. 프로젝트 자료실과 검색 결과에서 노출 확인

### 학력 및 활동 수정

관리자 페이지의 Profile Management에서 학력 시작·종료 연월 또는 활동 이력을 수정한다. 학력 상태 라벨은 저장된 날짜와 현재 `Asia/Seoul` 연월을 기준으로 자동 계산한다.

### 대표 프로젝트 관리

관리자는 공개 프로젝트 중 최대 3개를 대표 프로젝트로 지정한다. 대표 프로젝트가 부족하면 최신 공개 프로젝트를 자동으로 보충한다.

---

## 15. 운영 전 준비 체크리스트

- [ ] Netlify 사이트 및 GitHub 저장소 접근 확인
- [ ] Firebase 프로젝트 생성 또는 기존 프로젝트 확인
- [ ] Google 로그인 Provider 활성화
- [ ] 지정 관리자 계정의 관리자 권한 설정
- [ ] Firestore 및 Storage 보안 규칙 배포·테스트
- [ ] Firebase Storage 버킷 및 업로드 제한 설정
- [ ] Google Drive API 활성화 및 OAuth 동의 구성
- [ ] Drive 전용 저장 폴더 구성
- [ ] YouTube 채널에서 일부 공개 업로드 방식 확인
- [ ] 프로필 사진 업로드 여부 결정
- [ ] 프로젝트별 공개 파일과 저작권 확인
- [ ] 학력·활동의 실제 정보 및 영문 이름 표기 확인
- [ ] Firebase·Netlify 요금제, 저장 용량, 전송량 및 사용량 알림 확인

---

## 16. 기술 참고 자료

아래는 구현 시 참고할 공식 문서이다. 서비스 화면과 요금·정책은 변경될 수 있으므로 실제 구축 시 최신 안내를 다시 확인한다.

- [Firebase Authentication — Google 로그인](https://firebase.google.com/docs/auth/web/google-signin)
- [Cloud Firestore Security Rules](https://firebase.google.com/docs/firestore/security/rules-conditions)
- [Firebase Security Rules 시작하기](https://firebase.google.com/docs/rules/get-started)
- [Firebase 보안 체크리스트](https://firebase.google.com/support/guides/security-checklist)
- [Google Drive API — 파일 업로드](https://developers.google.com/workspace/drive/api/guides/manage-uploads)
- [YouTube IFrame Player API](https://developers.google.com/youtube/iframe_api_reference)
- [YouTube 임베드 플레이어 매개변수](https://developers.google.com/youtube/player_parameters)
- [Netlify Functions 시작하기](https://docs.netlify.com/build/functions/get-started/)
- [Netlify 환경변수 설정](https://docs.netlify.com/build/configure-builds/environment-variables/)
- [Netlify Build 설정 및 Git 연동](https://docs.netlify.com/build/configure-builds/overview/)

---

## 17. 최종 확정 사항 요약

| 항목 | 최종 결정 |
|---|---|
| 브랜드 | FOOD & AI LAB |
| 메인 컬러 | `#183B56`, `#54836A`, `#F3F1E8` |
| 디자인 | Modern Academic 70% + Creative Portfolio 30% |
| 첫 화면 | 연구자 소개 + 대표 프로젝트 통합형 |
| 프로필 | 사진 추후 업로드, 한글·영문 이름 병행 |
| 학력·활동 | 세로형 학력 타임라인 + 활동 카드 |
| 상단 메뉴 | HOME / ABOUT ME / PROJECT ARCHIVE / CONTACT |
| 자료실 | AI SMART WORK / FOOD & NUTRITION / ACADEMIC WORK / ETC. |
| 프로젝트 상세 | 상세 설명형 |
| 미디어 | 영상 내장 재생, 이미지 확대, 프롬프트·제작 과정 표시 |
| Footer | 이메일만 공개, 전화번호·상세 주소 비공개 |
| 자료 관리 | 관리자 직접 등록 + 외부 저장소 연동 |
| 문서 저장 | Google Drive |
| 영상 저장 | YouTube |
| 이미지 저장 | Firebase Storage |
| 자료 공개 | 전체 공개(단, 임시 저장 및 비공개 자료 제외) |
| 홈페이지 언어 | 한국어 중심 + 영어 병행 |
| 배포 | Netlify |
| 사이트 주소 | `https://aismartwork20213514.netlify.app` |
| 관리자 로그인 | Google 계정 로그인 |
| 관리자 계정 | `olleh08640@gmail.com` (비공개, 권한 확인 용도) |
| 메뉴 구조 | 4개 메뉴 |
| 검색 | 제목·설명·태그·연도·카테고리 통합 검색 |
| 연구 분야 | 3개 관심 분야 카드, 관리자 수정 가능 |
| 메인 문구 | `Explore. Research. Innovate.` |
| 대표 프로젝트 | 관리자 지정 + 최신 프로젝트 자동 보충 |
| 등록 양식 | 과목·교수·공동 작업자·AI 도구·태그까지 포함하는 확장형 |
| 게시 방식 | 임시 저장 → 미리보기 → 공개 |
| 화면 대응 | PC·태블릿·모바일 반응형 |
| 애니메이션 | 부드러운 미니멀 효과 + Reduced Motion 지원 |
| 기술 스택 | React, Vite, TypeScript, Firebase, Netlify Functions |

---

**문서의 목적:** 이 계획서는 FOOD & AI LAB 웹사이트의 정보 구조·디자인·데이터·관리 기능·보안·배포 방향을 개발 착수 전에 공유하기 위한 기준 문서이다. 실제 구현 단계에서는 Netlify·Firebase·Google API 프로젝트 설정값과 저장소 권한을 별도로 구성하고, 각 항목의 완료 여부를 테스트한 뒤 정식 공개한다.
