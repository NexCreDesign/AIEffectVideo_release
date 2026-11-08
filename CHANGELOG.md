# Changelog / 변경 기록

## 1.0.0 — 2026-11-08

First public release: a free edition that runs from a zip, without installing. Exports carry a small watermark.

**Editing**
- Copy rectangle, polygon and ellipse regions of effect videos onto the source video, per frame range, without resizing. Set the work position and the effect position separately.
- Several effect videos at once, sync offsets and track cutting. Effect videos may differ from the source in size or frame rate.
- Blue screen transparency per object.
- Text, mosaic and clip art objects; SRT, VTT and ASS/SSA subtitles.
- Join several source videos, trim each one, reorder them, fade in and out.
- Source audio on/off, several effect audio tracks with cutting.
- Undo and redo, recent projects, temporary backup and recovery.

**Export**
- MP4 with H.264, H.265, AV1 or VP9. Uses the graphics card's encoder when available; keeps 10-bit sources in 10-bit.
- Parts without objects are copied as they are when possible: fast and with no quality loss (smart rendering is not used in the free edition, because every frame carries the watermark).

**Other**
- Korean and English; user guide (F1) works offline.
- Optional AI connection (MCP): edit by chatting with Claude Desktop and other MCP apps. See [ai-effect-video-mcp](https://github.com/NexCreDesign/ai-effect-video-mcp).

---

## 1.0.0 — 2026-11-08 (한국어)

첫 공개 버전입니다. 설치 없이 zip을 풀어 실행하는 무료판이며, 내보낸 영상에 작은 워터마크가 들어갑니다.

**편집**
- 이펙트 영상의 사각형·다각형·타원 영역을 크기 변환 없이 프레임 구간 단위로 원본에 복사. 작업 위치와 이펙트 위치를 따로 지정
- 이펙트 영상 여러 개 동시 사용, 싱크 오프셋, 트랙 자르기. 크기나 프레임레이트가 원본과 달라도 사용 가능
- 객체별 블루스크린 투명 처리
- 글자·모자이크·클립아트 객체, SRT·VTT·ASS/SSA 자막
- 원본 영상 여러 개 이어 붙이기, 각각 앞뒤 자르기, 순서 변경, 페이드 인·아웃
- 원본 오디오 켜고 끄기, 이펙트 오디오 여러 트랙과 구간 자르기
- 실행 취소·다시 실행, 최근 프로젝트, 임시 백업과 복구

**내보내기**
- H.264·H.265·AV1·VP9 MP4. 그래픽 카드 인코더를 쓸 수 있으면 사용, 10비트 원본은 10비트로 유지
- 객체가 없는 구간은 가능하면 원본을 그대로 복사해 빠르고 화질 손실이 없음 (무료판은 모든 프레임에 워터마크가 들어가므로 이 기능을 쓰지 않음)

**기타**
- 한국어·영어, 오프라인 사용 설명서(F1)
- AI 연결(MCP, 선택): Claude Desktop 등 MCP 앱과 대화로 편집. [ai-effect-video-mcp](https://github.com/NexCreDesign/ai-effect-video-mcp/blob/main/README.ko.md) 참고
