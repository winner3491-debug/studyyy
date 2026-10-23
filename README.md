# 이음 · 전국 실종 신고 데이터 시각화

GitHub Pages에 바로 올릴 수 있는 정적 웹사이트입니다. `index.html`에 CSS, JavaScript, 통계 데이터, 시·도 경계를 모두 포함했습니다. Node.js 설치나 빌드, API 키가 필요하지 않습니다. 도로 지도 배경은 OpenStreetMap에서 불러오므로 인터넷 연결이 필요합니다.

## GitHub에서 게시하기

1. GitHub에 저장소를 만듭니다. GitHub Free라면 공개 저장소(Public)를 사용합니다.
2. 이 폴더 **안의 파일들**을 저장소의 최상위에 업로드하고 커밋합니다. ZIP 파일 자체를 업로드하는 방식이 아닙니다. 최소 실행 파일은 `index.html`이며, 출처와 라이선스 파일도 함께 올려 주세요.
3. 저장소에서 **Settings → Pages**를 엽니다.
4. **Source → Deploy from a branch**, **Branch → main**, **Folder → / (root)**를 선택하고 **Save**를 누릅니다. 사용 중인 기본 브랜치 이름이 다르면 그 브랜치를 고릅니다.
5. Pages 설정에 표시되는 **Visit site**로 접속합니다. 웹사이트 주소는 일반적으로 `https://계정명.github.io/저장소명/` 형태입니다.

GitHub 공식 안내: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## 파일

- `index.html`: 실행에 필요한 코드와 데이터가 들어 있는 단일 웹페이지
- `.nojekyll`: 정적 파일을 그대로 게시하도록 하는 설정
- `SOURCES.md`: 통계별 출처, 원문 링크, 가공 내역
- `data-coverage.json`: 실제 자료 확보 범위와 확인일
- `licenses/leaflet-LICENSE.txt`: Leaflet 라이선스

## 자료 범위

- 전국 연간 실종아동등 신고 건수: 2011–2025년 확보. 2025년 54,569건.
- 지역별 내역: 2013–2024년 확보. 2025·2026년 지역별 내역은 미확보.
- 2026년은 선택 가능한 연도이며 공식 연간·중간 수치는 미확보 상태로 표시합니다.
- 기준일 당시 미해결 신고: 2024-12-31 기준, 2024년만 제공.
- 지도 표시는 지역 합계이며 개별 실종 발생 위치가 아닙니다.
- 과거 1991–1996년 그래프는 현재 화면에서 제거했습니다. 출처 문서에는 이전 작업 이력이 남아 있습니다.
- 통계가 자동 갱신되는 사이트가 아닙니다. 확인일: 2026-10-23.

## 지도와 라이브러리

- 배경 지도: © OpenStreetMap contributors — https://www.openstreetmap.org/copyright
- 타일 이용 안내: https://operations.osmfoundation.org/policies/tiles/
- 지도 라이브러리: Leaflet 1.9.4, BSD-2-Clause. 라이선스 파일 동봉.
- 시·도 경계: southkorea-maps / KOSTAT 2013 — https://github.com/southkorea/southkorea-maps

## 확인

서버 코드와 localhost 경로가 없어 GitHub Pages의 저장소 하위 주소에서도 실행됩니다. 사이트에 보이는 공식 자료 링크는 외부 출처로 연결됩니다.
