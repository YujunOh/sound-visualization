# 소리 시각화

브라우저에서 동작하는 오디오 분석기 + 함수 시각화 도구. 외부 라이브러리 없이 순수 JavaScript로 만들었다.

## 파일
- `audio-analyzer.html` — 실시간 오디오 스펙트럼 분석기
- `mouse-tracker.html` — 인터랙티브 함수 뷰어 (sin, cos, tan + 히트맵)

## 실행
아무 브라우저에서 HTML 파일을 열면 된다.

```bash
# 그냥 더블클릭하거나
start audio-analyzer.html
```

## audio-analyzer.html
- 오디오 파일(.wav, .mp3 등)을 로드해서 실시간 스펙트럼 분석
- FFT 기반 주파수 분석 + Mel 필터뱅크
- 재생 중 실시간 시각화 (Canvas API)
- 스페이스바로 재생/일시정지

## mouse-tracker.html
- 4분면에 sin, cos, tan, 히트맵을 동시에 시각화
- 마우스 좌표가 4개 패널에 동기화
- 드래그로 이동, 휠로 줌

## 기술
- HTML5 Canvas API
- Web Audio API (AudioContext, AnalyserNode)
- 외부 라이브러리 없음 (Zero-Dependency)
