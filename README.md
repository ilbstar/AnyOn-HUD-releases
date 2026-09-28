# AnyOn HUD Free — 배포

대시보드 반사판에 비추는 안드로이드 HUD 앱 **AnyOn HUD Free**의 설치 파일과 지도 데이터를 배포하는 저장소입니다.
소스 코드는 공개하지 않습니다.

## 앱 설치

1. [Releases](../../releases)에서 최신 버전의 `AnyOnHUD-Free-<버전>.apk`를 휴대폰으로 받습니다.
2. 설치할 때 "출처를 알 수 없는 앱" 설치를 허용합니다.
3. 알림 읽기를 쓰려면 앱의 권한 › 알림 접근에서 허용합니다. 막혀 있으면 앱 정보 › ⋮ › '제한된 설정 허용' 후 다시 시도하세요.

## 주요 기능

- **내비 알림 읽기**: 구글 지도·네이버 지도·카카오내비·TMAP·Waze 길안내를 HUD로 표시
- **직접 안내**: 인터넷·유료 API 없이 휴대폰에서 목적지 검색, 경로 탐색, 턴 안내, 재탐색
- **단속카메라 알림**: 과속·구간단속 카메라

## 지도 데이터

앱의 설정 › 지도 데이터 › **받기**를 누르면 [`mapdata` 릴리스](../../releases/tag/mapdata)에서 전국 경로·검색 데이터(약 120MB)를 받습니다.
데이터는 매주 OpenStreetMap 최신 자료로 자동 갱신됩니다. Wi-Fi에서 받으세요.

| 파일 | 내용 |
|---|---|
| `manifest.json` | 데이터 버전, 파일 목록, SHA-256 |
| `korea.graph.gz` | 경로 그래프 (교차로, 도로, 회전 제한, IC/JC 이름) |
| `places.db.gz` | 장소 검색 DB (SQLite) |

## 데이터 출처와 라이선스

- 경로·검색 데이터(`korea.graph`, `places.db`)는 OpenStreetMap에서 가공한 데이터베이스로,
  **[Open Database License (ODbL) 1.0](https://opendatacommons.org/licenses/odbl/1-0/)** 로 배포합니다.
  © [OpenStreetMap contributors](https://www.openstreetmap.org/copyright)
- 지도 타일: [OpenFreeMap](https://openfreemap.org/) © OpenMapTiles, 데이터 © OpenStreetMap contributors
- 단속카메라: 경찰청 「전국무인교통단속카메라표준데이터」(공공데이터포털, 공공누리 제1유형), [No Mad Max](https://github.com/jangvis/no-mad-max-dataset) 가공

앱 실행 파일(APK)의 저작권은 제작자에게 있습니다.
