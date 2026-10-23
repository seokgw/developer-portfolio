# 석근욱 | Developer Portfolio

Java·Spring 기반 공공기관 웹 시스템의 기능 개선 경험과 개인 웹 프로젝트를 정리한 개발자용 포트폴리오입니다.

- 웹페이지: `index.html` (GitHub Pages 미게시)
- [개발 경험과 프로젝트 상세](docs/projects.md)
- [작성 근거와 검증 범위](docs/evidence.md)
- [기존 보안 인프라 포트폴리오](https://seokgw.github.io/security-portfolio/)

## 실무 경험

신라시스템에서 의왕시 통합예약시스템의 운영 단계 기능 개선과 오류 수정을 담당했습니다. Java, Spring, JSP, MariaDB, MyBatis 기반 기존 코드를 분석하여 도서관 시스템으로 이어지는 JWT 로그인 연계, 강좌 현황 연계, 추첨 로직 오류 수정을 수행했습니다. 수정 결과는 개발 서버에서 확인한 범위입니다. 업무 소스와 내부 자료는 공개하지 않습니다.

AI 도구는 코드 초안·구현 방향·오류 원인 후보 탐색에 활용했으며, 기존 코드·라이브러리·업무 조건과 대조해 검토하고 수정했습니다.

## 개인 프로젝트

| 프로젝트 | 개발 주제 | 결과물 |
| --- | --- | --- |
| 직관노트 | 인증, 경기 기록 CRUD, 사진 저장, 사용자 의견에 따른 입력 흐름 개선 | [서비스](https://jigwan-note.vercel.app/) · [소스](https://github.com/seokgw/security-portfolio/tree/main/jigwan-note) |
| 플랜두씨 다이어리 | Plan → Do → See 기록, API·데이터 모델, 현재 공개 앱의 계정별 저장 | [서비스](https://seokgw.github.io/security-portfolio/pds-diary/) · [소스](https://github.com/seokgw/security-portfolio/tree/main/pds-diary) |
| 짤·카드 스튜디오 | Canvas 합성, 이미지 다운로드, 템플릿 CRUD와 JSON 검증 | [서비스](https://seokgw.github.io/security-portfolio/meme-card-studio/) · [소스](https://github.com/seokgw/security-portfolio/tree/main/meme-card-studio) |

개인 프로젝트는 AI 협업 결과물입니다. 직관노트에서 사용자는 주제·요구사항·피드백 반영 방향과 데이터 보존 조건을 결정했고, 구현·배포·기술 검증은 AI가 수행했습니다. 플랜두씨는 사용자가 실제 기록과 개선점을 판단하고 AI가 구조·API·화면 구현을 수행했습니다. 상세 역할과 확인 범위는 프로젝트 문서에 구분했습니다.

## 저장소 범위

이 저장소에는 개발자용 소개 페이지와 프로젝트 설명을 독립적으로 관리합니다. 기존 프로젝트의 소스와 서비스 URL은 그대로 연결하며 원본 저장소를 변경하지 않습니다. 기존 보안 직무용 이력서·자기소개서는 복사하지 않았습니다.

HTML·CSS만 사용하여 빌드 없이 실행할 수 있습니다.

```powershell
python -m http.server 8000
```

`http://localhost:8000`을 열거나 `index.html`을 직접 엽니다. GitHub Pages 게시 시 `main` 브랜치의 루트 디렉터리를 사용합니다. 현재 저장소는 비공개이며 웹 호스팅은 설정하지 않았습니다.

