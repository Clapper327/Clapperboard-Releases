# Clapperboard

현재 버전: `3.21`

Clapperboard는 여러 카메라로 촬영한 영상을 오디오 기준으로 정렬하고, 말이 없는 구간을 찾아 편집용 XML 또는 CapCut 프로젝트로 내보내는 데스크톱 도구입니다. 촬영 현장에서 한 카메라는 길게 녹화되고 다른 카메라는 배터리나 발열 때문에 여러 조각으로 나뉘는 상황까지 염두에 두고 만들었습니다.

## 배포 상태

- Windows: `Clapperboard_Setup_3.21.exe` 배포 중
- macOS: 추후 `Clapperboard_for_Mac.pkg` 형식으로 배포 예정
- 앱 내 업데이트: Windows 설치 프로그램 기준으로 먼저 활성화됨

## 다운로드

Windows 최신 릴리스:

```text
https://github.com/Clapper327/Clapperboard-Releases/releases/tag/v3.21
```

Windows 설치 파일:

```text
Clapperboard_Setup_3.21.exe
```

설치 후 앱을 실행하면 새 버전 확인이 가능하며, 새 버전이 있을 때 상단 헤더에 `업데이트` 버튼이 표시됩니다.

## 주요 기능

| 기능 | 설명 |
|---|---|
| 멀티카메라 오디오 동기화 | 여러 촬영 파일의 파형, 슬레이트, 메타데이터를 조합해 트랙 간 시작 위치를 맞춥니다. |
| 분할 촬영본 처리 | 같은 카메라가 여러 클립으로 나뉘어도 긴 기준 촬영본 위에 상대 위치를 배치합니다. |
| 약한 오디오 보정 | 작은 대화 소리나 낮은 레벨의 오디오를 분석할 때 보조 증폭과 필터링을 적용합니다. |
| 메타데이터 보조 싱크 | 파형 신뢰도가 낮을 때 녹화 시작 시각, 파일 생성 시각, 상대 순서 등을 보조 근거로 사용합니다. |
| 무음 제거 | 기준 오디오 트랙의 무음 구간을 감지해 제거 또는 마킹할 수 있습니다. |
| 파형 미리보기 | 전체 트랙 또는 개별 트랙을 보며 제거될 구간과 남을 구간을 확인할 수 있습니다. |
| Premiere XML 내보내기 | Premiere Pro에서 열 수 있는 XML을 생성합니다. |
| CapCut 내보내기 | Windows CapCut draft 구조로 내보낼 수 있습니다. |
| Final Cut Pro XML | macOS 빌드에서는 Final Cut Pro용 FCPXML 내보내기를 지원합니다. |
| 앱 내 업데이트 | 공개 업데이트 메타데이터를 확인해 새 설치 프로그램을 다운로드하고 실행할 수 있습니다. |

## 기본 사용 흐름

1. 촬영 파일을 트랙 A, B, C 등에 불러옵니다.
2. 필요한 경우 기준 오디오 트랙과 무음 감지 설정을 조정합니다.
3. `Sync` 또는 슬레이트 감지로 동기화를 확인합니다.
4. 파형 미리보기에서 전체 트랙 또는 개별 트랙을 확인합니다.
5. 실행 후 Premiere XML, CapCut draft 등 필요한 결과물을 엽니다.

## 업데이트 방식

Clapperboard는 공개 업데이트 메타데이터를 확인해 현재 설치된 버전보다 높은 버전이 있을 때 업데이트 버튼을 보여줍니다.

업데이트 다운로드는 `Clapper327/Clapperboard-Releases`의 GitHub Release 자산으로 제한되며, 설치 파일은 SHA256 검증을 통과해야 실행됩니다.

현재 업데이트 메타데이터:

```text
https://api.github.com/repos/Clapper327/Clapperboard-Releases/contents/latest.json?ref=main
```

## Windows 설치 정보

- 설치 파일: `Clapperboard_Setup_3.21.exe`
- 설치 위치: 사용자 설치 기준 `%LOCALAPPDATA%\Programs\Clapperboard`
- 재설치/업데이트: 새 설치 파일을 실행하면 기존 설치본 위에 덮어 설치됩니다.
- 무인 설치 예시:

```bat
Clapperboard_Setup_3.21.exe /CURRENTUSER /VERYSILENT /SUPPRESSMSGBOXES /NORESTART
```

## macOS 안내

macOS 버전은 같은 Clapperboard 코드베이스에서 관리됩니다. macOS 배포판은 Finder 기반 파일 선택, macOS 경로/캐시 처리, Final Cut Pro XML 내보내기를 포함하며, 추후 `.pkg` 설치 파일로 공개 배포될 예정입니다.
