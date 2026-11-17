# 🍎 灵动岛 Web 复刻 DynamicIsland-WebDemo

> 一个纯前端实现的 iOS 灵动岛（Dynamic Island）动效复刻，使用 **HTML + CSS + 原生 JavaScript**，无需任何框架依赖，在任意现代浏览器中打开即可运行。

## ✨ 功能特性

- **5 种状态切换**（通过按钮交互或自动触发）
  - ⚫ 空闲（原始黑色胶囊）
  - 📞 来电（头像 + 姓名 + 接听/拒接按钮，头像呼吸动画）
  - 🎵 音乐播放（专辑封面 + 进度条 + 控制按钮，封面旋转动画）
  - ⏱️ 计时器（实时秒数更新）
  - 💬 消息通知（头像 + 发送者 + 消息预览，5 秒自动收起）

- **核心动效实现**
  - 所有状态使用 `cubic-bezier(0.34, 1.56, 0.64, 1)` 弹性缓动曲线，还原苹果原生的 "pop" 弹性感
  - CSS `transition` 实现胶囊大小、圆角、内容的平滑过渡
  - `@keyframes` 动画实现呼吸（pulse）、旋转（spin）、弹入（popIn）效果
  - 使用 `overflow: hidden` + 黑底模拟灵动岛的物理形态

- **零依赖**：不使用 React/Vue/SwiftUI，所有代码在单个 HTML 文件中

## 🚀 快速运行

```bash
# 方式 1：直接打开
open index.html  # macOS
# 或
start index.html # Windows
# 或在 Linux：
xdg-open index.html

# 方式 2：本地服务（推荐）
python3 -m http.server 8080
# 然后访问 http://localhost:8080
```

## 📁 项目结构

```
Lingdongdao-WebDemo/
├── index.html    # 全部代码（HTML + CSS + JS）
├── README.md     # 本文件
└── LICENSE       # MIT License
```

## 🛠️ 技术栈

| 技术 | 用途 |
|---|---|
| HTML5 | 语义化结构 |
| CSS3 | Flex 布局、动画、`cubic-bezier` 弹性曲线、`@keyframes` |
| 原生 JavaScript | 状态切换逻辑、计时器、DOM 操作 |

## 📚 设计参考

- Apple 官方 Dynamic Island 设计语言
- iOS Human Interface Guidelines
- WWDC 2022：Introducing Dynamic Island

## 📝 License

MIT © Mxz-1

---

> 本项目仅用于学习和个人展示，灵感来自 Apple Inc. 的 Dynamic Island 设计。
