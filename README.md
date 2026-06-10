# CastFi

**같은 Wi-Fi 안의 Windows PC와 Android 폰을 잇는 음악 컨트롤 + 오디오 보정(EQ) 앱**
PC에서 재생하는 음악(Spotify · YouTube Music)을 한 곳에서 다루고, 시스템 전역 EQ · 헤드폰 보정 · 가사 · 뮤직비디오까지 제공합니다. *(English below)*

---

## 주요 기능

### 🎵 재생 컨트롤
- **Spotify** — 재생/일시정지 · 이전/다음 · 볼륨 · 시크 · 큐 · 검색 · 좋아요 (Web API 연동).
- **YouTube Music** — 앱 안에 내장된 탭으로 네이티브 재생 + 검색.
- 그 외 앱도 Windows 미디어 세션(SMTC) 기반 기본 제어.

### 📂 내 플레이리스트
- 어떤 플랫폼에서 담은 곡이든 **Spotify/YT Music으로 재생** (제목·아티스트 자동 매칭).
- 곡을 누르면 **그 곡부터 플레이리스트 재생** — 다음/이전이 플레이리스트 안에서 동작.
- **셔플 · 반복(전체/한 곡)** — 재생 중에 토글해도 즉시 반영.
- 현재 재생 중인 곡 ▶ 표시, 순서 편집 · 백업/복원.

### 🎚 시스템 EQ · 헤드폰 보정
[Equalizer APO](https://equalizerapo.com/) 위에서 동작하는 시스템 전역 EQ.
- **헤드폰 자동 보정** — AutoEQ · squig.link 측정 데이터에서 내 헤드폰 검색 → Harman 타겟 보정.
- **AI EQ** — 자연어("저음 강조, 보컬 또렷하게")로 EQ 생성.
- 그래픽/파라메트릭 EQ 편집, 프리셋 저장 · 공유, 호환 EQ 가져오기/내보내기(AutoEQ · oratory1990 등).

### 📜 가사 · 🎬 뮤직비디오
- 동기 가사(LRCLIB) + 한글 번역, 전체화면 가사 보기.
- 곡에 맞는 뮤직비디오 배경 재생.

### 📊 신호 경로
- Roon 스타일 다이어그램 — 소스 → EQ → 출력 장치, 포맷/품질 표시.

### 📱 Android 리모컨 *(테스트 중)*
같은 Wi-Fi에서 PC를 자동 발견해 원격 제어(재생/볼륨/EQ/가사/플레이리스트). 정식 공개 준비 중입니다.

---

## 다운로드 · 설치

1. **[Releases](https://github.com/Ghostseller/CastFi/releases)** 에서 최신 `CastFi-Setup-x.y.z.exe` 다운로드.
2. 실행해 설치 — 설치 후 트레이에 상주하며 창을 닫아도 백그라운드에서 동작합니다.
3. Windows SmartScreen 경고가 뜨면(코드 서명 준비 중) **"추가 정보" → "실행"** 을 눌러 주세요.

**시스템 요구사항**
- Windows 10/11 (64-bit). Windows 10은 [WebView2 런타임](https://developer.microsoft.com/microsoft-edge/webview2/)이 필요할 수 있습니다(대부분 기본 설치됨).
- EQ·헤드폰 보정 기능: [Equalizer APO](https://equalizerapo.com/) 설치 필요.
- Spotify 원격 제어 일부 기능(재생 시작/큐)은 Spotify Premium 필요.

**시작하기**
1. 앱 실행 → 설정에서 **Spotify 연결**(브라우저 로그인 1회).
2. YouTube Music은 앱 안의 YT Music 탭에서 로그인.
3. EQ 탭에서 헤드폰 모델 검색 → 자동 보정 적용.

**자동 업데이트** — 새 버전이 나오면 앱이 알려 주고, 확인 한 번으로 다운로드·검증·설치까지 자동 진행됩니다.

---

## 개인정보 · 약관
- [개인정보 처리방침 (Privacy)](PRIVACY.md) · [이용약관 (Terms)](TERMS.md)
- 익명 사용 통계는 설정에서 끌 수 있습니다(opt-out).

## 피드백
버그 제보·기능 제안은 [Issues](https://github.com/Ghostseller/CastFi/issues)에 남겨 주세요.

---

# English

**CastFi connects your Windows PC and Android phone on the same Wi-Fi for music control and audio correction (EQ).**
Control the music playing on your PC (Spotify · YouTube Music) in one place, with system-wide EQ, headphone correction, synced lyrics, and music-video backgrounds.

## Features
- **Playback control** — Spotify (play/pause · next/prev · volume · seek · queue · search · likes via the Web API), YouTube Music (built-in native tab + search), and basic control of other apps via Windows media sessions (SMTC).
- **My Playlists** — songs added from any platform play on Spotify/YT Music (automatic title/artist matching). Tap a song to play the playlist from that song; shuffle & repeat (all/one) apply instantly even during playback; now-playing ▶ indicator; reorder, backup & restore.
- **System EQ & headphone correction** — built on [Equalizer APO](https://equalizerapo.com/). Auto-correction from AutoEQ / squig.link measurements (Harman target), AI EQ from natural language, graphic/parametric editing, presets, import/export (AutoEQ · oratory1990).
- **Lyrics & music videos** — synced lyrics (LRCLIB) with translation and a full-screen view; music-video backgrounds matched to the current song.
- **Signal path** — Roon-style diagram: source → EQ → output device, with format/quality info.
- **Android remote** *(in testing)* — auto-discovers your PC on the same Wi-Fi for remote playback/EQ/lyrics/playlist control. Public release coming.

## Download & Install
1. Get the latest `CastFi-Setup-x.y.z.exe` from **[Releases](https://github.com/Ghostseller/CastFi/releases)**.
2. Run the installer — the app lives in the system tray and keeps running in the background.
3. If Windows SmartScreen warns (code signing is in progress), click **"More info" → "Run anyway"**.

**Requirements** — Windows 10/11 (64-bit); [WebView2 Runtime](https://developer.microsoft.com/microsoft-edge/webview2/) on Windows 10 (usually preinstalled); [Equalizer APO](https://equalizerapo.com/) for EQ features; Spotify Premium for some remote-playback features.

**Getting started** — launch the app, connect Spotify in Settings (one-time browser login); sign in to YT Music inside the built-in tab; search your headphone model in the EQ tab to apply auto-correction.

**Auto-update** — the app notifies you when a new version is available and handles download, verification, and installation with one click.

## Privacy & Terms
[Privacy Policy](PRIVACY.md) · [Terms of Service](TERMS.md). Anonymous usage analytics can be turned off in Settings.

## Feedback
Please report bugs or request features via [Issues](https://github.com/Ghostseller/CastFi/issues).
