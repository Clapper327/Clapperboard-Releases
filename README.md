# Clapperboard Releases

현재 Windows 버전: **3.24**

여러 카메라의 촬영 파일을 오디오와 슬레이트 파형으로 동기화하고, 무음 구간을 정리해 Premiere Pro XML, CapCut 프로젝트 또는 macOS의 Final Cut Pro XML로 내보내는 데스크톱 앱입니다.

> 이 저장소는 설치 파일과 공개 업데이트 정보만 배포합니다.

## 다운로드

[Clapperboard 3.24 Windows 릴리스](https://github.com/Clapper327/Clapperboard-Releases/releases/tag/v3.24)

설치 파일: `Clapperboard_Setup_3.24.exe`

설치 프로그램은 현재 사용자 영역의 `%LOCALAPPDATA%\Programs\Clapperboard`에 앱을 설치하고 시작 메뉴 바로가기를 만듭니다. 같은 설치 파일을 다시 실행하면 기존 설치본 위에 업데이트됩니다.

## 3.24 주요 변경사항

- `지금 업데이트` 한 번으로 다운로드, 파일 검증, 앱 종료, 무인 설치, 새 버전 재실행까지 완료합니다.
- 이미 배포된 v3.23의 업데이트 버튼도 별도 다운로드 페이지나 설치 마법사 조작 없이 v3.24로 넘어갑니다.
- SHA256과 예상 파일 크기가 모두 맞아야 설치 파일을 실행합니다.
- 다운로드 폴더에서 설치 파일을 직접 실행할 때는 일반 설치 마법사를 유지합니다.
- Windows 번들에 FFmpeg와 ffprobe `8.1.2`를 포함합니다.

## 앱 안에서 업데이트

Clapperboard는 시작할 때와 `도움말 > 업데이트 확인`을 눌렀을 때 이 저장소의 [`latest.json`](./latest.json)을 확인합니다. 새 버전이 있으면 본창 헤더에 `업데이트` 버튼이 나타납니다.

Windows에서 `지금 업데이트`를 누르면 다음 순서가 자동으로 진행됩니다.

1. GitHub Release에서 최신 설치 파일 다운로드
2. 공개 피드의 파일 크기와 SHA256 검증
3. 실행 중인 Clapperboard 종료
4. 현재 사용자 영역에 새 버전 설치
5. 설치된 새 버전 자동 실행

업데이트 파일 URL은 이 저장소의 GitHub Release 자산으로 제한됩니다.

## 주요 기능

| 기능 | 설명 |
|---|---|
| 멀티카메라 Sync | 오디오 파형, 슬레이트, Synking/GCC-PHAT와 메타데이터를 조합해 여러 촬영본의 상대 위치를 찾습니다. |
| 분할 촬영 대응 | 같은 카메라가 배터리나 발열 때문에 여러 파일로 나뉜 경우에도 긴 기준 촬영본 위에 배치합니다. |
| 약한 오디오 보정 | 작은 음성은 게인 증폭과 필터링으로 분석하고 신뢰도가 낮으면 메타데이터와 상대 시간으로 보완합니다. |
| 무음 제거 | 기준 오디오 트랙에서 무음 구간을 찾아 제거하거나 마커로 남깁니다. |
| 파형 미리보기 | 전체 트랙 또는 개별 트랙의 동기화와 제거 예정 구간을 확인합니다. |
| 편집기 내보내기 | Premiere Pro XML, CapCut 프로젝트, macOS Final Cut Pro XML을 지원합니다. |

## 파일 무결성

- 파일: `Clapperboard_Setup_3.24.exe`
- 크기: `81,178,069` bytes
- SHA256: `F6D3C5EDFFF5FB7F27223CDF8B99A7EB44D23EBCC8B5874C62059788BD20F1F5`

PowerShell에서 확인:

```powershell
Get-FileHash .\Clapperboard_Setup_3.24.exe -Algorithm SHA256
```

## Windows 보안 안내

현재 설치 파일에는 Authenticode 코드 서명이 없습니다. GitHub HTTPS와 SHA256으로 파일 무결성을 검증하지만, Windows Defender SmartScreen이 `알 수 없는 게시자` 또는 `인식할 수 없는 앱` 경고를 표시할 수 있습니다. Defender나 SmartScreen을 끄는 것은 권장하지 않습니다.

## macOS

macOS v3.24 pkg는 서명, 공증, 권한 처리와 실제 구버전 원클릭 업데이트 검증을 마친 뒤 별도로 배포합니다. 그전까지 공개 업데이트 피드의 `mac` 값은 `null`로 유지됩니다.

## 라이선스

이 저장소의 문서와 업데이트 메타데이터는 [MIT License](./LICENSE)를 따릅니다.

```text
Copyright (c) 2026 Clapper327
```

배포 파일에 포함된 FFmpeg와 기타 구성 요소는 각 프로젝트의 라이선스를 따릅니다.
