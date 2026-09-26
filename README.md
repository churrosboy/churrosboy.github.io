# Portfolio

순수 HTML/CSS 로 만든 원페이지 학술 포트폴리오. 빌드 도구 없이 GitHub Pages 에 그대로 배포됩니다.

## 구조
- `index.html` — 모든 섹션 (About / News / Education / Experience / Publications / Projects / Honors / Teaching)
- `assets/css/style.css` — 스타일 (라이트/다크 자동)
- `images/profile.jpg` — 프로필 사진 (현재는 `profile.svg` 플레이스홀더)
- `images/projects/`, `images/publications/` — 카드 썸네일 (이미지 또는 mp4)
- `files/cv.pdf` — CV

## 로컬 확인
```bash
python3 -m http.server 8000   # http://localhost:8000
```

## 배포 (GitHub Pages)
1. GitHub 에서 `<아이디>.github.io` 라는 이름의 public 저장소 생성
2. 아래 실행
```bash
git init && git add . && git commit -m "Initial portfolio"
git branch -M main
git remote add origin https://github.com/<아이디>/<아이디>.github.io.git
git push -u origin main
```
3. Settings → Pages → Source: `Deploy from a branch`, Branch: `main` / `/ (root)`
4. 1~2분 후 `https://<아이디>.github.io` 에서 확인
