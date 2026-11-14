# 第一课参考资料

## VS Code 界面、工作区和快捷键

- [官方入门教程](https://code.visualstudio.com/docs/editing/getting-started/editor-tutorial)带你打开项目并完成一次编辑。
- [界面总览](https://code.visualstudio.com/docs/editing/getting-started/userinterface)介绍活动栏、编辑区、底部面板和分屏。
- [工作区](https://code.visualstudio.com/docs/editing/workspaces/workspaces)解释打开文件夹和多根工作区。
- [默认快捷键](https://code.visualstudio.com/docs/reference/default-keybindings) · [Windows 一页速查表](https://code.visualstudio.com/shortcuts/keyboard-shortcuts-windows.pdf)
- [集成终端](https://code.visualstudio.com/docs/terminal/basics) · [终端字体与外观](https://code.visualstudio.com/docs/terminal/appearance)
- [VS Code Markdown](https://code.visualstudio.com/docs/languages/markdown)介绍内置预览。

## 查找、跨文件跳转和编辑

- [基本编辑](https://code.visualstudio.com/docs/editing/codebasics)介绍多光标、跨文件搜索和替换预览。
- [代码导航](https://code.visualstudio.com/docs/editing/editingevolved)介绍面包屑、跳转到定义和查找引用。
- [IntelliSense](https://code.visualstudio.com/docs/editing/intellisense) · [JavaScript 支持](https://code.visualstudio.com/docs/languages/javascript) · [自定义代码片段](https://code.visualstudio.com/docs/editing/userdefinedsnippets)
- [VS Code 调试](https://code.visualstudio.com/docs/debugtest/debugging)介绍断点、变量和调用栈。

## 扩展与配置

- 安装和管理扩展，准备独立的演示配置。[扩展市场](https://code.visualstudio.com/docs/configure/extensions/extension-marketplace) · [Profiles](https://code.visualstudio.com/docs/configure/profiles)
- 界面语言。[简体中文语言包](https://marketplace.visualstudio.com/items?itemName=MS-CEINTL.vscode-language-pack-zh-hans) · [显示语言设置](https://code.visualstudio.com/docs/configure/locales)
- 静态页面预览，保存后自动刷新。[Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
- 选择 Python 环境、补全和跳转。[Python](https://marketplace.visualstudio.com/items?itemName=ms-python.python) · [Pylance](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance) · [Pylance 自动导入](https://github.com/microsoft/pylance-release/blob/main/docs/howto/auto-import-guide.md)
- 代码格式、检查和行内提示。[Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) · [Ruff](https://docs.astral.sh/ruff/editors/setup/) · [Error Lens](https://marketplace.visualstudio.com/items?itemName=usernamehw.errorlens)
- 主题、文件图标、窗口颜色、缩进和 Markdown 目录。[One Dark Pro](https://marketplace.visualstudio.com/items?itemName=zhuangtongfa.Material-theme) · [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme) · [Peacock](https://marketplace.visualstudio.com/items?itemName=johnpapa.vscode-peacock) · [indent-rainbow](https://marketplace.visualstudio.com/items?itemName=oderwat.indent-rainbow) · [Markdown All in One](https://marketplace.visualstudio.com/items?itemName=yzhang.markdown-all-in-one)

## Python、Flask 和远程开发

- [Python 虚拟环境](https://docs.python.org/3/library/venv.html) · [VS Code 中选择 Python 环境](https://code.visualstudio.com/docs/python/environments)
- [Flask 安装](https://flask.palletsprojects.com/en/stable/installation/) · [Flask Quickstart](https://flask.palletsprojects.com/en/stable/quickstart/)
- [Remote - SSH](https://code.visualstudio.com/docs/remote/ssh)介绍连接远端、打开文件夹和安装远端扩展。
- [Ports 与端口转发](https://code.visualstudio.com/docs/remote/ssh#_forwarding-a-port--creating-ssh-tunnel)说明如何从本机浏览器访问远端服务。
- [GNU nano 手册](https://www.nano-editor.org/dist/latest/nano.html) · [Vim 入门](https://vimhelp.org/usr_02.txt.html)

## 开源项目如何处理 Issue 与 PR

- [开源的定义](https://opensource.org/osd)
- [什么是 GitHub](https://docs.github.com/en/get-started/start-your-journey/what-is-github)
- [GitHub Issues](https://docs.github.com/en/issues/tracking-your-work-with-issues/learning-about-issues/about-issues)
- [Pull requests](https://docs.github.com/en/pull-requests/reference/pull-requests)


- [VS Code 贡献入口](https://github.com/microsoft/vscode/blob/main/CONTRIBUTING.md) · [贡献指南](https://github.com/microsoft/vscode/wiki/How-to-Contribute)。报 bug 前查重，给出运行环境、复现步骤和预期与实际结果。
- [CPython 的 PR 生命周期](https://devguide.python.org/getting-started/pull-request-lifecycle/)。确认问题、开分支、验证改动和提交 PR。
- [Vite 贡献指南](https://github.com/vitejs/vite/blob/main/CONTRIBUTING.md)。处理 bug 时准备最小复现，讨论功能时先写清楚动机和使用场景。
- [GitHub 如何关联 PR 和 Issue](https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/linking-a-pull-request-to-an-issue)。查看何时可用 `Fixes #编号` 在合入后关闭 Issue。
- Vue 的最小复现、修复和回归测试。[Issue #15495](https://github.com/vuejs/core/issues/15495) · [PR #15498](https://github.com/vuejs/core/pull/15498)
- Flask 的边界用例与修复。[Issue #6093](https://github.com/pallets/flask/issues/6093) · [PR #6096](https://github.com/pallets/flask/pull/6096)

## 环境问题案例

- [Werkzeug Issue #2789](https://github.com/pallets/werkzeug/issues/2789)。Flask 2.2.2 搭配 Werkzeug 3.0.0 时，导入 Flask 就会失败。报告里的三个版本和最小复现帮助维护者定位了兼容性问题。
- [Vite 讨论 #20286](https://github.com/vitejs/vite/discussions/20286) · [Vite 7 的运行时要求](https://vite.dev/blog/announcing-vite7#node-js-support)。新建项目在 Node.js 20.9.0 上报错，Vite 7 官方要求 Node.js 20.19+ 或 22.12+。

## 课后延伸

- [MIT Missing Semester：开发环境与工具](https://missing.csail.mit.edu/2026/development-environment/)
- [Microsoft Learn：VS Code 入门短视频](https://learn.microsoft.com/en-us/shows/visual-studio-code/learn-visual-studio-code-in-7min-official-beginner-tutorial)
