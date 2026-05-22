# Sheets Backup Viewer

구글 시트 백업 뷰어 — 서식(색상·테두리·폰트·병합) 그대로 보기

## 파일 구조

```
/
├── backup-tool.html   ← 로컬에서 실행해서 JSON 추출
├── viewer.html        ← GitHub Pages에서 시트 보기
├── robots.txt         ← 검색엔진 차단
├── README.md
└── data/
    ├── 시트이름1.json
    └── 시트이름2.json
```

## 사용법

### 1. 백업 추출 (로컬)
`backup-tool.html`을 브라우저에서 열고 Google Sheets API 키 + URL 입력 → JSON 다운로드

### 2. GitHub에 올리기
다운로드한 `.json` 파일을 `data/` 폴더에 넣고 push

### 3. 뷰어 URL
```
https://[username].github.io/[repo]/viewer.html?file=data/시트이름.json
```

## GitHub Pages 설정
Settings → Pages → Branch: main / (root)
