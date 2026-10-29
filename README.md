# chanmip-skills

구글 시트 '판매관리'의 지난주(월~일) 판매내역을 집계해 주간 매출 리포트를 만들고, 슬랙 채널에 제목 한 줄 + 스레드 본문으로 게시하는 Claude 스킬입니다.

## 설치 방법

### Claude Code (플러그인 마켓플레이스)
```
/plugin marketplace add chanmip1229/weekly-sales-report-skill
/plugin install weekly-sales-report@chanmip-skills
```

### Claude 앱 (.skill 파일)
설정 → 기능(Capabilities) → 스킬에서 `weekly-sales-report.skill`을 업로드하세요.

## 구성
```
.claude-plugin/marketplace.json
plugins/weekly-sales-report/
  .claude-plugin/plugin.json
  skills/weekly-sales-report/SKILL.md
weekly-sales-report.skill
```

## 필요한 연결
- Google Drive / Google Sheets
- Slack

대상 슬랙 채널은 실행할 때 지정합니다. 저장소에는 채널 ID가 포함되어 있지 않습니다.
