# 新电脑恢复清单

## 1. 解压工作区

建议把压缩包解压到类似路径：

```powershell
D:\MyDeepLearning
```

如果盘符不同也可以，但新电脑上的 agent 要先读本迁移包里的相对路径说明。

## 2. 创建 Python 虚拟环境

不要复制旧电脑 `.venv`。在新电脑重新创建：

```powershell
cd /d D:\MyDeepLearning
py -3.13 -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r LearningTransfer_2026-05-16\requirements_transfer.txt
```

如果新电脑没有 Python 3.13，也可以先用已安装的 Python 3.12/3.13 创建环境；深度学习包如果安装失败，再根据新电脑 CPU/GPU 和 PyTorch 官网命令调整。

## 3. 检查环境

```powershell
.\.venv\Scripts\python.exe --version
.\.venv\Scripts\python.exe -c "import torch, torchvision; print(torch.__version__, torchvision.__version__)"
```

CPU-only 学习 MNIST 是可以的，不必为了入门强制装 CUDA。

## 4. Node / DeepSeek TUI

旧电脑环境：

```text
Node v22.17.0
npm 10.9.2
deepseek-tui v0.8.28
default model: deepseek-v4-flash
context_window: 1000000
```

新电脑如需 DeepSeek TUI：

```powershell
npm i -g deepseek-tui
deepseek --version
deepseek setup --tools --plugins
deepseek auth set --provider deepseek
deepseek config set default_text_model deepseek-v4-flash
deepseek --model deepseek-v4-flash doctor --json
```

注意：`deepseek auth set --provider deepseek` 需要你自己输入 API key。不要从旧电脑复制或公开 API key。

## 5. Codex / skills

新电脑上先让 agent 读取：

```text
LearningTransfer_2026-05-16\03_skills_inventory.md
LearningTransfer_2026-05-16\reference_docs\SKILLS_GUIDE_current_machine.md
```

如果缺少某个 skill，优先按新电脑 Codex 的安装方式重新安装。只有在确认目录结构兼容时，才复制旧电脑的完整 skills 目录。

## 6. 继续学习时的第一条指令

可以对新电脑 agent 说：

```text
请先读取 D:\MyDeepLearning\LearningTransfer_2026-05-16\05_AGENT_START_HERE_PROMPT.md，然后按里面的学习模式继续。先不要写完整项目，只确认当前文件状态，并告诉我下一小步。
```

