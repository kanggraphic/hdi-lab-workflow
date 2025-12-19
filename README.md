# HDI Lab 아카이빙 프로젝트 워크플로우 관리 시스템

![HDI Lab](https://img.shields.io/badge/HDI_Lab-홍익대학교-0033A0?style=for-the-badge)
![Status](https://img.shields.io/badge/status-active-success?style=for-the-badge)

## 🎨 프로젝트 소개

홍익대학교 HDI Lab의 아카이빙 프로젝트를 효율적으로 관리하기 위한 워크플로우 관리 시스템입니다.

### ✨ 주요 기능

- **📋 프로세스 관리**: 6개 주요 프로세스별 작업 진행 상황 추적
- **✅ 체크박스 기능**: 작업 완료 상태 실시간 저장 및 관리
- **👥 팀 뷰**: 산업디자인/시각디자인 팀별 작업 현황 확인
- **📊 진행률 시각화**: 프로세스별 진행률 및 통계 대시보드
- **🔍 검색 & 필터**: 작업 및 담당자 검색, 필터링 기능
- **💾 자동 저장**: localStorage 기반 실시간 자동 저장

### 🎯 프로세스 구조

1. **KICK OFF** - 프로젝트 시작 및 계획 수립
2. **평가대상 연구** - 평가 대상 품목 정의 및 데이터 수집
3. **평가지표 연구** - 평가 문항 개발 및 검증
4. **평가페이지 개발** - 제품/시각 디자인 평가 시스템 구축
5. **평가 실행** - 전문가 평가 진행 및 관리
6. **보고서 작성** - 데이터 정리 및 최종 보고서 작성

## 🚀 빠른 시작

### 로컬에서 실행

```bash
# 저장소 클론
git clone https://github.com/kanggraphic/hdi-lab-workflow.git

# 디렉토리 이동
cd hdi-lab-workflow

# 브라우저로 실행
open index.html
```

### Python 웹서버로 실행

```bash
# Python 3 내장 웹서버 실행
python3 -m http.server 8000

# 브라우저에서 접속
# http://localhost:8000/index.html
```

## 🌐 배포

### GitHub Pages

1. Settings → Pages
2. Source: `claude/check-file-formats-c4DN4` 브랜치 선택
3. 배포 완료 대기 (1-2분)

### Netlify

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/kanggraphic/hdi-lab-workflow)

### Vercel

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/kanggraphic/hdi-lab-workflow)

## 🛠 기술 스택

- **Frontend**: React 18 (UMD)
- **Styling**: Tailwind CSS
- **Fonts**: Noto Sans KR
- **Storage**: localStorage API
- **Build**: Babel Standalone (JSX 변환)

## 🎨 디자인 시스템

### 컬러 팔레트

```css
--hongik-blue: #0033A0      /* 홍익대 메인 블루 */
--hongik-blue-dark: #002266  /* 홍익대 다크 블루 */
--hongik-blue-light: #3366CC /* 홍익대 라이트 블루 */
--hongik-yellow: #FFD700     /* 홍익대 골드 */
--hongik-yellow-dark: #FFC700 /* 홍익대 다크 골드 */
```

### 타이포그래피

- **Font Family**: Noto Sans KR
- **Weights**: 300 (Light) ~ 900 (Black)

## 📱 화면 구성

### 1. 클래스뷰 (카드뷰)
- 프로세스별 카드 형태 표시
- 진행률 원형 차트
- 주요 작업 미리보기

### 2. 논문포장검색 (간트차트)
- 프로세스별 타임라인 시각화
- 진행률 바 차트

### 3. 중점서범 (팀뷰)
- 팀원별 작업 현황
- 개인별 진행률 통계

## 👥 팀 구성

### 산업디자인 팀
- 홍지수 (팀장)
- 조성환, 배진형, 신성렬

### 시각디자인 팀
- 강동구 (팀장)
- 임정민, 이유안, 한수민

## 📊 프로젝트 통계

- **총 프로세스**: 6개
- **총 작업**: 85개
- **팀 구성**: 2개 팀, 8명

## 🔧 개발 가이드

### 데이터 구조

```javascript
{
  id: "001",
  title: "KICK OFF",
  color: "indigo",
  description: "프로젝트 시작 및 계획 수립",
  tasks: [
    {
      id: "001-1",
      name: "프로젝트 목표 정의",
      assignee: "홍지수",
      completed: true
    }
  ]
}
```

### localStorage 키

- `hdi-lab-project-phases`: 프로세스 및 작업 데이터

## 📝 라이선스

이 프로젝트는 홍익대학교 HDI Lab의 내부 프로젝트입니다.

## 📞 문의

- **프로젝트 관리자**: HDI Lab
- **기술 지원**: GitHub Issues

---

**Made with ❤️ by HDI Lab @ Hongik University**
