# TAU Player

**Bit-perfect hi-fi music player for Windows** with a real-time 3D particle visualizer.
Closed source — this repository hosts release binaries only.

**비트퍼펙트 하이파이 음악 플레이어** — 실시간 3D 파티클 비주얼라이저 탑재.
소스코드는 비공개이며, 이 저장소는 실행 파일만 배포합니다.

---

## Download / 다운로드

Grab **`tau-player.exe`** from the [latest release](https://github.com/Valangkro/TAU-Player/releases/latest).

[Releases](https://github.com/Valangkro/TAU-Player/releases/latest)에서 **`tau-player.exe`**를 받으세요.

- Windows 10/11 64-bit
- Portable single file — no install needed / 설치 없이 바로 실행되는 포터블 파일
- WebView2 runtime required (preinstalled on Windows 11 / Win11 기본 탑재)

## Features / 주요 기능

### Bit-perfect audio / 비트퍼펙트 재생
- Decodes **FLAC, WAV, ALAC, AAC, MP3, OGG** natively (symphonia) — bypasses the browser audio stack / 브라우저 오디오 스택 우회, 네이티브 디코딩
- Streams at each track's **native sample rate** — no resampling / 곡마다 네이티브 샘플레이트로 재생, 리샘플링 없음
- **WASAPI Exclusive mode** toggle to bypass the Windows mixer / 윈도우 믹서를 우회하는 WASAPI 단독 모드 토글

### Real-time visualization / 실시간 비주얼라이저
- **5,500-particle GPU visualizer** reacting to a 64-band FFT (kick-driven emission, scale & color modulation, bloom glow) / 64밴드 FFT로 구동되는 5,500 파티클 비주얼라이저
- **Circular spectrum ring** — 128-segment ring displaced per band / 밴드별 반경 변위 원형 스펙트럼 링
- **Vocal-reactive visuals** — classic DSP extracts vocal pitch (F0) and confidence to tint the core & photon ring / 보컬 피치(F0) 추출로 코어·광자 링 색상 반응

### Player / 플레이어
- **Synced lyrics (.lrc)** — line-level timing with syllable-by-syllable highlighting driven by the audio envelope / `.lrc` 가사 싱크 — 음절 단위 점등
- **Playlist & folder sync** — watch folders, drag & drop, auto-mirroring of outside files into the sync root / 플레이리스트·폴더 동기화, 드래그&드롭
- **Windows integration** — media keys, lock-screen "now playing" card with album art & timeline (SMTC), system tray controls / 미디어 키, 잠금화면 재생 카드, 트레이 아이콘
- **Session restore** — reopens your last queue at the exact playback position / 마지막 재생 목록·위치 자동 복원

## Notes / 참고
- Unsigned binary: SmartScreen may warn on first run → "More info → Run anyway" / 서명되지 않은 exe라 첫 실행 시 SmartScreen 경고가 뜰 수 있습니다 → "추가 정보 → 실행"
- Report issues via the [Issues](https://github.com/Valangkro/TAU-Player/issues) tab / 문제 제보는 Issues 탭으로
