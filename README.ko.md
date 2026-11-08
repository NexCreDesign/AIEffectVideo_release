# AI Effect Video

[English](README.md)

**AI Effect Video**는 Windows용 영상 편집기입니다. 원본 영상 위에 이펙트 영상(불꽃, 폭발, 빛 등)의 원하는 부분을 크기 변환 없이 프레임 단위로 복사해 얹고, 글자·모자이크·그림을 넣어 새 영상으로 내보냅니다.

이 저장소는 프로그램을 **내려받는 곳**입니다. 프로그램의 소스 코드는 여기에 공개하지 않습니다.

## 내려받기

**[Releases 페이지](https://github.com/NexCreDesign/AIEffectVideo_release/releases/latest)**에서 최신 버전을 받으세요.

| 파일 | 내용 |
|---|---|
| `EffectVideo-<버전>.zip` | **프로그램.** 이 파일만 있으면 됩니다. |
| `EffectVideo-<버전>-ffmpeg-source.zip` | 프로그램 안에 들어 있는 FFmpeg 부분의 소스 코드입니다. 라이선스 때문에 함께 제공합니다([자세히](FFMPEG_SOURCE.md)). 프로그램을 쓰는 데는 필요 없습니다. |

## 필요한 환경

- Windows 11 (64비트). Windows 10에서도 될 수 있지만 시험하지 않았습니다.
- DirectX 11을 지원하는 그래픽 카드를 권장합니다. 없어도 동작하지만 느립니다.

## 실행 방법

1. `EffectVideo-<버전>.zip`을 내려받습니다.
2. 계속 둘 폴더에 압축을 풉니다. 예: `C:\Tools`. zip 안에 이미 `EffectVideo-<버전>` 폴더가 들어 있어서 `C:\Tools\EffectVideo-<버전>` 폴더가 만들어집니다. 설치할 것은 없습니다.
   - Windows의 **압축 풀기** 창에서 대상 폴더에 `C:\Tools`만 입력하세요. 대상 폴더가 `EffectVideo-<버전>`으로 끝나면 같은 이름의 폴더가 한 겹 더 생깁니다.
3. 그 폴더의 `effect_video.exe`를 실행합니다.
   - 파란색 **"Windows의 PC 보호"** 창이 나오면 **추가 정보** → **실행**을 누르세요. 아직 코드 서명이 없어서 나오는 창입니다.
4. 프로그램에서 **F1**을 누르면 사용 설명서가 열립니다.

프로그램을 지우려면 그 폴더를 삭제하면 됩니다. 설정과 로그는 `%APPDATA%\EffectVideo`, `%LOCALAPPDATA%\EffectVideo`에 있으니 모두 지우려면 이 폴더도 삭제하세요.

## 무료판

무료판은 모든 기능을 쓸 수 있습니다. 내보낸 영상과 프로그램의 작업영상 화면 오른쪽 아래에 작은 **"AI Effect Video Free"** 표시가 들어갑니다.

## AI로 편집하기 (선택)

Claude Desktop 같은 AI 앱을 연결하면 대화로 편집할 수 있습니다. 바뀐 내용은 편집기 화면에 바로 보이고 Ctrl+Z로 되돌릴 수 있습니다. AI 앱은 따로 설치해야 하며, 편집기에 AI 모델이 들어 있지는 않습니다.
연결 방법: **[ai-effect-video-mcp](https://github.com/NexCreDesign/ai-effect-video-mcp/blob/main/README.ko.md)**

## 내려받은 파일 확인 (선택)

릴리스마다 파일의 SHA-256 값을 적어 둡니다. PowerShell에서 아래를 실행하고 결과를 릴리스 페이지의 값과 비교하세요.

```powershell
Get-FileHash .\EffectVideo-1.0.0.zip -Algorithm SHA256
```

## 문의와 오류 신고

**nexcredesign@protonmail.com**으로 메일을 보내거나, 프로그램의 **도움말 › 문의하기**를 쓰세요. 다음을 함께 보내 주시면 도움이 됩니다.

- 버전: **도움말 › AI Effect Video 정보…**
- 무엇을 했고 어떻게 되었는지
- 로그 파일: **도움말 › 로그 저장…**으로 저장

AI 연결에 관한 질문은 [ai-effect-video-mcp Issues](https://github.com/NexCreDesign/ai-effect-video-mcp/issues)에 남기셔도 됩니다.

## 라이선스와 개인정보

- [사용권 계약](LICENSE.md): 무료로 쓸 수 있고, 프로그램을 재배포할 수는 없습니다. 오픈소스 구성 요소는 각자의 라이선스를 따릅니다.
- [개인정보처리방침](PRIVACY.md): 프로그램은 개인정보를 수집하지 않습니다.
- 오픈소스 고지: zip 안의 `THIRD_PARTY_NOTICES.html`과 `licenses` 폴더, 프로그램의 **도움말 › AI Effect Video 정보…**
- [변경 기록](CHANGELOG.md)
