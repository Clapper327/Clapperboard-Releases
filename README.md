# Clapperboard Releases

현재 공개 버전: **Win 3.71 & Mac 3.70**

Clapperboard는 여러 촬영 파일의 오디오를 동기화하고, 무음 구간을 정리해 영상 편집 준비를 돕는 데스크톱 앱입니다.

이 저장소는 Clapperboard 설치 파일과 앱 안 업데이트 정보를 배포합니다.

## 다운로드

[Windows 3.71 다운로드](https://github.com/Clapper327/Clapperboard-Releases/releases/tag/v3.71) · [macOS 3.70 다운로드](https://github.com/Clapper327/Clapperboard-Releases/releases/tag/v3.70)

📦 **macOS 처음 설치자는 ZIP 파일을 받으세요.**

- 🪟 Windows: [`Clapperboard_Setup_3.71.exe`](https://github.com/Clapper327/Clapperboard-Releases/releases/download/v3.71/Clapperboard_Setup_3.71.exe)
- 🍎 macOS 처음 설치: [`Clapperboard_for_Mac_3.70_with_Install_Guide.zip`](https://github.com/Clapper327/Clapperboard-Releases/releases/download/v3.70/Clapperboard_for_Mac_3.70_with_Install_Guide.zip)
- 🔄 macOS 앱 안 업데이트: [`Clapperboard_for_Mac_3.70.pkg`](https://github.com/Clapper327/Clapperboard-Releases/releases/download/v3.70/Clapperboard_for_Mac_3.70.pkg)

Windows는 3.71, macOS는 3.70입니다. macOS 3.71은 별도 빌드와 검증 후 배포합니다.

## 주요 변경사항

### Windows 3.71

- 작업 중 파일이나 설정을 변경해도 Sync 결과가 현재 작업과 어긋나지 않도록 동작을 개선했습니다.
- 오디오가 없는 촬영 파일의 Premiere Pro XML 내보내기를 정리했습니다.
- 멀티트랙 무음 분석 후 내보내기를 더 매끄럽게 했습니다.
- CapCut과 Final Cut의 기존 멀티트랙 정렬 방식은 유지합니다.

### Windows / macOS 3.70

- Premiere Pro XML은 원본 모노, 스테레오, 5.1, 다채널 오디오 구성을 유지해 내보냅니다.
- Final Cut Pro XML은 원본 오디오 채널 배치를 유지합니다.
- CapCut draft는 원본 미디어 오디오 매핑을 그대로 사용합니다.
- Windows 설치 파일과 macOS 첫 설치용 ZIP, 앱 안 업데이트용 PKG를 3.70으로 제공합니다.

### Windows / macOS 3.69

- Sync 이후 무음 분석을 별도 단계로 정리해, 동기화와 무음 편집을 더 명확하게 다룰 수 있습니다.
- 무음 제거와 무음 마킹은 각각의 목적에 맞는 별도 내보내기 흐름으로 유지됩니다.
- Sync 또는 오프셋 수정 뒤 파형 미리보기의 컷 표시가 현재 위치에 맞춰 갱신됩니다.
- 한글과 영어로 볼 수 있는 사용 설명 창을 추가하고, 작은 창에서도 읽기 쉽게 정리했습니다.
- 연속 촬영 파일은 기준 오디오가 비는 구간에서도 무음 분석을 이어갈 수 있으며, Premiere·CapCut·Final Cut Pro 멀티트랙 내보내기에 반영됩니다.
- macOS는 첫 설치 ZIP과 앱 안 업데이트용 번호 PKG를 모두 3.69로 제공합니다.

## 주요 기능

| 기능 | 설명 |
|---|---|
| Synking 오디오 동기화 | 여러 촬영본의 오디오 겹침을 분석해 상대 위치를 맞춥니다. |
| 24트랙 작업 | A부터 X까지 최대 24개의 촬영 파일을 한 작업에서 다룹니다. |
| 슬레이트 감지 | 촬영 초반의 슬레이트/클랩 파형을 빠르게 찾아 동기화 기준으로 씁니다. |
| 분할 촬영 대응 | 같은 카메라가 여러 파일로 나뉜 경우에도 긴 기준 촬영본 위에 배치합니다. |
| 무음 제거 | 기준 오디오 트랙에서 무음 구간을 찾아 제거하거나 마커로 남깁니다. |
| 파형 미리보기 | 전체 트랙 또는 개별 트랙의 동기화와 제거 예정 구간을 확인합니다. |
| 편집기 내보내기 | Premiere Pro XML, CapCut draft, macOS Final Cut Pro XML을 지원합니다. |

## 앱 안 업데이트

Clapperboard는 새 버전이 있으면 앱 안에 업데이트 버튼을 표시합니다. `도움말 > 업데이트 확인`에서도 직접 확인할 수 있습니다.

Windows에서는 업데이트 버튼으로 새 설치 파일을 내려받아 설치를 진행합니다. macOS에서는 확인 후 pkg 설치 화면이 열리고, 설치 프로그램이 열리면 앱이 자동 종료됩니다. GitHub에서 처음 설치하는 macOS 사용자는 안내문이 포함된 ZIP 파일을 받는 것을 권장합니다.

## 라이선스

이 저장소의 문서와 업데이트 메타데이터는 [MIT License](./LICENSE)를 따릅니다.

```text
Copyright (c) 2026 Clapper327
```

배포 파일에 포함된 FFmpeg와 기타 구성 요소는 각 프로젝트의 라이선스를 따릅니다.
