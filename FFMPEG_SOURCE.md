# FFmpeg source code / FFmpeg 소스 코드

[한국어](#한국어) · [English](#english)

## English

AI Effect Video uses the **FFmpeg** libraries (`avcodec`, `avformat`, `avutil`, `avfilter`, `avdevice`, `swscale`, `swresample` DLLs) under the **GNU LGPL version 2.1 or later**. FFmpeg is built without GPL or non-free parts, and is linked dynamically: the DLLs sit next to `effect_video.exe` under their usual names.

### Where the source is
Each [release](https://github.com/NexCreDesign/AIEffectVideo_release/releases) has an `EffectVideo-<version>-ffmpeg-source.zip`, the **exact** source used for the DLLs of that version:

| File in the zip | Contents |
|---|---|
| `ffmpeg-<version>.tar.xz` | FFmpeg, unmodified official release |
| `dav1d`, `SVT-AV1`, `libaom`, `rav1e`, `libvpx`, `libvpl`, `zlib`, `nv-codec-headers`, `AMF-headers` archives | Libraries built into the FFmpeg DLLs |
| `mingw-w64-*.tar.gz` | Windows runtime headers and libraries used by the build |
| `BUILD.txt` | SHA-256 and original download address of each archive, and the exact FFmpeg `configure` options |
| `build_ffmpeg.sh` | The build script |
| `SOURCE_README.txt` | How to rebuild |

The licenses of all these components are in the program's `licenses` folder and `THIRD_PARTY_NOTICES.html`.

### Rebuilding and replacing the DLLs
1. On Ubuntu (WSL on Windows works), put the archives in `third_party/ffmpeg-src/` and `build_ffmpeg.sh` in `scripts/ffmpeg/` of an empty folder.
2. Install the packages listed at the top of the script, then run `bash scripts/ffmpeg/build_ffmpeg.sh`.
3. The DLLs are created in `third_party/ffmpeg-lgpl/bin/`.
4. To use your DLLs, put them in the folder shown in **Help › About AI Effect Video…** in the program (for the zip edition, `%LOCALAPPDATA%\EffectVideo\ffmpeg\`). The program loads DLLs from there first, and the About window lists which DLLs are in use. You can also replace the DLLs in the program folder.

If you have a question about the source, email nexcredesign@protonmail.com.

---

## 한국어

AI Effect Video는 **FFmpeg** 라이브러리(`avcodec`, `avformat`, `avutil`, `avfilter`, `avdevice`, `swscale`, `swresample` DLL)를 **GNU LGPL 2.1 이상**으로 사용합니다. FFmpeg는 GPL·비자유(non-free) 부분 없이 빌드했고, 동적으로 연결됩니다. DLL은 원래 이름 그대로 `effect_video.exe` 옆에 있습니다.

### 소스 위치
[릴리스](https://github.com/NexCreDesign/AIEffectVideo_release/releases)마다 `EffectVideo-<버전>-ffmpeg-source.zip`이 있습니다. 그 버전의 DLL을 만든 **바로 그** 소스입니다.

| zip 안의 파일 | 내용 |
|---|---|
| `ffmpeg-<버전>.tar.xz` | FFmpeg 공식 릴리스, 수정 없음 |
| `dav1d`, `SVT-AV1`, `libaom`, `rav1e`, `libvpx`, `libvpl`, `zlib`, `nv-codec-headers`, `AMF-headers` 압축 파일 | FFmpeg DLL 안에 들어간 라이브러리 |
| `mingw-w64-*.tar.gz` | 빌드에 쓴 Windows 런타임 헤더·라이브러리 |
| `BUILD.txt` | 각 압축 파일의 SHA-256과 원래 내려받은 주소, FFmpeg `configure` 옵션 전체 |
| `build_ffmpeg.sh` | 빌드 스크립트 |
| `SOURCE_README.txt` | 다시 빌드하는 방법 |

이 구성 요소들의 라이선스는 프로그램의 `licenses` 폴더와 `THIRD_PARTY_NOTICES.html`에 있습니다.

### 다시 빌드해서 DLL 바꾸기
1. Ubuntu(Windows에서는 WSL도 됨)의 빈 폴더에 압축 파일들을 `third_party/ffmpeg-src/`에, `build_ffmpeg.sh`를 `scripts/ffmpeg/`에 넣습니다.
2. 스크립트 맨 위에 적힌 패키지를 설치하고 `bash scripts/ffmpeg/build_ffmpeg.sh`를 실행합니다.
3. DLL이 `third_party/ffmpeg-lgpl/bin/`에 만들어집니다.
4. 만든 DLL은 프로그램의 **도움말 › AI Effect Video 정보…**에 나오는 폴더(zip판은 `%LOCALAPPDATA%\EffectVideo\ffmpeg\`)에 넣으세요. 프로그램은 그 폴더의 DLL을 먼저 읽고, 정보 창에 어떤 DLL을 쓰는지 보여 줍니다. 프로그램 폴더의 DLL을 직접 바꿔도 됩니다.

소스에 관한 질문은 nexcredesign@protonmail.com으로 보내 주세요.
