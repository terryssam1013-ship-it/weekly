# TERRY'S WEEKLY — weekly.terrys.kr

학생이 폰으로 내신변형문제를 풀고, 즉시 채점되며, 결과가 관리자 페이지에 실시간으로 쌓이는 사이트.

## 파일
- `index.html` 학생 페이지 (`/?s=세트id` 로 접속하면 해당 세트 바로 시작)
- `admin.html` 관리자 (`/admin`) — PIN은 `config.js`의 `adminPin`
- `config.js` Firebase 주소 + 관리자 PIN
- `sets/*.json` 문제 세트 원본 (관리자 페이지 [세트 관리]에서 등록)

## 배포
Vercel이 이 레포(main)를 자동 배포 → weekly.terrys.kr (가비아 CNAME → cname.vercel-dns.com)

## 새 세트 올리기 (매주)
1. 테리에게 "학생/과/범위" 알려주면 `sets/xxx.json` 생성
2. `/admin` → [세트 관리] → JSON 등록
3. [링크 복사] → 학생에게 카톡으로 전송

<!-- deploy: 2026-10-30 -->
