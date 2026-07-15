# Clapperboard Releases

현재 공개 버전: **Win 3.60 & Mac 3.34**

Clapperboard는 여러 촬영 파일의 오디오를 동기화하고, 무음 구간을 정리해 영상 편집 준비를 돕는 데스크톱 앱입니다.

이 저장소는 Clapperboard 설치 파일과 앱 안 업데이트 정보를 배포합니다.

## 다운로드

[Clapperboard Win 3.60 & Mac 3.34 다운로드](https://github.com/Clapper327/Clapperboard-Releases/releases/tag/v3.60)

📦 **macOS 처음 설치자는 ZIP 파일을 받으세요.**

- 🪟 Windows: [`Clapperboard_Setup_3.60.exe`](https://github.com/Clapper327/Clapperboard-Releases/releases/download/v3.60/Clapperboard_Setup_3.60.exe)
- 🍎 macOS 처음 설치: [`Clapperboard_for_Mac_3.34_with_Install_Guide.zip`](https://github.com/Clapper327/Clapperboard-Releases/releases/download/v3.34/Clapperboard_for_Mac_3.34_with_Install_Guide.zip)
- 🔄 macOS 앱 안 업데이트: [`Clapperboard_for_Mac_3.34.pkg`](https://github.com/Clapper327/Clapperboard-Releases/releases/download/v3.34/Clapperboard_for_Mac_3.34.pkg)

Windows는 현재 3.60입니다. macOS는 3.60 포팅과 패키지 검증이 끝날 때까지 공개 최신 버전을 3.34로 유지합니다.

## 주요 변경사항

- 최대 24트랙 작업 흐름을 정식 Clapperboard 기능으로 정리했습니다.
- Synking 엔진 기반 오디오 동기화를 개선해, 분할 촬영본과 부분 겹침 촬영본을 더 안정적으로 배치합니다.
- A 트랙이 비어 있어도 남은 트랙을 자동으로 승격하고 offset을 재정렬합니다.
- 파형 미리보기 재생, 플레이헤드 이동, 무음 컷 표시 갱신 흐름을 다듬었습니다.
- Premiere XML과 CapCut draft 내보내기에서 여러 트랙의 시작 위치와 공통 무음 제거 타이밍을 더 안정적으로 유지합니다.

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
