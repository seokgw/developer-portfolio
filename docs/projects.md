# 개발 경험과 프로젝트

## 1. 공공기관 웹 시스템 운영 개발

의왕시 통합예약시스템은 구축이 완료된 서비스에 기능을 추가하고 오류를 수정해야 하는 환경이었습니다. 기존 Java·Spring·JSP·MariaDB·MyBatis 코드와 연계 방식을 확인하고 JWT 기반 도서관 로그인 연계, 강좌 현황 연계, 추첨 로직 수정을 수행했습니다.

개발 서버에서 변경한 기능의 정상 동작을 확인했습니다. 운영 적용 성과·장애 감소율·사용자 증가 수치는 확인된 근거가 없어 기재하지 않습니다. AI는 초안과 원인 후보 탐색에 활용했으며 사용자가 제안을 검토·수정했습니다. 사내 코드와 내부 구조는 공개 대상에서 제외합니다.

## 2. 직관노트

야구 직관 기록을 경기 결과·사진·후기로 남기는 개인 웹 서비스입니다. HTML·CSS·JavaScript와 Supabase Auth·PostgreSQL·Storage, Vercel을 사용합니다.

친구가 전한 로그인 부담과 반복 입력 문제를 사용자가 개선 요청으로 정리했습니다. AI가 소개 화면·로그인 없는 샘플·구장 선택·계정별 응원팀 저장을 구현했습니다. 계정별 기록 CRUD와 사진 저장 흐름을 구성했습니다.

2026-10-19 검증 기록에는 실제 계정 로그인, 응원팀 유지, 등록·수정·삭제, 사진 저장·정리, 임시 수신함의 인증 메일 1건, 390×844 뷰포트 확인이 있습니다. 이번 분리 작업에서 이 기능 검증을 다시 실행하지 않았습니다. 개선 후 친구의 재사용 평가와 실물 기기 검증은 확인되지 않았습니다.

- [서비스](https://jigwan-note.vercel.app/)
- [원본 프로젝트 설명](https://github.com/seokgw/security-portfolio/blob/main/jigwan-note/PORTFOLIO.md)
- [당시 검증 보고서](https://github.com/seokgw/security-portfolio/blob/main/jigwan-note/documents/verification-2026-10-19.md)

## 3. 플랜두씨 다이어리

실제 MCP 서버 구축 과정을 Plan → Tasks → Do → See로 연결해 기록하는 프로젝트입니다. 사용자가 계획·예상 시간·수행 기록·개선점을 판단하고 AI가 데이터 구조·API·화면·테스트 코드를 작성했습니다.

기존 서버 구현은 Node.js·Express·MariaDB이며, transaction과 SELECT FOR UPDATE, 유일 키를 통한 중복 완료 방지 구조를 포함합니다. 현재 공개 앱은 GitHub Pages 화면과 Supabase의 계정별 저장 구조입니다. 두 구현의 운영 구조를 혼동하지 않도록 원본 README를 연결합니다. 이번 작업에서는 DB 연동이나 동시성 동작을 재검증하지 않았습니다.

- [서비스](https://seokgw.github.io/security-portfolio/pds-diary/)
- [소스·구조·실행 방법](https://github.com/seokgw/security-portfolio/tree/main/pds-diary)

## 4. 짤·카드 스튜디오

브라우저에서 이미지와 문구를 합성하는 Canvas 도구입니다. 미리보기와 다운로드가 같은 렌더러를 사용하며, 1:1·4:5·9:16 비율, PNG/JPEG 출력, localStorage 템플릿 CRUD, 스키마 검증 후 JSON 가져오기를 제공합니다.

기능 설명은 원본 README 기준입니다. AI 협업 결과물로 소개하며 사용자 직접 구현 범위는 추가 확인이 필요합니다. 이번 작업에서는 이미지 출력 품질과 자동 테스트를 재실행하지 않았습니다.

- [서비스](https://seokgw.github.io/security-portfolio/meme-card-studio/)
- [소스·테스트 안내](https://github.com/seokgw/security-portfolio/tree/main/meme-card-studio)

## 5. MCP 서버 구성과 인증 연결

서비스 실행 경로와 실제 배포 경로의 불일치를 복구하고, Nginx·HTTPS·Google OAuth·PKCE 기반 인증 게이트웨이를 연결한 사례입니다. 당시 서비스 기동·health·MCP initialize·도구 목록, 미인증 401과 인증 후 초기화 200, 인증서 갱신 dry-run, 클라이언트 로그인 성공이 기록됐습니다.

사용자는 점검·복구를 요청하고 OAuth 승인에 참여했습니다. 구현·서버 설정·기술 검증은 AI 수행 범위이며, 세부 설정의 사용자 직접 수행 범위는 추가 확인이 필요합니다. 현재 운영 상태는 재검증하지 않았습니다.
