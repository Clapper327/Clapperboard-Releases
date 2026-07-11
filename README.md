# Clapperboard Releases

현재 공개 버전: **Win 3.28 & Mac 3.30**

Clapperboard는 여러 촬영 파일의 오디오를 동기화하고, 무음 구간을 정리해 영상 편집 프로그램으로 넘길 수 있게 도와주는 데스크톱 앱입니다.

> 이 저장소는 Clapperboard 설치 파일과 앱 업데이트 정보를 배포합니다.

## 다운로드

[Clapperboard Win 3.28 & Mac 3.30 다운로드](https://github.com/Clapper327/Clapperboard-Releases/releases/tag/v3.30-mac-guide)

- Windows: `Clapperboard_Setup_3.28.exe`
- macOS 처음 설치: `Clapperboard_for_Mac_3.30_with_Install_Guide.zip`
- macOS 앱 안 업데이트: `Clapperboard_for_Mac_3.30.pkg`

Windows는 현재 3.28을 유지하며, 이번 macOS 개선사항은 추후 Windows 업데이트에 반영할 예정입니다.

## 주요 변경사항

- macOS 업데이트에서 설치 프로그램을 받기 전에 확인창을 표시하도록 개선했습니다.
- macOS 설치 프로그램이 열리면 Clapperboard for Mac이 자동 종료되어 업데이트 적용이 더 깔끔해졌습니다.
- macOS 처음 설치 사용자를 위해 한글/영문 설치 안내문이 들어 있는 ZIP 파일을 추가했습니다.
- macOS 패키지를 3.30으로 업데이트했습니다.
- Sync, Slate Detect, 무음 제거, 파형 미리보기, Premiere XML, Final Cut Pro XML, CapCut 내보내기 동작은 유지했습니다.

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

Windows에서는 업데이트 버튼으로 새 설치 파일을 받아 설치를 진행할 수 있습니다. macOS에서는 확인 후 패키지 설치 화면을 열고, 설치 프로그램이 열리면 앱이 자동 종료됩니다. GitHub에서 처음 설치하는 macOS 사용자는 안내문이 포함된 ZIP 파일을 받는 것을 권장합니다.

## 라이선스

이 저장소의 문서와 업데이트 메타데이터는 [MIT License](./LICENSE)를 따릅니다.

```text
Copyright (c) 2026 Clapper327
```

배포 파일에 포함된 FFmpeg와 기타 구성 요소는 각 프로젝트의 라이선스를 따릅니다.
