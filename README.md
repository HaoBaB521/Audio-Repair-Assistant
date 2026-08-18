[Uploading Audio_Repair_Assistant_Release_Notes_v2.0.0.0_Beta.md…]()

# 🎵 Audio Repair Assistant v2.0.0.0 Beta

> **作者：浩BaB** | Windows 音频深度修复工具

---

## 📌 版本亮点

v2.0.0.0 Beta 是一次全面重构升级，从命令行脚本进化为带现代化 UI 的桌面应用。

**核心承诺：全程不自动改动用户默认音频设备**，只修复系统层面的音频问题。

---

## ✨ 新增功能

- **7 语言实时切换**：English / 简体中文 / 繁體中文 / Русский / 日本語 / 한국어 / Español，设置内一键切换，界面文字即时生效，作者名「浩BaB」所有语言保持原样
- **全新美化 UI**：基于 customtkinter 的左右分栏卡片布局，Microsoft YaHei UI 清晰字体，支持深色/浅色/跟随系统主题
- **设置面板**：语言切换、主题切换、开机自启、修复后自动重启、记住上次选项、创建桌面快捷方式、打开程序目录、关于页
- **修复后设备选择**：修复完成自动弹出设备选择对话框，可手动指定默认音频输出设备
- **独立卸载程序**：安装包内嵌 uninstall.exe，支持控制面板卸载和目录内直接卸载
- **自定义安装目录**：安装时可选择任意路径，相关文件统一归档

---

## 🔧 修复策略（7 项）

| 策略 | 说明 |
|------|------|
| 🔄 重启音频服务 | 重启 Windows Audio / Endpoint Builder / MMCSS |
| 🔒 禁用自动切换设备 | 防止系统自动锁定/切换默认音频设备（核心修复） |
| 🎚 禁用音频增强 | 关闭 Win11 音频处理层，减少延迟和爆音 |
| 🚫 禁用独占模式 | 防止应用独占音频导致其他程序无声 |
| 🧹 清理异常进程 | 终止 Nahimic / Realtek 等残留进程 |
| 📦 重新注册音频组件 | 修复 audioses / mmdevapi 等 DLL |
| 🔍 系统文件检查 SFC | 检查损坏系统文件，限时 60 秒防卡死 |

---

## ⚙️ 设置项

- 🌐 **语言**：7 种语言国旗按钮网格选择，实时切换
- 🎨 **外观**：深色 / 浅色 / 跟随系统
- 🔧 **常规**：开机自启、修复后自动重启（10秒）、记住上次修复选项
- 📌 **快捷方式**：一键创建桌面快捷方式、打开程序目录
- ℹ **关于**：版本号、作者、配置文件路径

---

## 🛡 技术特性

- 全局异常捕获，崩溃写入 `crash_log.txt`，防闪退
- 管理员权限自动检测与提权
- SFC 扫描 60 秒超时强制终止，避免长时间等待
- 快捷方式创建 win32com + PowerShell 双重保障
- 设置持久化到 `settings.json`

---

## 📦 交付文件

| 文件 | 说明 | 大小 |
|------|------|------|
| `ARA_Setup.exe` | 安装包（内嵌主程序+卸载程序+图标） | 42.7MB |
| `AudioRepairAssistant.exe` | 便携版（免安装） | 14.8MB |
| `uninstall.exe` | 独立卸载程序 | 13.7MB |

---

## ⚠️ 注意事项

- 部分修复操作需要管理员权限，程序会自动提示提权
- 修复完成后建议重启电脑使设置完全生效
- 默认音频设备不会被自动改动，需手动在「选择设备」中指定

---
---

# 🎵 Audio Repair Assistant v2.0.0.0 Beta（繁體中文）

> **作者：浩BaB** | Windows 音訊深度修復工具

---

## 📌 版本亮點

v2.0.0.0 Beta 是一次全面重構升級，從命令列指令碼進化為帶現代化 UI 的桌面應用。

**核心承諾：全程不自動變更使用者預設音訊裝置**，只修復系統層面的音訊問題。

---

## ✨ 新增功能

- **7 語言即時切換**：English / 简体中文 / 繁體中文 / Русский / 日本語 / 한국어 / Español，設定內一鍵切換，介面文字即時生效，作者名「浩BaB」所有語言保持原樣
- **全新美化 UI**：基於 customtkinter 的左右分欄卡片佈局，Microsoft YaHei UI 清晰字體，支援深色/淺色/跟隨系統主題
- **設定面板**：語言切換、主題切換、開機自啟、修復後自動重啟、記住上次選項、建立桌面捷徑、開啟程式目錄、關於頁
- **修復後裝置選擇**：修復完成自動彈出裝置選擇對話框，可手動指定預設音訊輸出裝置
- **獨立解除安裝程式**：安裝包內嵌 uninstall.exe，支援控制台解除安裝和目錄內直接解除安裝
- **自訂安裝目錄**：安裝時可選擇任意路徑，相關檔案統一歸檔

---

## 🔧 修復策略（7 項）

| 策略 | 說明 |
|------|------|
| 🔄 重啟音訊服務 | 重啟 Windows Audio / Endpoint Builder / MMCSS |
| 🔒 停用自動切換裝置 | 防止系統自動鎖定/切換預設音訊裝置（核心修復） |
| 🎚 停用音訊增強 | 關閉 Win11 音訊處理層，減少延遲和爆音 |
| 🚫 停用獨佔模式 | 防止應用獨佔音訊導致其他程式無聲 |
| 🧹 清理異常程序 | 終止 Nahimic / 瑞昱 等殘留程序 |
| 📦 重新註冊音訊元件 | 修復 audioses / mmdevapi 等 DLL |
| 🔍 系統檔案檢查 SFC | 檢查損毀系統檔案，限時 60 秒防卡死 |

---

## ⚙️ 設定項

- 🌐 **語言**：7 種語言國旗按鈕網格選擇，即時切換
- 🎨 **外觀**：深色 / 淺色 / 跟隨系統
- 🔧 **一般**：開機自啟、修復後自動重啟（10秒）、記住上次修復選項
- 📌 **捷徑**：一鍵建立桌面捷徑、開啟程式目錄
- ℹ **關於**：版本號、作者、設定檔路徑

---

## 🛡 技術特性

- 全域例外攔截，崩潰寫入 `crash_log.txt`，防閃退
- 系統管理員權限自動偵測與提權
- SFC 掃描 60 秒逾時強制終止，避免長時間等待
- 捷徑建立 win32com + PowerShell 雙重保障
- 設定持久化到 `settings.json`

---

## 📦 交付檔案

| 檔案 | 說明 | 大小 |
|------|------|------|
| `ARA_Setup.exe` | 安裝包（內嵌主程式+解除安裝程式+圖示） | 42.7MB |
| `AudioRepairAssistant.exe` | 可攜版（免安裝） | 14.8MB |
| `uninstall.exe` | 獨立解除安裝程式 | 13.7MB |

---

## ⚠️ 注意事項

- 部分修復操作需要系統管理員權限，程式會自動提示提權
- 修復完成後建議重啟電腦使設定完全生效
- 預設音訊裝置不會被自動變更，需手動在「選擇裝置」中指定

---
---

# 🎵 Audio Repair Assistant v2.0.0.0 Beta（English）

> **Author: 浩BaB** | Windows Audio Deep Repair Tool

---

## 📌 Release Highlights

v2.0.0.0 Beta is a full rebuild upgrade, evolving from a command-line script to a modern UI desktop application.

**Core promise: never automatically changes your default audio device** — only repairs system-level audio issues.

---

## ✨ New Features

- **7-Language Real-Time Switching**: English / 简体中文 / 繁體中文 / Русский / 日本語 / 한국어 / Español. One-click switch in settings, UI text updates instantly. Author name "浩BaB" stays unchanged across all languages.
- **All-New Polished UI**: customtkinter-based two-column card layout, clear Microsoft YaHei UI fonts, supports Dark / Light / System theme
- **Settings Panel**: language switch, theme switch, auto-start on boot, auto-reboot after repair, remember last options, create desktop shortcut, open program folder, about page
- **Post-Repair Device Selection**: device picker dialog pops up automatically after repair, manually set default audio output device
- **Standalone Uninstaller**: uninstall.exe embedded in installer, supports Control Panel uninstall and direct folder uninstall
- **Custom Install Directory**: choose any path during install, all related files archived together

---

## 🔧 Repair Strategies (7 items)

| Strategy | Description |
|----------|-------------|
| 🔄 Restart Audio Services | Restart Windows Audio / Endpoint Builder / MMCSS |
| 🔒 Disable Auto-Switch Device | Prevent system from auto-locking/switching default device (core fix) |
| 🎚 Disable Audio Enhancements | Turn off Win11 audio processing layer, reduce latency and crackling |
| 🚫 Disable Exclusive Mode | Prevent apps from独占 audio, causing other apps silent |
| 🧹 Clean Abnormal Processes | Terminate Nahimic / Realtek residual processes |
| 📦 Re-register Audio Components | Repair audioses / mmdevapi DLLs |
| 🔍 System File Check (SFC) | Check corrupted system files, 60s timeout to prevent hang |

---

## ⚙️ Settings

- 🌐 **Language**: 7-language flag button grid, real-time switch
- 🎨 **Appearance**: Dark / Light / System
- 🔧 **General**: auto-start on boot, auto-reboot after repair (10s), remember last repair options
- 📌 **Shortcut**: one-click create desktop shortcut, open program folder
- ℹ **About**: version, author, config file path

---

## 🛡 Technical Features

- Global exception handler, crashes logged to `crash_log.txt`, prevents silent exit
- Automatic admin privilege detection and elevation
- SFC scan 60-second timeout force-kill, avoids long waits
- Shortcut creation via win32com + PowerShell dual fallback
- Settings persisted to `settings.json`

---

## 📦 Deliverables

| File | Description | Size |
|------|-------------|------|
| `ARA_Setup.exe` | Installer (embedded app + uninstaller + icon) | 42.7MB |
| `AudioRepairAssistant.exe` | Portable (no install) | 14.8MB |
| `uninstall.exe` | Standalone uninstaller | 13.7MB |

---

## ⚠️ Notes

- Some repairs require admin privileges, app will prompt for elevation automatically
- Recommend reboot after repair for all settings to take full effect
- Default audio device is never changed automatically — set it manually via "Select Device"

---
---

# 🎵 Audio Repair Assistant v2.0.0.0 Beta（日本語）

> **作者: 浩BaB** | Windows オーディオ深度修復ツール

---

## 📌 バージョンハイライト

v2.0.0.0 Beta は全面リニューアルアップグレードで、コマンドラインスクリプトからモダンな UI を備えたデスクトップアプリへ進化しました。

**コアプロミス：デフォルトオーディオデバイスを自動で変更しません** — システムレベルのオーディオ問題のみ修復します。

---

## ✨ 新機能

- **7言語リアルタイム切替**: English / 简体中文 / 繁體中文 / Русский / 日本語 / 한국어 / Español。設定内でワンクリック切替、UI テキストが即時反映されます。作者名「浩BaB」は全言語でそのまま保持されます。
- **全新美化 UI**: customtkinter ベースの左右2カラムカードレイアウト、鮮明な Microsoft YaHei UI フォント、ダーク/ライト/システムテーマ対応
- **設定パネル**: 言語切替、テーマ切替、起動時自動開始、修復後自動再起動、前回オプション記憶、デスクトップショートカット作成、プログラムフォルダを開く、バージョン情報
- **修復後デバイス選択**: 修復完了後にデバイス選択ダイアログが自動表示、デフォルトオーディオ出力デバイスを手動指定可能
- **スタンドアロンアンインストーラー**: uninstall.exe をインストーラーに内蔵、コントロールパネルからのアンインストールとフォルダ直接アンインストールに対応
- **カスタムインストールディレクトリ**: インストール時に任意のパスを選択可能、関連ファイルを一括アーカイブ

---

## 🔧 修復ストラテジー（7項目）

| ストラテジー | 説明 |
|-------------|------|
| 🔄 オーディオサービス再起動 | Windows Audio / Endpoint Builder / MMCSS を再起動 |
| 🔒 自動切換を無効化 | システムがデフォルトデバイスを自動変更するのを防止（コア修復） |
| 🎚 音声強調を無効化 | Win11 オーディオ処理レイヤーをオフ、遅延とノイズを削減 |
| 🚫 排他モード無効化 | アプリがオーディオを独占し他のプログラムが無音になるのを防止 |
| 🧹 異常プロセス清理 | Nahimic / Realtek などの残留プロセスを終了 |
| 📦 オーディオコンポーネント再登録 | audioses / mmdevapi などの DLL を修復 |
| 🔍 システムファイル検査(SFC) | 破損ファイルを検査、60秒タイムアウトでフリーズ防止 |

---

## ⚙️ 設定項目

- 🌐 **言語**: 7言語の国旗ボタングリッド、リアルタイム切替
- 🎨 **外観**: ダーク / ライト / システム
- 🔧 **一般**: 起動時自動開始、修復後自動再起動（10秒）、前回修復オプション記憶
- 📌 **ショートカット**: ワンクリックでデスクトップショートカット作成、プログラムフォルダを開く
- ℹ **バージョン情報**: バージョン、作者、設定ファイルパス

---

## 🛡 技術特性

- グローバル例外ハンドラ、クラッシュを `crash_log.txt` に記録、サイレント終了を防止
- 管理者権限の自動検出と昇格
- SFC スキャン 60 秒タイムアウトで強制終了、長時間待機を回避
- ショートカット作成は win32com + PowerShell デュアル保証
- 設定は `settings.json` に永続化

---

## 📦 配布ファイル

| ファイル | 説明 | サイズ |
|---------|------|--------|
| `ARA_Setup.exe` | インストーラー（アプリ+アンインストーラー+アイコン内蔵） | 42.7MB |
| `AudioRepairAssistant.exe` | ポータブル版（インストール不要） | 14.8MB |
| `uninstall.exe` | スタンドアロンアンインストーラー | 13.7MB |

---

## ⚠️ 注意事項

- 一部の修復には管理者権限が必要、アプリが自動で昇格を促します
- 修復後は PC を再起動して設定を完全に反映させることを推奨
- デフォルトオーディオデバイスは自動変更されません —「デバイス選択」で手動設定してください

---
---

# 🎵 Audio Repair Assistant v2.0.0.0 Beta（한국어）

> **저자: 浩BaB** | Windows 오디오 딥 복구 도구

---

## 📌 버전 하이라이트

v2.0.0.0 Beta는 명령줄 스크립트에서 현대적인 UI의 데스크톱 앱으로 진화한 전면 재구축 업그레이드입니다.

**핵심 약속：기본 오디오 장치를 절대 자동으로 변경하지 않습니다** — 시스템 레벨의 오디오 문제만 복구합니다.

---

## ✨ 새로운 기능

- **7개 언어 실시간 전환**: English / 简体中文 / 繁體中文 / Русский / 日本語 / 한국어 / Español. 설정에서 원클릭 전환, UI 텍스트가 즉시 반영됩니다. 저자명 "浩BaB"은 모든 언어에서 그대로 유지됩니다.
- **새롭게 디자인된 UI**: customtkinter 기반 2열 카드 레이아웃, 선명한 Microsoft YaHei UI 폰트, 다크/라이트/시스템 테마 지원
- **설정 패널**: 언어 전환, 테마 전환, 부팅 시 자동 시작, 수리 후 자동 재시작, 마지막 옵션 기억, 바탕화면 바로가기 만들기, 프로그램 폴더 열기, 정보
- **수리 후 장치 선택**: 수리 완료 후 장치 선택 대화상자가 자동 표시, 기본 오디오 출력 장치를 수동 지정 가능
- **독립형 제거 프로그램**: uninstall.exe가 설치 프로그램에 내장, 제어판 제거와 폴더 직접 제거 지원
- **사용자 정의 설치 디렉토리**: 설치 시 원하는 경로 선택 가능, 관련 파일을 일괄 아카이브

---

## 🔧 복구 전략 (7가지)

| 전략 | 설명 |
|------|------|
| 🔄 오디오 서비스 재시작 | Windows Audio / Endpoint Builder / MMCSS 재시작 |
| 🔒 자동 전환 비활성화 | 시스템이 기본 장치를 자동 변경하는 것 방지 (핵심 복구) |
| 🎚 오디오 향상 비활성화 | Win11 오디오 처리 레이어 끄기, 지연과 노이즈 감소 |
| 🚫 독점 모드 비활성화 | 앱이 오디오를 독점하여 다른 프로그램이 무음이 되는 것 방지 |
| 🧹 비정상 프로세스 정리 | Nahimic / Realtek 등 잔여 프로세스 종료 |
| 📦 오디오 구성요소 재등록 | audioses / mmdevapi 등 DLL 복구 |
| 🔍 시스템 파일 검사(SFC) | 손상된 파일 검사, 60초 제한으로 프리즈 방지 |

---

## ⚙️ 설정 항목

- 🌐 **언어**: 7개 언어 국기 버튼 그리드, 실시간 전환
- 🎨 **외관**: 다크 / 라이트 / 시스템
- 🔧 **일반**: 부팅 시 자동 시작, 수리 후 자동 재시작 (10초), 마지막 수리 옵션 기억
- 📌 **바로가기**: 원클릭 바탕화면 바로가기 만들기, 프로그램 폴더 열기
- ℹ **정보**: 버전, 저자, 설정 파일 경로

---

## 🛡 기술적 특징

- 전역 예외 처리, 크래시를 `crash_log.txt`에 기록, 자동 종료 방지
- 관리자 권한 자동 감지 및 상승
- SFC 스캔 60초 타임아웃 강제 종료, 장시간 대기 방지
- 바로가기 생성은 win32com + PowerShell 이중 보장
- 설정은 `settings.json`에 영구 저장

---

## 📦 배포 파일

| 파일 | 설명 | 크기 |
|------|------|------|
| `ARA_Setup.exe` | 설치 프로그램 (앱+제거 프로그램+아이콘 내장) | 42.7MB |
| `AudioRepairAssistant.exe` | 포터블 버전 (설치 불필요) | 14.8MB |
| `uninstall.exe` | 독립형 제거 프로그램 | 13.7MB |

---

## ⚠️ 주의사항

- 일부 복구에는 관리자 권한이 필요하며, 앱이 자동으로 상승을 요청합니다
- 수리 후 PC를 재시작하여 모든 설정이 완전히 적용되도록 권장합니다
- 기본 오디오 장치는 자동으로 변경되지 않습니다 — "장치 선택"에서 수동으로 설정하세요

---
---

# 🎵 Audio Repair Assistant v2.0.0.0 Beta（Русский）

> **Автор: 浩BaB** | Инструмент глубокого восстановления аудио Windows

---

## 📌 Основные моменты релиза

v2.0.0.0 Beta — это полная переработка и升级, эволюция от командного скрипта до десктопного приложения с современным интерфейсом.

**Главное обещание：никогда не меняет устройство по умолчанию автоматически** — восстанавливает только системные проблемы аудио.

---

## ✨ Новые возможности

- **Переключение 7 языков в реальном времени**: English / 简体中文 / 繁體中文 / Русский / 日本語 / 한국어 / Español. Одно нажатие в настройках, текст интерфейса обновляется мгновенно. Имя автора «浩BaB» остаётся неизменным на всех языках.
- **Полностью обновлённый интерфейс**: двухколоночная карточная раскладка на customtkinter, чёткие шрифты Microsoft YaHei UI, поддержка тёмной/светлой/системной темы
- **Панель настроек**: переключение языка, темы, автозапуск при загрузке, автоперезагрузка после ремонта, запоминание последних опций, создание ярлыка на рабочем столе, открытие папки программы, о программе
- **Выбор устройства после ремонта**: диалог выбора устройства появляется автоматически после ремонта, можно вручную задать устройство вывода по умолчанию
- **Автономная программа удаления**: uninstall.exe встроен в установщик, поддерживает удаление через панель управления и напрямую из папки
- **Пользовательский каталог установки**: можно выбрать любой путь при установке, все связанные файлы архивируются вместе

---

## 🔧 Стратегии восстановления (7 пунктов)

| Стратегия | Описание |
|-----------|----------|
| 🔄 Перезапуск аудио служб | Перезапуск Windows Audio / Endpoint Builder / MMCSS |
| 🔒 Отключить авто-переключение | Запретить системе менять устройство по умолчанию (основное исправление) |
| 🎚 Отключить улучшения аудио | Выключить слой обработки Win11, уменьшить задержку и помехи |
| 🚫 Отключить монопольный режим | Запретить приложениям захватывать аудио, из-за чего другие программы молчат |
| 🧹 Очистка процессов | Завершить остаточные процессы Nahimic / Realtek |
| 📦 Перерегистрация компонентов | Восстановить DLL audioses / mmdevapi |
| 🔍 Проверка файлов (SFC) | Проверка повреждённых файлов, таймаут 60с для предотвращения зависания |

---

## ⚙️ Настройки

- 🌐 **Язык**: сетка кнопок с флагами 7 языков, переключение в реальном времени
- 🎨 **Внешний вид**: Тёмная / Светлая / Системная
- 🔧 **Общее**: автозапуск при загрузке, автоперезагрузка после ремонта (10с), запоминать последние опции
- 📌 **Ярлык**: создание ярлыка на рабочем столе в один клик, открытие папки программы
- ℹ **О программе**: версия, автор, путь к конфигу

---

## 🛡 Технические особенности

- Глобальный обработчик исключений, краши записываются в `crash_log.txt`, предотвращает тихий выход
- Автоматическое определение и повышение прав администратора
- SFC сканирование с принудительным завершением по таймауту 60с, избегает долгих ожиданий
- Создание ярлыка через win32com + PowerShell двойной запасной вариант
- Настройки сохраняются в `settings.json`

---

## 📦 Поставляемые файлы

| Файл | Описание | Размер |
|------|----------|--------|
| `ARA_Setup.exe` | Установщик (встроены приложение+удалитель+иконка) | 42.7MB |
| `AudioRepairAssistant.exe` | Портативная версия (без установки) | 14.8MB |
| `uninstall.exe` | Автономная программа удаления | 13.7MB |

---

## ⚠️ Примечания

- Некоторые восстановления требуют прав администратора, приложение автоматически запросит повышение
- Рекомендуется перезагрузка после ремонта для полного применения всех настроек
- Устройство по умолчанию никогда не меняется автоматически — задайте его вручную через «Выбрать устройство»

---
---

# 🎵 Audio Repair Assistant v2.0.0.0 Beta（Español）

> **Autor: 浩BaB** | Herramienta de reparación profunda de audio Windows

---

## 📌 Destacados de la versión

v2.0.0.0 Beta es una actualización de reconstrucción completa, evolucionando de un script de línea de comandos a una aplicación de escritorio con interfaz moderna.

**Promesa principal：nunca cambia automáticamente tu dispositivo de audio predeterminado** — solo repara problemas de audio a nivel de sistema.

---

## ✨ Nuevas funciones

- **Cambio de 7 idiomas en tiempo real**: English / 简体中文 / 繁體中文 / Русский / 日本語 / 한국어 / Español. Un clic en ajustes, el texto de la interfaz se actualiza al instante. El nombre del autor "浩BaB" se mantiene igual en todos los idiomas.
- **Interfaz completamente renovada**: diseño de tarjetas de dos columnas basado en customtkinter, fuentes claras Microsoft YaHei UI, soporta tema Oscuro / Claro / Sistema
- **Panel de ajustes**: cambio de idioma, cambio de tema, inicio automático al arrancar, reinicio automático tras reparar, recordar últimas opciones, crear acceso directo, abrir carpeta del programa, acerca de
- **Selección de dispositivo tras reparar**: diálogo de selección aparece automáticamente tras la reparación, puedes establecer manualmente el dispositivo de salida predeterminado
- **Desinstalador independiente**: uninstall.exe integrado en el instalador, soporta desinstalación desde panel de control y directamente desde la carpeta
- **Directorio de instalación personalizado**: elige cualquier ruta al instalar, todos los archivos relacionados se archivan juntos

---

## 🔧 Estrategias de reparación (7 elementos)

| Estrategia | Descripción |
|------------|-------------|
| 🔄 Reiniciar servicios de audio | Reiniciar Windows Audio / Endpoint Builder / MMCSS |
| 🔒 Desactivar auto-cambio | Evitar que el sistema cambie el dispositivo predeterminado (corrección principal) |
| 🎚 Desactivar mejoras de audio | Apagar capa de procesamiento Win11, reducir latencia y crujidos |
| 🚫 Desactivar modo exclusivo | Evitar que apps acaparen el audio, haciendo que otras apps se queden mudas |
| 🧹 Limpiar procesos anormales | Terminar procesos residuales Nahimic / Realtek |
| 📦 Re-registrar componentes | Reparar DLL audioses / mmdevapi |
| 🔍 Comprobación de archivos (SFC) | Comprobar archivos dañados, tiempo máximo 60s para evitar bloqueos |

---

## ⚙️ Ajustes

- 🌐 **Idioma**: cuadrícula de botones con banderas de 7 idiomas, cambio en tiempo real
- 🎨 **Apariencia**: Oscuro / Claro / Sistema
- 🔧 **General**: inicio automático al arrancar, reinicio automático tras reparar (10s), recordar últimas opciones
- 📌 **Acceso directo**: crear acceso directo en un clic, abrir carpeta del programa
- ℹ **Acerca de**: versión, autor, ruta del archivo de configuración

---

## 🛡 Características técnicas

- Manejador global de excepciones, los fallos se registran en `crash_log.txt`, evita cierres silenciosos
- Detección automática y elevación de privilegios de administrador
- Escaneo SFC con terminación forzada por tiempo máximo de 60s, evita esperas largas
- Creación de acceso directo vía win32com + PowerShell doble respaldo
- Ajustes guardados en `settings.json`

---

## 📦 Archivos entregados

| Archivo | Descripción | Tamaño |
|---------|-------------|--------|
| `ARA_Setup.exe` | Instalador (app + desinstalador + icono integrados) | 42.7MB |
| `AudioRepairAssistant.exe` | Versión portátil (sin instalación) | 14.8MB |
| `uninstall.exe` | Desinstalador independiente | 13.7MB |

---

## ⚠️ Notas

- Algunas reparaciones requieren privilegios de administrador, la app lo solicitará automáticamente
- Se recomienda reiniciar tras reparar para que todos los ajustes surtan efecto completo
- El dispositivo de audio predeterminado nunca se cambia automáticamente — establécelo manualmente desde "Seleccionar dispositivo"
