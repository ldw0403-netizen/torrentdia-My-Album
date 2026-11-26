# My Album v1.0.3 — 통합 안내 / Unified Guide / 統合ガイド / 统一说明

> 공용 전자앨범 & 디지털 프레임 (General Edition) — Android APK + Windows Portable
>
> 📦 산출물 (Deliverables / 成果物 / 交付物)
>
> | 파일 | 용도 |
> |---|---|
> | `MyAlbum_v1.0.3.apk` | Android 설치 파일 (v1+v2+v3 서명) |
> | `MyAlbum_v1.0.3_Windows_Portable.zip` | Windows 포터블 (압축 해제 후 바로 실행, 설치 불필요) |
> | `README.md` | 본 통합 안내 (KO/EN/JA/ZH) |

---

## 1️⃣ 한국어 (Korean)

### ✅ v1.0.3 변경 사항

| 항목 | 내용 |
|---|---|
| **유튜브 재생 창 이중 노출 제거** | 재생 시 플레이어 박스가 유튜브 섹션 안의 재생 영역 위에 겹쳐 렌더링되던 구조를 폐지하고, 재생 영역(#ytPlayerArea) 안으로 **단일 창 통합**했습니다. 스크롤·회전·키보드 팝업 시에도 재생 창은 화면에 **단 하나만** 존재하며 어긋나지 않습니다. 무드 영상 미니 플레이어와 전체화면(⛶) 모드는 그때만 화면 고정 방식으로 전환됩니다. |
| **홈 복귀 시 검색 초기화** | 유튜브 검색 후 하단 **홈** 탭(또는 다른 탭)으로 이동하면 검색 입력값·검색 결과 목록·상태 메시지를 즉시 초기화합니다. 다시 유튜브 탭으로 돌아오면 이전 검색 기록이 남지 않은 깨끗한 초기 상태로 표시됩니다. (저장한 영상 목록은 유지) |
| **검색창 안내 문구 변경** | `검색어 입력 (예: 아이유 라일락)` → **`보고 싶은 영상이나 노래 제목을 검색해 보세요`** |

### 📱 Android 설치·실행

1. `MyAlbum_v1.0.3.apk`를 기기로 복사 후 실행해 설치합니다. (출처 불명 앱 설치 허용 필요)
2. v1.0.2가 설치되어 있으면 **바로 덮어쓰기 설치**됩니다 (같은 서명 키). v1.0.1 이하에서는 기존 앱 삭제 후 설치해 주세요.
3. 설정에서 사진·음악·로고·날씨 지역을 직접 구성하면 홈 화면 전자앨범이 완성됩니다.

### 🖥️ Windows 포터블 실행

1. `MyAlbum_v1.0.3_Windows_Portable.zip`을 원하는 폴더에 **압축 해제**합니다 (설치 과정 없음).
2. 폴더 안의 **`MyAlbum.exe`**를 실행합니다.
3. 실행 즉시 **풀페이지(전체화면) 화면보호기 감상 모드**로 시작합니다 — 제목 표시줄·작업표시줄 없이 배경과 위젯이 화면 끝까지 표시됩니다.

**입력 감지·제어**

- 평상시에는 화면이 깨끗하게 유지되고(6초 후 UI 자동 숨김·커서 숨김), **마우스 움직임·키보드 입력·클릭/터치**가 감지되면 하단 탭·상단 버튼·BGM 도크·제어 칩이 자연스럽게 나타납니다.
- 우하단 제어 칩: **`⤡ 창 모드` / `⤢ 전체화면`** 전환, **`✕ 종료`** 버튼 제공.
- **`ESC` / `F11`**: 전체화면 ↔ 창 모드 전환 · **`Alt+F4`**: 앱 종료 · **`Alt+Tab`·`Windows` 키**: 다른 화면 전환(OS 기본 동작 그대로 사용 가능).

**포터블 로컬 저장**

- 설정(사진·음악·로고·날씨·언어 등), 저장한 영상 목록, 캐시는 모두 **exe 폴더 안 `data\` 경로**에 저장됩니다.
- 폴더를 통째로 USB·다른 PC로 옮기면 설정까지 그대로 이동하는 진정한 포터블 구조입니다.
- 포터블 폴더에 쓰기 권한이 없는 위치(예: 일부 시스템 폴더)에서 실행하면 기본 위치에 저장하고 한 번 안내를 표시합니다.
- Windows 버전은 Android(v1.0.3)와 **동일한 앱 본체(index.html)**를 사용하므로 유튜브 재생·검색 동작이 완전히 같습니다. Android의 Capacitor 저장 호출은 포터블 `data\files` 폴더로 연결되어 사진·음악·로고가 영구 보존됩니다.

### 🎛️ 주요 기능

- **홈**: 슬라이드 전자앨범 (전환 속도 설정, 로고 이미지+텍스트 동시 표시, 날씨·시계 위젯, 무드 영상 미니 플레이어)
- **구글 포토 / 픽팍**: 계정 연동 후 앱 안에서 바로 열람
- **유튜브**: 검색(최상단) → 붙여넣기 재생 → 쇼츠/일반 통합 목록 → ⛶ 전체화면 최대화
- **설정**: 기기 사진·음악 직접 추가(자동 스캔 없음), 로고 이미지·텍스트 동시 사용, 언어(KO/EN/JA/ZH), 화면 꺼짐 주기
- **BGM**: 설정에서 추가한 음악만 재생 (자동 시작 스위치·반복·볼륨)

---

## 2️⃣ English

### ✅ v1.0.3 Changes

| Item | Description |
|---|---|
| **YouTube player: single window** | The floating player box that overlaid the in-section play area is gone; the player is now **integrated inside the YouTube play area** (#ytPlayerArea). Only **one** playback window exists on screen at any time and it never drifts on scroll, rotation, or keyboard popups. The mood-video mini player and the ⛶ fullscreen mode still switch to fixed positioning only while active. |
| **Search reset on tab change** | Leaving the YouTube tab (Home button or any other tab) now clears the search input, results list, and status message. Returning to YouTube shows a clean initial state. (Saved videos are kept.) |
| **Search placeholder changed** | `검색어 입력 (예: 아이유 라일락)` → **`보고 싶은 영상이나 노래 제목을 검색해 보세요`** ("Search for a video or song you want to watch") |

### 📱 Android Install

1. Copy `MyAlbum_v1.0.3.apk` to the device and open it (allow installing from unknown sources).
2. Over v1.0.2 it installs directly (same signing key). From v1.0.1 or older, uninstall first.
3. Configure photos, music, logo, and the weather region in Settings to complete the album.

### 🖥️ Windows Portable

1. **Extract** `MyAlbum_v1.0.3_Windows_Portable.zip` to any folder — no installer.
2. Run **`MyAlbum.exe`** inside the folder.
3. It starts in **fullscreen screensaver mode** — no title bar, no taskbar; the background and widgets fill the screen edge to edge.

**Input detection & control**

- The UI stays clean while idle (auto-hidden after 6 s, cursor hidden); any **mouse movement, keyboard input, click, or touch** smoothly brings back the bottom tabs, top buttons, BGM dock, and control chip.
- Control chip (bottom-right): **`⤡ Window` / `⤢ Fullscreen`** toggle and **`✕ Exit`**.
- **`ESC` / `F11`**: switch fullscreen ↔ window · **`Alt+F4`**: exit · **`Alt+Tab` / `Windows` key**: standard OS behavior still works.

**Portable local storage**

- Settings, saved-video list, and cache live in the **`data\` folder next to the exe** — copy the whole folder to a USB stick or another PC and everything travels with it.
- If the folder is read-only, the app saves to the default location and shows a one-time notice.
- The Windows build ships the **same app core (index.html)** as Android v1.0.3, so YouTube playback/search behaves identically; Capacitor storage calls are redirected to `data\files` so photos, music, and the logo persist permanently.

### 🎛️ Features

- **Home**: slideshow album (transition speed, logo image + text together, weather & clock widgets, mood-video mini player)
- **Google Photos / PikPak**: linked accounts browsable in-app
- **YouTube**: search (top) → paste-link playback → Shorts/regular merged list → ⛶ fullscreen
- **Settings**: add device photos/music manually (no auto-scan), logo image + text together, languages (KO/EN/JA/ZH), screen-off interval
- **BGM**: only tracks added in Settings (auto-start switch, repeat, volume)

---

## 3️⃣ 日本語 (Japanese)

### ✅ v1.0.3 の変更内容

| 項目 | 内容 |
|---|---|
| **YouTube 再生ウィンドウの二重表示を解消** | セクション内の再生エリアに重なって浮かぶプレイヤーボックス方式を廃止し、再生エリア(#ytPlayerArea)の**内側に単一ウィンドウとして統合**しました。スクロール・回転・キーボード表示時でも**画面に再生ウィンドウは常に1つだけ**存在し、ずれません。ムード動画のミニプレイヤーと ⛶ フルスクリーンモードは、その間だけ固定表示に切り替わります。 |
| **ホーム復帰時に検索を初期化** | 検索後に下の**ホーム**タブ(または他のタブ)へ移ると、検索語・結果リスト・ステータスを即座にクリアします。YouTube タブに戻ると過去の検索が残らないクリーンな初期状態です。(保存済み動画リストは保持) |
| **検索欄のプレースホルダー変更** | `검색어 입력 (예: 아이유 라일락)` → **`보고 싶은 영상이나 노래 제목을 검색해 보세요`**（意味: 見たい動画や曲名を検索してみましょう） |

### 📱 Android インストール

1. `MyAlbum_v1.0.3.apk` を端末にコピーして開く（提供元不明アプリの許可が必要）。
2. v1.0.2 が入っていれば**そのまま上書き**できます（同一署名キー）。v1.0.1 以前は一度アンインストールしてください。
3. 設定タブで写真・音楽・ロゴ・天気地域を指定するとアルバムが完成します。

### 🖥️ Windows ポータブル版

1. `MyAlbum_v1.0.3_Windows_Portable.zip` を任意のフォルダへ**解凍**（インストール作業なし）。
2. フォルダ内の **`MyAlbum.exe`** を実行。
3. 起動直後から**フルスクリーンのスクリーンセーバー鑑賞モード** — タイトルバー・タスクバーなしで背景とウィジェットが画面いっぱいに表示されます。

**入力検知と操作**

- 待機中は画面がクリーンに保たれ（6秒でUI自動非表示・カーソル非表示）、**マウス移動・キーボード入力・クリック/タッチ**を検知すると下タブ・上ボタン・BGMドック・操作チップがスムーズに現れます。
- 右下の操作チップ：**`⤡ ウィンドウ` / `⤢ 全画面`** 切替、**`✕ 終了`**。
- **`ESC` / `F11`**：全画面 ↔ ウィンドウ切替 · **`Alt+F4`**：終了 · **`Alt+Tab` / `Windows`キー**：OS標準動作のまま利用可能。

**ポータブル ローカル保存**

- 設定・保存済み動画リスト・キャッシュはすべて **exe フォルダ内の `data\`** に保存されます。フォルダごとUSBや別PCへ移すと設定もそのまま移行します。
- 書き込み権限がない場所では既定の場所に保存し、一度だけ案内を表示します。
- Windows 版は Android v1.0.3 と**同じアプリ本体(index.html)**を使用するため YouTube の動作は完全に同一です。Capacitor の保存呼び出しは `data\files` へ転送され、写真・音楽・ロゴは永久保存されます。

### 🎛️ 主な機能

- **ホーム**：スライドショーアルバム（切替速度、ロゴ画像＋テキスト同時表示、天気・時計ウィジェット、ムード動画ミニプレイヤー）
- **Google フォト / PikPak**：連携アカウントをアプリ内で閲覧
- **YouTube**：検索(最上部) → リンク貼り付け再生 → ショート/通常 統合リスト → ⛶ フルスクリーン
- **設定**：端末の写真・音楽を手動追加（自動スキャンなし）、ロゴ画像＋テキスト同時使用、言語(KO/EN/JA/ZH)、画面消灯間隔
- **BGM**：設定で追加した曲のみ再生（自動開始スイッチ・リピート・音量）

---

## 4️⃣ 中文 (Chinese)

### ✅ v1.0.3 变更内容

| 项目 | 说明 |
|---|---|
| **YouTube 播放窗口双重显示修复** | 废除悬浮播放框叠加在区块内播放区域之上的旧结构，改为**整合进播放区域(#ytPlayerArea)内部的单窗口**。无论滚动、旋转或弹出键盘，屏幕上**始终只有一个播放窗口**，不会错位。氛围视频迷你播放器和 ⛶ 全屏模式仅在激活时切换为固定定位。 |
| **返回主页时重置搜索** | 在 YouTube 搜索后切换到下方**主页**标签(或其他标签)时，立即清空搜索词、结果列表和状态提示。再次回到 YouTube 时呈现干净的初始状态。(已保存视频列表保留) |
| **搜索框提示语更换** | `검색어 입력 (예: 아이유 라일락)` → **`보고 싶은 영상이나 노래 제목을 검색해 보세요`**（含义：搜索想看的视频或歌曲名称） |

### 📱 Android 安装

1. 将 `MyAlbum_v1.0.3.apk` 复制到设备并打开安装（需允许安装未知来源应用）。
2. 已装 v1.0.2 可直接**覆盖安装**（同一签名密钥）；v1.0.1 及更早版本请先卸载。
3. 在设置中配置照片、音乐、Logo、天气地区即可完成相册。

### 🖥️ Windows 便携版

1. 将 `MyAlbum_v1.0.3_Windows_Portable.zip` **解压**到任意文件夹——无需安装。
2. 运行文件夹内的 **`MyAlbum.exe`**。
3. 启动即为**全屏屏保欣赏模式**——无标题栏、无任务栏，背景与组件铺满整个屏幕。

**输入检测与控制**

- 平时画面保持干净（6 秒后自动隐藏界面并隐藏鼠标指针）；检测到**鼠标移动、键盘输入、点击/触摸**时，底部标签、顶部按钮、BGM 停靠栏和控制芯片会平滑出现。
- 右下角控制芯片：**`⤡ 窗口模式` / `⤢ 全屏`** 切换、**`✕ 退出`**。
- **`ESC` / `F11`**：全屏 ↔ 窗口切换 · **`Alt+F4`**：退出应用 · **`Alt+Tab` / `Windows` 键**：保持系统默认行为，可正常切换窗口。

**便携本地存储**

- 设置、已保存视频列表和缓存全部保存在 **exe 同目录的 `data\` 文件夹**中。整个文件夹拷贝到 U 盘或其他电脑，配置会一并带走。
- 若所在位置没有写入权限，则改用默认位置保存并提示一次。
- Windows 版与 Android v1.0.3 使用**同一应用本体(index.html)**，YouTube 播放/搜索行为完全一致；Capacitor 存储调用被重定向到 `data\files`，照片、音乐、Logo 永久保存。

### 🎛️ 主要功能

- **主页**：幻灯片相册（切换速度、Logo 图片+文字同时显示、天气与时钟组件、氛围视频迷你播放器）
- **Google 相册 / PikPak**：登录后在应用内直接浏览
- **YouTube**：搜索(置顶) → 粘贴链接播放 → Shorts/普通视频合并列表 → ⛶ 全屏最大化
- **设置**：手动添加设备照片与音乐（无自动扫描）、Logo 图片与文字同时启用、界面语言(KO/EN/JA/ZH)、息屏周期
- **BGM**：仅播放设置中添加的音乐（自动播放开关、循环、音量）

---

## 📜 버전 히스토리 / Version History / バージョン履歴 / 版本历史

| 버전 | 주요 내용 |
|---|---|
| **v1.0.3** | 유튜브 재생 창 단일 통합(이중 노출 제거) · 탭 이동 시 검색 초기화 · 검색창 안내 문구 변경 · **Windows 포터블 신규 제공**(전체화면 감상 모드·입력 감지 옵션 UI·포터블 로컬 저장) |
| v1.0.2 | 홈버튼 즉시 복귀(모든 창 닫기+페이드) · 유튜브 정식 아이콘·앱 안 인라인 재생 · 검색 카드 최상단 · 쇼츠/일반 통합+전체화면 · 음악 자동 스캔 제거 · 로고 이미지/텍스트 동시 표시 |
| v1.0.1 | 초기 배포 (Android) |

## 🔑 참고 / Notes / 備考 / 备注

- Android 업그레이드 경로: v1.0.2 → v1.0.3 덮어쓰기 가능(동일 서명). 서명 키: `myalbum.keystore`.
- Windows 포터블 데이터 폴더 구조: `data\User Data\`(설정·캐시) · `data\files\`(사진·음악·로고) · `data\crashDumps\`.
- YouTube 임베드가 차단된 영상은 저작권·임베드 설정상 앱 내 재생이 불가할 수 있으며, 이 경우 앱 안의 '새 창' 버튼으로 이어서 시청할 수 있습니다.
- 무드 영상 모드는 탭을 이동해도 홈 화면에서 계속 재생됩니다.
