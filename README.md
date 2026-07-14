# Clapperboard Releases

현재 공개 버전: **Win 3.34 & Mac 3.31**

Clapperboard는 여러 촬영 파일의 오디오를 동기화하고, 무음 구간을 정리해 영상 편집 프로그램으로 넘길 수 있게 도와주는 데스크톱 앱입니다.

> 이 저장소는 Clapperboard 설치 파일과 앱 업데이트 정보를 배포합니다.

## 다운로드

[Clapperboard Win 3.34 & Mac 3.31 다운로드](https://github.com/Clapper327/Clapperboard-Releases/releases/tag/v3.34)

📦 **macOS 처음 설치자는 ZIP 파일을 받으세요.**

- 🪟 Windows: [`Clapperboard_Setup_3.34.exe`](https://github.com/Clapper327/Clapperboard-Releases/releases/download/v3.34/Clapperboard_Setup_3.34.exe)
- 🍎 macOS 처음 설치: [`Clapperboard_for_Mac_3.31_with_Install_Guide.zip`](https://github.com/Clapper327/Clapperboard-Releases/releases/download/v3.31-mac-guide/Clapperboard_for_Mac_3.31_with_Install_Guide.zip)
- 🔄 macOS 앱 안 업데이트: [`Clapperboard_for_Mac_3.31.pkg`](https://github.com/Clapper327/Clapperboard-Releases/releases/download/v3.31-mac-guide/Clapperboard_for_Mac_3.31.pkg)

Windows는 현재 3.34입니다. macOS는 3.31을 유지하며, 다음 macOS 패키지는 별도 배포 예정입니다.

## 주요 변경사항

- A 트랙을 비워도 남은 첫 파일을 자동으로 A로 올리고, 기존 트랙의 시간 관계를 유지합니다.
- 멀티카메라 Sync의 기준 선택과 복구 흐름을 다듬었습니다.
- 📦 macOS 처음 설치 사용자는 한글/영문 설치 안내문이 들어 있는 ZIP 파일을 받도록 안내를 유지했습니다.
- macOS 공개 패키지는 3.31을 유지합니다.

## 주요 기능

| 기능 | 설명 |
|---|---|
| 멀티카메라 Sync | 여러 촬영본의 오디오를 비교해 상대 위치를 맞춥니다. |
| 슬레이트 감지 | 촬영 초반의 박수/슬레이트 피크를 찾아 동기화 기준으로 활용합니다. |
| 분할 촬영 대응 | 같은 카메라가 여러 파일로 나뉜 경우에도 긴 기준 촬영본 위에 배치합니다. |
| 무음 제거 | 기준 오디오 트랙에서 무음 구간을 찾아 제거하거나 마커로 남깁니다. |
| 파형 미리보기 | 전체 트랙 또는 개별 트랙의 동기화와 제거 예정 구간을 확인합니다. |
| 편집기 내보내기 | Premiere Pro XML, CapCut 프로젝트, macOS Final Cut Pro XML을 지원합니다. |

## 앱 안에서 업데이트

Clapperboard는 새 버전이 있으면 앱 안에 업데이트 버튼을 표시합니다. `도움말 > 업데이트 확인`에서도 직접 확인할 수 있습니다.

Windows에서는 업데이트 버튼으로 새 설치 파일을 받아 설치를 진행할 수 있습니다. macOS에서는 확인 후 패키지 설치 화면을 열고, 설치 프로그램이 열리면 앱이 자동 종료됩니다. 📦 GitHub에서 처음 설치하는 macOS 사용자는 안내문이 포함된 ZIP 파일을 받는 것을 권장합니다.

## 라이선스

이 저장소의 문서와 업데이트 메타데이터는 [MIT License](./LICENSE)를 따릅니다.

```text
Copyright (c) 2026 Clapper327
```

배포 파일에 포함된 FFmpeg와 기타 구성 요소는 각 프로젝트의 라이선스를 따릅니다.
