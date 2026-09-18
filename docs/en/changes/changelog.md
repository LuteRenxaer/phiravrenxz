# Release notes

Newest first. Published versions come from the project releases on GitHub and are quoted as published (they are written in Chinese); character-related entries have been removed. The first section covers changes that are in the source tree but not released yet.

## Source (unreleased)

These changes are in the source tree with no release behind them, from commit `e0c4b51` (the multiplayer / first-run / judgement batch) onwards. Build from source to use them.

Multiplayer:

- No spectating
- No results screen: a match ends straight back in the room
- The room-selection (lobby) page was rebuilt, its stat blocks following the parallelogram style of `ending.rs`
- The connect page keeps only two buttons: connect and back to home
- The pause / resume countdown is back to 3 seconds

Room page:

- The score cards lost their black-and-white gradient background
- The grade slot shows the real grade (F / C / B / A / S / V)
- The start button is greyed out and disabled instead of being hidden when the conditions are not met
- Picking a chart starts downloading / syncing it in the background right away
- The buttons at the end of the top bar are laid out by text width
- The bold black line on the right is gone, and the bright end of the bottom-right gradient is brighter

Interface and first run:

- A new first-run wizard: language, sign-in, volume, other settings, final confirmation, and only then the main screen; returning players do not see it again
- The loading screen was re-animated: the background slides in from the right, the panel fades in offset to the left, the cover fades in; pressing start fires a full-screen white flash
- The start button on the song select screen is now a white parallelogram, with a proportionally smaller icon that dims while held
- Full-screen adaptation: 16:10, 21:9, 4:3 and portrait all lay out correctly (supported range 21:9 to 9:16)

Judgement:

- Flick matches Phira: it is no longer "pre-judged" into a free Perfect before you actually swipe, and the late-press protection was added

## v1.3.15fix — 2026-08-23

- 修复 bug
- 新增谱面 Phira-Firefly Tutorial EX

Assets: PhirLie_v1.3.15_fix.apk (243.4 MB), PhirLie_v1.3.15_PC_fix.zip (268.9 MB)

## v1.3.1fix — 2026-08-23

- 修了一些 bug

Assets: PhirLie_v1.3.1_fix.apk (250.3 MB), PhirLie_v1.3.1_PC_fix.zip (258.8 MB)

## v1.3.0 — 2026-08-21

1. 新增 UI 比例功能，可缩放菜单 UI / 字体 / 触摸，背景不缩放
2. 显示分数默认打开，低分辨率默认关闭
3. 个人资料页面美化，平行四边形风格，去掉阴影
4. 修复输入框无法复制粘贴的 bug
5. 导出谱面支持 pez 格式
6. 支持批量下载谱面
7. 去掉原来的输入框，改成游戏内输入框
8. 新增旧主页模式，可切换旧版背景和音乐
9. 设置页新增自定义栏，可调整 UI 位置 / 主页 UI 偏移 / 主题色等
10. 暂停界面重做，仿 ending.rs 布局
11. 修复多纹理模型兼容性和表情堆叠问题
12. 设置菜单栏支持滚动
13. 修复视频播放 / 谱面解锁动画闪退
14. 修复 drag / flick 键盘判定、输入法卡键等问题
15. 内置谱面
16. 添加 XC-SIM（需登录）
17. 首个有 APK 的版本

Assets: PhirLie-v1.3.0-native-input.apk (241.7 MB), PhirLie_v1.3.0_PC.zip (256 MB)

## v1.2.84 — 2026-08-16

1. 更改 UI
2. 添加新设置功能
3. 修复谱面库闪退的 bug
4. 移除了 cmd 窗口

Assets: PhirLie.v1.2.84.zip (88 MB)

## v1.2.55 — 2026-08-06

1. 修改了 ending.rs、loading.rs
2. 没有了

Assets: phirLte-win-v1.2.55.zip (57.8 MB)

## v1.2.54 — 2026-08-03

1. 修了一点点 bug
2. 只有 Windows 版本

Assets: PhirLie.zip (54.3 MB)

---

All versions and assets: [GitHub Releases](https://github.com/LuteRenxaer/Phira-Vrenxz/releases).
