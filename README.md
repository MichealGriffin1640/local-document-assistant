mg1640-local-document-assistant

这是一个简单的 MCP（Model Context Protocol）本地文档助手示例，安装并运行后，它会在终端输出一句话：“Hello from mg1640-local-document-assistant!”
本教程将一步一步教你从零开始安装并运行这个程序，即使你完全没有 Python 经验也能成功。
1. 安装 Python
首先需要确保你的电脑上安装了 Python 3.8 及以上版本。
Windows 用户
打开 Python 官方下载页面
下载最新的 Windows installer
安装时务必勾选 "Add Python to PATH" 选项，然后点击 Install
macOS 用户
打开终端（Terminal）输入：
`brew install python`
Linux 用户（Debian/Ubuntu）
`sudo apt update`
`sudo apt install python3 python3-pip`
安装完成后，打开终端输入：
`python3 --version`
看到版本号（例如 Python 3.11.5）就说明安装成功。注意：本版本使用python版本为3.10

2. 安装 uv
uv 是一个快速的 Python 包管理工具，比传统的 pip 更高效。
安装命令（跨平台）：
`curl -LsSf https://astral.sh/uv/install.sh | sh`
Windows 用户（PowerShell）：
`powershell -c "irm https://astral.sh/uv/install.ps1 | iex"`
验证是否安装成功：
`uv --version`

3. 克隆本项目代码
在终端中运行：
`git clone https://github.com/hacimi/mg1640-local-document-assistant.git`
`cd mg1640-local-document-assistant`
如果没有安装 Git，可以先参考：https://git-scm.com/downloads

4. 使用 uv 创建虚拟环境
在项目目录下执行：
`uv venv`
这样会创建一个隔离的 Python 环境，避免污染系统。

5. 安装依赖
`uv pip install .`
这会根据 pyproject.toml 中的配置安装你的 MCP 包。

6. 运行程序
安装完成后，直接运行命令：
`mg1640-local-document-assistant`
你将会看到输出：
`Hello from mg1640-local-document-assistant!`
