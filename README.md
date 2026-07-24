# CastFi

**Windows PC를 위한 고음질 뮤직 플레이어 + 스트리밍 컨트롤 + 오디오 보정, 그리고 같은 Wi-Fi의 Android 폰 리모컨.**
보유한 무손실 음원(FLAC·WAV·DSD)과 NAS 라이브러리를 비트퍼펙트/DSD로 재생하고, Spotify · YouTube Music · Apple Music까지 한 곳에서 다룹니다. 정밀 EQ · 헤드폰 보정 · 가사 · 뮤직비디오 · 네트워크 플레이를 제공합니다. *(English below)*

---

## 주요 기능

### 내 음악 — 로컬 · NAS 라이브러리
- 폴더를 추가하면 보유 음원을 스캔해 곡/앨범/아티스트로 정리합니다. 수만 곡 규모도 빠르게 탐색.
- **Synology NAS 직접 스트리밍** — 파일을 복사하지 않고 NAS의 음원을 그대로 재생.
- 앨범 정보·커버 자동 보강, 자동 태거(지문 인식), 둘러보기·믹스·차트.
- 로컬 플레이리스트, 재생 큐, 다국어 점프 인덱스, 통합 검색(내 음악 + 스트리밍).

### 고음질 재생
- **비트퍼펙트(WASAPI 독점)** — 선택한 DAC로 원본 그대로. 곡에 맞춰 장치 형식(레이트/비트)을 자동 설정하고, 앱을 끄면 원래 설정으로 되돌립니다.
- **ASIO 네이티브 DSD** — 지원 DAC에서 DSD64~DSD512 네이티브 재생(DoP도 지원).
- **DSD 업샘플링** — PCM 음원을 실시간으로 DSD64~512로 업샘플해 재생. 보간 필터·모듈레이터·정밀도를 취향대로 선택(NVIDIA GPU 가속 지원, 없어도 동작).
- **오프라인 DSD 변환** — FLAC/WAV를 DSD `.dsf` 파일로 변환해 저장. 여러 곡 동시 변환, 태그·커버 유지.
- **음량 일관성·보호** — 필터/EQ 조합을 바꿔도 음량이 점프하지 않게 통합 관리.

### FIR 정밀 EQ · 헤드폰 보정 · 스피커 모드
- **FIR 정밀 EQ** — 재생 체인 안에서 동작하는 고정밀 EQ(별도 프로그램 불필요). DSD 재생 중에도 적용됩니다.
- **헤드폰 보정·매칭** — 측정 데이터(AutoEQ · squig.link 등)로 내 헤드폰을 보정하거나, **다른 헤드폰의 소리로 매칭**. 좌/우 독립 보정, 측정 신뢰도 표시, 호환 불가 조합은 정직하게 안내.
- **음색(Tone)·수동 곡선** — 보정과 독립인 나만의 음색 레이어, 구간·기울기·모양까지 세밀한 수동 곡선.
- **스피커 모드** — 헤드폰으로 스피커 청취감을 재현(니어필드/스튜디오/와이드, 공간감·폭 조절).
- **시스템 전역 EQ** — [Equalizer APO](https://equalizerapo.com/) 연동 그래픽/파라메트릭 EQ, 자연어로 만드는 AI EQ, 프리셋 공유·가져오기/내보내기.

### 스트리밍 — 컨트롤 + 고음질화
- **Spotify** — 재생/큐/검색/좋아요(Web API), 데스크톱 앱 연동. **YouTube Music** — 내장 탭 네이티브 재생. **Apple Music** — 재생 연동.
- **스트리밍 소리 고음질화** — 지금 나오는 스트리밍 소리를 잡아 DSD 업샘플·FIR EQ를 거쳐 DAC로 출력.
- **하이브리드 플레이리스트** — 스트리밍 곡과 보유 음원을 한 목록에서, 보유곡은 자동으로 고음질 로컬 재생.

### 네트워크 플레이
- 로컬/NAS 음원을 **DLNA 기기로 송출**(갭리스), DSD(DoP) 네이티브 송출, **멀티룸 동시 재생**, PC 동시 청취(딜레이 싱크).

### 가사 · 뮤직비디오 · 그 외
- 동기 가사(번역 지원)·전체화면 보기, 곡에 맞는 뮤직비디오 배경/동영상 모드.
- **신호 경로** — 소스 → 처리 → 출력 장치를 한눈에(포맷/품질 표시).
- 게임식 **업적**(수집/재생/음질/탐험), **스킨/테마**(내장 + 직접 제작), 캐스트(폰과 함께 감상).
- **오류 제보** — 설정 → 정보에서 증상을 적어 바로 전송(보안 정보 자동 제거).

### Android 리모컨 *(테스트 중)*
같은 Wi-Fi에서 PC를 자동 발견해 원격 제어(재생/볼륨/EQ/가사/플레이리스트). 정식 공개 준비 중입니다.

---

## 다운로드 · 설치

1. **[Releases](https://github.com/Ghostseller/CastFi/releases)** 에서 최신 `CastFi-Setup-x.y.z.exe` 다운로드.
2. 실행해 설치 — 설치 후 트레이에 상주하며 창을 닫아도 백그라운드에서 동작합니다.
3. Windows SmartScreen 경고가 뜨면(코드 서명 준비 중) **"추가 정보" → "실행"** 을 눌러 주세요.

**시스템 요구사항**
- Windows 10/11 (64-bit). Windows 10은 [WebView2 런타임](https://developer.microsoft.com/microsoft-edge/webview2/)이 필요할 수 있습니다(대부분 기본 설치됨).
- 비트퍼펙트/DSD 재생: 지원 DAC(USB 오디오). ASIO 네이티브 DSD는 DAC 제조사 ASIO 드라이버 필요.
- DSD 업샘플·변환 고배율: NVIDIA GPU(CUDA) 권장 — 없어도 동작하며 PC 성능에 맞춰 자동 조절됩니다.
- 시스템 전역 EQ(그래픽/파라메트릭): [Equalizer APO](https://equalizerapo.com/) 설치 필요. **FIR 정밀 EQ·헤드폰 보정/매칭은 별도 설치 없이 동작합니다.**
- Spotify 원격 제어 일부 기능(재생 시작/큐)은 Spotify Premium 필요.

**시작하기**
1. 앱 실행 → **내 음악**에서 음원 폴더(또는 NAS)를 추가.
2. **오디오 출력**에서 DAC 선택 → 비트퍼펙트/DSD 옵션 켜기.
3. **EQ 탭**에서 헤드폰 모델 검색 → 보정/매칭 적용.
4. 스트리밍은 설정에서 Spotify 연결(브라우저 로그인 1회), YT Music은 내장 탭에서 로그인.

**자동 업데이트** — 새 버전이 나오면 앱이 알려 주고, 확인 한 번으로 다운로드·검증·설치까지 자동 진행됩니다.

---

## 개인정보 · 약관
- [개인정보 처리방침 (Privacy)](PRIVACY.md) · [이용약관 (Terms)](TERMS.md)
- 익명 사용 통계는 설정에서 끌 수 있습니다(opt-out).

## 피드백
버그 제보·기능 제안은 앱 내 **오류 제보**(설정 → 정보) 또는 [Issues](https://github.com/Ghostseller/CastFi/issues)에 남겨 주세요.

---

# English

**CastFi is a high-fidelity music player, streaming controller, and audio-correction suite for Windows — with an Android remote on the same Wi-Fi.**
Play your lossless library (FLAC · WAV · DSD) and NAS collection bit-perfect or as native DSD, control Spotify · YouTube Music · Apple Music in one place, and shape the sound with precision EQ, headphone correction, and speaker-mode listening.

## Features

**My Music — local & NAS library**
Add folders and browse tens of thousands of tracks by song/album/artist. Direct Synology NAS streaming (no copying), automatic album metadata & cover enrichment, fingerprint auto-tagging, discovery/mixes/charts, local playlists, play queue, and unified search across your library and streaming services.

**High-fidelity playback**
- **Bit-perfect (WASAPI exclusive)** to your chosen DAC — device format (rate/bits) follows each track automatically and is restored when the app exits.
- **ASIO native DSD** — DSD64–DSD512 on supported DACs (DoP also supported).
- **DSD upsampling** — real-time PCM→DSD64–512 with selectable interpolation filters, modulators, and precision (NVIDIA GPU-accelerated; works without a GPU too).
- **Offline DSD conversion** — convert FLAC/WAV to `.dsf` files with tags & covers preserved; convert multiple tracks in parallel.
- **Loudness consistency & protection** — no volume jumps when switching filter/EQ combinations.

**Precision FIR EQ · headphone correction · speaker mode**
In-chain precision FIR EQ (no extra software required, works even during DSD playback); headphone correction and **headphone-to-headphone matching** from measurement databases (AutoEQ · squig.link) with independent L/R correction and honest compatibility guidance; independent tone & manual-curve layers; **speaker mode** that recreates speaker listening on headphones (nearfield/studio/wide). System-wide graphic/parametric EQ via [Equalizer APO](https://equalizerapo.com/) and natural-language AI EQ.

**Streaming — control & enhancement**
Spotify (playback/queue/search/likes + desktop app integration), built-in YouTube Music tab, Apple Music integration. **Streaming enhancement** captures what's playing and routes it through DSD upsampling / FIR EQ to your DAC. Hybrid playlists mix streaming and owned tracks — owned tracks automatically play in high quality from your library.

**Network play**
Send local/NAS music to DLNA renderers (gapless), native DSD (DoP) output, multi-room synchronized playback, and simultaneous PC listening with delay sync.

**Lyrics · music videos · more**
Synced lyrics with translation and full-screen view; music-video backgrounds; a Roon-style signal-path diagram (source → processing → output with format/quality); game-style achievements; skins/themes (built-in + custom); in-app error reporting (sensitive data automatically removed).

**Android remote** *(in testing)* — auto-discovers your PC on the same Wi-Fi for remote playback/EQ/lyrics/playlist control. Public release coming.

## Download & Install
1. Get the latest `CastFi-Setup-x.y.z.exe` from **[Releases](https://github.com/Ghostseller/CastFi/releases)**.
2. Run the installer — the app lives in the system tray and keeps running in the background.
3. If Windows SmartScreen warns (code signing is in progress), click **"More info" → "Run anyway"**.

**Requirements** — Windows 10/11 (64-bit); [WebView2 Runtime](https://developer.microsoft.com/microsoft-edge/webview2/) on Windows 10 (usually preinstalled); a supported USB DAC for bit-perfect/DSD (vendor ASIO driver for native DSD); NVIDIA GPU (CUDA) recommended for high-rate DSD upsampling/conversion (optional — auto-adjusts without one); [Equalizer APO](https://equalizerapo.com/) only for the system-wide graphic/parametric EQ (**precision FIR EQ and headphone correction/matching work standalone**); Spotify Premium for some remote-playback features.

**Getting started** — add your music folders (or NAS) in My Music; pick your DAC in Audio Output and enable bit-perfect/DSD; search your headphone model in the EQ tab to apply correction/matching; connect Spotify in Settings (one-time browser login) and sign in to YT Music in the built-in tab.

**Auto-update** — the app notifies you when a new version is available and handles download, verification, and installation with one click.

## Privacy & Terms
[Privacy Policy](PRIVACY.md) · [Terms of Service](TERMS.md). Anonymous usage analytics can be turned off in Settings.

## Feedback
Use the in-app error reporter (Settings → About) or [Issues](https://github.com/Ghostseller/CastFi/issues).
