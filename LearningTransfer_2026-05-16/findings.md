# Findings

## 当前工作区

- 根目录：`D:\MyDeepLearning`
- 当前存在的顶层目录：`.venv`、`LearningNotes`、`OpenSourceProjectPractice`、`ResearchPlanning`、`ScratchNotebooks`、`ScratchScripts`、`.obsidian`、`.ipynb_checkpoints`
- 关键规划文档存在：
  - `D:\MyDeepLearning\ResearchPlanning\ML_DL_8_Month_Learning_Plan.md`
  - `D:\MyDeepLearning\ResearchPlanning\future_network_ai_github_projects.md`

## 学习主线

- 8 个月从 ML 到 DL：传统 ML、sklearn、特征工程、神经网络基础、PyTorch、CNN/序列模型、Attention/Transformer、综合项目。
- 研究方向主线：未来网络 + AI，重点候选包括 GNN/数字孪生路由、算力网络切片和边缘计算、O-RAN xApp 异常检测、ICN/CDN 缓存优化、电信 LLM/遥测基础模型。

## 已有练习项目

- `OpenSourceProjectPractice\simple-linear-regression-notebook`
- `OpenSourceProjectPractice\iris-knn-from-scratch`
- `OpenSourceProjectPractice\interactive-neuron-demo`

## MNIST 状态差异

记忆中记录过一个 MNIST 练习 checkpoint：已做到 `SmallCNN` 前向传播并打印 `logits shape = torch.Size([64, 10])`，下一步是 `CrossEntropyLoss`、`Adam`、打印第一批 `initial loss`。  
但当前磁盘搜索没有找到 `D:\MyDeepLearning\OpenSourceProjectPractice\mnist-digit-recognition`、`mnist-from-scratch-guide.md` 或 `train.py`。新电脑继续时应先重新定位该项目；如果确实不存在，就按 `02_resume_points_and_known_gaps.md` 从 checkpoint 重建。

## 当前环境快照

- Python：`3.13.5`，来自 `D:\MyDeepLearning\.venv\Scripts\python.exe`
- 关键 Python 包：
  - `torch==2.11.0`
  - `torchvision==0.26.0`
  - `matplotlib==3.10.9`
  - `numpy==2.4.4`
  - `pillow==12.2.0`
  - `tqdm==4.67.3`
- Node：`v22.17.0`
- npm：`10.9.2`
- DeepSeek TUI：`v0.8.28`
- DeepSeek 默认模型：`deepseek-v4-flash`
- DeepSeek 当前模型能力：`context_window: 1000000`

