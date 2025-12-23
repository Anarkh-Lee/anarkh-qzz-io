# 📟 Anarkh Terminal Portfolio

> A retro, interactive terminal-style personal website.
> <br>
> **Live Demo:** [https://anarkh.qzz.io](https://anarkh.qzz.io)

![License](https://img.shields.io/badge/license-MIT-green)
![Status](https://img.shields.io/badge/status-online-brightgreen)
![Style](https://img.shields.io/badge/style-cyberpunk-purple)

## 📖 Introduction

**Anarkh Terminal** 是一个极简主义的单页（Single-Page）个人作品集网站，模拟了复古 CRT 显示器和 Linux 终端的交互体验。

它专为展示开发者（特别是后端/架构师）的技术栈而设计，去除了现代网页的浮华，回归纯粹的命令行交互。访问者可以通过输入命令（如 `help`, `skills`, `project`）来探索我的个人信息。

## ✨ Features

* **📺 CRT 视觉特效**：模拟老式显示器的扫描线（Scanlines）、微光和屏幕弧度感。
* **⌨️ 真实交互**：支持键盘打字输入，模拟真实的 Shell 体验。
* **🔊 打字机动画**：开机自检（Boot sequence）与输出文本均带有逐字打印动画。
* **📱 响应式设计**：支持移动端访问，点击屏幕即可唤起虚拟键盘进行交互。
* **⚡️ 极致轻量**：纯原生 HTML/CSS/JS 实现，无任何第三方依赖框架，加载速度极快。
* **🔒 隐私友好**：无 Cookie，无追踪。

## 🛠️ Tech Stack

* **Core:** HTML5, CSS3 (Variables & Animations), Vanilla JavaScript (ES6+).
* **Hosting:** Cloudflare Pages (自动部署).
* **Domain:** `anarkh.qzz.io`.

## 🚀 Quick Start

### 本地运行
只需要克隆仓库并直接在浏览器打开 `index.html` 即可：

```bash
git clone [https://github.com/yourname/anarkh-site.git](https://github.com/yourname/anarkh-site.git)
cd anarkh-site
# 双击 index.html 或使用 Live Server 打开
```

### 部署 (Cloudflare Pages)

1. Fork 本仓库。
2. 登录 [Cloudflare Dashboard](https://dash.cloudflare.com)。
3. 进入 **Workers & Pages** -> **Create Application** -> **Pages** -> **Connect to Git**。
4. 选择本仓库，**Build Settings** 全部留空（因为是纯静态 HTML）。
5. 点击 **Deploy**。

## ⚙️ Customization (如何修改内容)

所有显示的文本和命令逻辑都位于 `index.html`底部的 `<script>` 标签中。你可以通过修改 `commands` 对象来自定义你自己的简历。

打开 `index.html`，找到以下部分进行修改：

JavaScript



```
const commands = {
    // 修改 'about' 命令的输出
    'about': 'Hello! I am a Java Development Engineer...',
    
    // 修改 'skills' 命令的输出
    'skills': 'Backend: Java, Spring Boot...',
    
    // 添加你自己的新命令
    'mycmd': 'This is a custom command response.',
    
    // ...
};
```

## 📝 Command List

当前支持的命令：

- `help`: 显示帮助菜单。
- `whoami`: 显示当前用户身份。
- `skills`: 展示技术栈 (Java, Neo4j, etc.)。
- `project`: 展示近期项目经验。
- `contact`: 获取联系方式。
- `clear`: 清屏。
- `reboot`: 重启终端（刷新页面）。
- `sudo`: 尝试获取超级管理员权限（彩蛋）。

## 📄 License

MIT License © 2025 Anarkh