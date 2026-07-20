# Clapperboard Releases

현재 공개 버전: **Win 3.63 & Mac 3.62**

Clapperboard는 여러 촬영 파일의 오디오를 동기화하고, 무음 구간을 정리해 영상 편집 준비를 돕는 데스크톱 앱입니다.

이 저장소는 Clapperboard 설치 파일과 앱 안 업데이트 정보를 배포합니다.

## 다운로드

[Windows 3.63 다운로드](https://github.com/Clapper327/Clapperboard-Releases/releases/tag/v3.63) · [macOS 3.62 다운로드](https://github.com/Clapper327/Clapperboard-Releases/releases/tag/v3.62)

📦 **macOS 처음 설치자는 ZIP 파일을 받으세요.**

- 🪟 Windows: [`Clapperboard_Setup_3.63.exe`](https://github.com/Clapper327/Clapperboard-Releases/releases/download/v3.63/Clapperboard_Setup_3.63.exe)
- 🍎 macOS 처음 설치: [`Clapperboard_for_Mac_3.62_with_Install_Guide.zip`](https://github.com/Clapper327/Clapperboard-Releases/releases/download/v3.62/Clapperboard_for_Mac_3.62_with_Install_Guide.zip)
- 🔄 macOS 앱 안 업데이트: [`Clapperboard_for_Mac_3.62.pkg`](https://github.com/Clapper327/Clapperboard-Releases/releases/download/v3.62/Clapperboard_for_Mac_3.62.pkg)

Windows는 3.63, macOS는 3.62입니다. macOS 3.63은 다음 릴리스에서 제공됩니다.

## 주요 변경사항

### Windows 3.63

- 무음 마킹 모드에서 공통 무음 구간을 모든 트랙에 같은 색으로 표시하고, 트랙마다 컷 위치를 동일하게 맞춰 정렬을 유지합니다.
- CapCut / Final Cut 멀티캠 내보내기가 모든 트랙을 같은 시작점에 맞추도록 정렬해(마그네틱 타임라인) 카메라 간 싱크가 어긋나지 않습니다. 최대 24트랙에서 확인했습니다.
- Final Cut Pro XML 멀티캠 내보내기(카메라별 트랙, 동기화 타임라인)를 추가하고, 무음 클립을 한 색으로 구분합니다.
- 동기화 확인이 전체 트랙 파형 미리보기 창으로 바로 열립니다.

### macOS 3.62 (유지)

- macOS는 현재 3.62이며 24트랙, Synking, 전체 트랙 재생, Premiere/CapCut/Final Cut 내보내기와 실행 버튼 옆 업데이트 버튼을 포함합니다. macOS 3.63은 다음 릴리스에서 제공됩니다.

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
