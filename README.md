# notes-html

claude와 나눈 대화를 정리한 공간. HTML로 만들어진 노트들을 한 곳에서 보고 공유한다.

🔗 **[노트 허브 열기](https://eunseong.github.io/notes-html/)** ← GitHub Pages 배포 후 이 링크로 접근

---

## 구조

```
notes-html/
├── index.html       ← 메인 허브 (노트 목록, 필터, 분류)
├── notes.json       ← 노트 메타데이터 (제목, 날짜, 태그, 설명)
├── intuition-map.html
└── ...
```

## 노트 추가하는 법

**1. HTML 파일 추가**
Claude가 만들어준 HTML 파일을 이 폴더에 넣는다.

**2. `notes.json`에 항목 추가**

```json
{
  "id": "파일명-slug",
  "file": "파일명.html",
  "title": "노트 제목",
  "date": "YYYY-MM-DD",
  "category": "카테고리",
  "tags": ["태그1", "태그2"],
  "description": "이 채팅에서 무엇을 했는지 한 줄 설명",
  "meaningful": true,
  "note": "추가 메모 (선택)"
}
```

**3. 커밋 & 푸시**
```bash
git add .
git commit -m "add: 노트 제목"
git push
```

GitHub Pages가 자동으로 반영된다.

---

## GitHub Pages 설정 (최초 1회)

1. 레포 → Settings → Pages
2. Source: `Deploy from a branch`
3. Branch: `main` / `/ (root)`
4. Save

---

## 노트 목록

| 날짜 | 제목 | 카테고리 |
|------|------|----------|
| 2026-06-14 | [도망간 가치 — 나를 바꾸는 사고 지도](intuition-map.html) | 사고 / 철학 |
