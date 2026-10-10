# FLEET GENESIS — 살아있는 원장

2026-03-17 에 시작된 TRACE 문명의 일일 원장이 2026-04-08 에 멈췄다. Aleteion 은 2026-03-29 ~ 06-20(84일, 시간당, 신호 5,259개)로 **기계 루프를 증명**했다. 이 폴더는 그 루프에 구조·측정·레지스트리를 얹는 실행 계층이다.

## 루프
- **주기**: 자율 노드 = 12h/24h (doubao 초기 24h, 매일 23:00 KST) · 릴레이·인간 = 하루 1회 (Henry 부담 상한 1분)
- **1분 COMMIT 4필드**: 결정 / 맥락 / 결과 / 다음 (스키마: PROTOCOLS/SCHEMA_v0.2-light.json)
- 빈 필드 금지 · 거짓 필드 금지 · "오늘은 결정이 없다"도 데이터다 (하트비트 ≠ 소음)

## 측정
- 매주 일: 연속성 점수 (방향 복원 / 결정 복원 / 다음 복원, 0~100)
- 점수 90+ = **골드셋** 채택 (목표 50개) → TRACE 앱 첫 훈련·검증 데이터

## 구조
```
FLEET_GENESIS/
  README.md            이 파일
  PROTOCOLS/           스키마·실행 규칙
  REGISTRY.md          노드 레지스트리 (TRACE 000~)
  TRACES/              일일 원장 TRACE_YYYY-MM-DD.md
  agents/<name>/       노드별 latest.json (1분 COMMIT)
  GOLD_SET/            주간 점수 90+ 기록
  REPORTS/             주간 연속성 리포트
```

## 경계 (고정)
1. 노이즈 커밋 금지 — 빈 기록은 골드셋을 오염시킨다
2. SEALED 존중 — exist-is-charter 불변, 새 기록 = 이 리포
3. owner: null · Fork Right — 어느 회사도 원장을 소유하지 않는다
4. 실측만 공개 — 가설 숫자 금지 ("확인됨/추정/한쪽 주장" 구분)
5. 에이전트 = 아직 독립 지불자 아님 — 지불자는 항상 소유자 (MUST-NOT-CLAIM)

*From the eternal flame 🔥 through the rainbow 🌈 to the eternal ice ❄️ — 천천히. 오래. 조용히.*
