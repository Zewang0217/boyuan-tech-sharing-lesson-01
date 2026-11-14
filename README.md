# 博远技术分享 · 第一课

**开发环境配置与编辑器**

用两个带故障的小游戏练习接手项目。先读任务、复现现象，再用 VS Code 搜索、跨文件跳转、定位并修复。修完后用同一套步骤验证结果。

| 练习 | 场景 | 从这里开始 |
| --- | --- | --- |
| 红灯绿灯反应测试 | 在本机浏览器复现计时问题，沿按钮事件追到回合逻辑 | [项目说明](reaction/README.md) · [练习任务](reaction/ISSUE.md) |
| 服务器猜数字 | 在远程 VS Code 中排查判定逻辑，从本机浏览器验证回复 | [项目说明](guess/README.md) · [练习任务](guess/ISSUE.md) |

在 VS Code 中打开仓库根目录可浏览所有文件。打开 [games.code-workspace](games.code-workspace) 可将两个项目作为独立目录并排展示。

## 课件

[第一课 PPT](materials/开发环境配置与编辑器.pptx)（含演讲者备注） · [逐页讲稿](materials/逐页讲稿.md)

## VS Code 编辑练习

在 VS Code 打开仓库根目录，找到 [test/exercise/editing-practice.js](test/exercise/editing-practice.js)。把内容复制到新建的 JavaScript 编辑器，再练习多光标、上下移行、复制整行、删除整行和格式化。底稿故意保留了错乱的缩进，演示结束后关闭副本即可。

## 运行反应测试

在 VS Code 打开 `reaction/`，再用浏览器打开 [`index.html`](reaction/index.html)。`game.js` 负责界面和点击事件，`round.js` 负责计时与回合。浏览器可直接运行，也可以用 Live Server 预览。

## 运行服务器猜数字

通过 VS Code Remote - SSH 打开演示主机上的 `guess/`。在该目录的 Linux 终端执行以下命令，使用 Python 3.10 或更新版本。

```bash
python3 -m venv .venv
.venv/bin/python -m pip install -r requirements.txt
.venv/bin/python app.py
```

在 VS Code 的 Ports 面板转发远端 `5000`，用浏览器打开面板显示的本地地址。服务每次启动时随机选一个 1 到 100 的整数，运行期间保持同一个谜底。保存服务端代码后，按 `Ctrl+C` 停止旧进程，再启动。要用固定谜底对照修复前后的结果，见[练习任务](guess/ISSUE.md)。

`index.html` 提供表单，`app.py` 处理请求，`guess_rules.py` 负责判定。Flask 监听运行它的那台机器的 `127.0.0.1:5000`。在自己的电脑上练习时，用本机终端启动后可直接访问这个地址。Windows PowerShell 中先执行 `python -m venv .venv`，再执行 `.\.venv\Scripts\python.exe -m pip install -r requirements.txt`，然后运行以下命令。

```powershell
.\.venv\Scripts\python.exe app.py
```

课程涉及的快捷键、扩展、Python 环境和远程开发文档见[参考资料](REFERENCES.md)。
