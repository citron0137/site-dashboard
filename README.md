# site-dashboard

개인용 링크 대시보드. https://dashboard.rahoon.site

`citron0137.github.io` 에서 분리되어 나온 저장소다. 포트폴리오 사이트(rahoon.site)와 성격이 다른 개인 도구라서 따로 산다.

## 구조

정적 HTML 한 장. 빌드 없음. GitHub Pages 가 서빙한다.

- `index.html` — 대시보드 본체 (인라인 CSS/JS)
- `links.json` — 링크 목록

## 링크 수정

`links.json` 을 편집하고 커밋하면 끝. `services[]` 의 각 항목은 다음 형태다.

```json
{
  "name": "GitHub",
  "url": "https://github.com/citron0137",
  "subtitle": "github.com/citron0137",
  "icon": "https://raw.githubusercontent.com/WalkxCode/dashboard-icons/main/png/github.png",
  "location": "External"
}
```

## 검색 노출

개인 도구라서 `robots.txt` 의 `Disallow: /` 와 `index.html` 의 `noindex` 로 색인을 막는다.
