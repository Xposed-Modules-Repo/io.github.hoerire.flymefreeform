# Flyme 小窗（FlymeFreeform）

在 ColorOS 上把手边的小窗做得更顺手一点：从屏幕下角斜划呼出扇形菜单，滑到想要的应用松手，小窗直接打开；用完点一下窗外就收起。

模块不添加常驻服务，复用系统已有的自由窗与智能侧边栏能力，只多加一层呼出方式与判定逻辑。

<p align="center">
  <img src="https://raw.githubusercontent.com/Hoerire/FlymeFreeform/main/docs/images/preview.gif" width="320" alt="小窗交互预览" />
</p>

## 功能

- **扇形呼出**：左右下角斜向内上滑呼出扇形菜单，滑到哪一格那一格图标放大反馈，松手即用小窗打开
- **「更多」面板**：分「收藏」与「最近」两组，收藏沿用系统智能侧边栏的设置与排序，最近展示近期启动过的应用
- **窗外关闭**：单击或双击小窗外部即可关闭，也可以整体关掉这个行为
- **上滑迷你窗**：在小窗底部横条上快速上滑，切换成迷你窗
- **快捷项管理**：应用、分身应用、侧边栏工具与快捷入口可混合固定，最多六项，支持拖动排序
- **手势设置**：「触发范围」调整底角手势识别区；「命中范围」（40–140dp，默认 140dp）调整扇形图标的命中半径，拖动时实时预览每一格的命中圈
- **自动暂停**：横屏或游戏模式下自动暂停，退出后恢复，两项可分别关闭

## 截图

<p align="center">
  <img src="https://raw.githubusercontent.com/Hoerire/FlymeFreeform/main/docs/images/more-panel.jpg" width="300" alt="更多面板：收藏与最近" />
  <img src="https://raw.githubusercontent.com/Hoerire/FlymeFreeform/main/docs/images/hit-range-preview.jpg" width="300" alt="命中范围实时预览" />
</p>

## 要求

- ColorOS（Android 15 / API 35 及以上），已在 ColorOS 17 上验证
- LSPosed（libxposed API 102）
- 模块作用域：系统界面、系统框架、桌面、智能侧边栏

## 安装

1. 下载本模块的最新 APK 并安装
2. 在 LSPosed 中启用模块，勾选上面的四个作用域
3. 重启一次设备（模块代码在系统进程里，需要重启才会加载）
4. 打开「Flyme 小窗」应用调整设置，设置项即时生效

## 说明

- 面向 ColorOS 定制，换机型或系统版本可能失效
- 非官方实现，与魅族、Flyme、OPPO、ColorOS 及其关联方无关
- 基于 GPL-3.0 开源的 [Mangi-11/FlymeFreeform](https://github.com/Mangi-11/FlymeFreeform) 继续开发
- 源码：[Hoerire/FlymeFreeform](https://github.com/Hoerire/FlymeFreeform)
