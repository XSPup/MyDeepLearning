# 恢复点与已知差异

## 可以直接继续的内容

### 8 个月计划

从 `reference_docs/ML_DL_8_Month_Learning_Plan.md` 继续。这个文件是长期路线图，不依赖本机环境。

### 未来网络 + AI 项目规划

从 `reference_docs/future_network_ai_github_projects.md` 继续。这个文件已经包含候选仓库、优先路线和开源学习材料替代方案。

### 已存在练习项目

可继续检查这些目录：

```text
D:\MyDeepLearning\OpenSourceProjectPractice\simple-linear-regression-notebook
D:\MyDeepLearning\OpenSourceProjectPractice\iris-knn-from-scratch
D:\MyDeepLearning\OpenSourceProjectPractice\interactive-neuron-demo
```

迁移到新电脑后路径可能不同，但相对路径应保持一致。

## MNIST checkpoint

这是来自旧记忆的学习进度：

- 项目名：`mnist-digit-recognition`
- 原记忆路径：`D:\MyDeepLearning\OpenSourceProjectPractice\mnist-digit-recognition`
- 练习方式：用户自己写代码，agent 一步一步指导。
- 已验证内容：
  - Python `.venv`
  - `torch`
  - `torchvision`
  - MNIST 数据加载
  - `DataLoader`
  - `SmallCNN`
  - 一批输入通过模型后输出：`logits shape = torch.Size([64, 10])`
- 下一步：
  - 添加 `nn.CrossEntropyLoss()`
  - 添加 `torch.optim.Adam(model.parameters(), lr=...)`
  - 取第一批 batch，计算 `loss = criterion(logits, labels)`
  - 打印 `initial loss`
  - 暂时不要直接写完整训练循环，先验证 loss 能正常计算。

## 当前磁盘差异

2026-05-16 核对当前 `D:\MyDeepLearning` 时，没有找到：

```text
D:\MyDeepLearning\OpenSourceProjectPractice\mnist-digit-recognition
D:\MyDeepLearning\OpenSourceProjectPractice\mnist-from-scratch-guide.md
train.py
```

这意味着新电脑继续时要先判断：这些文件是没打包、被移动、还是之前没有持久保存。不要假设 MNIST 项目已经存在。

## 如果需要重建 MNIST 项目

建议新电脑上的 agent 按这个节奏继续：

1. 建立目录：`OpenSourceProjectPractice\mnist-digit-recognition`
2. 建立最小文件：`README.md`、`requirements.txt`、`train.py`
3. 只先写到能完成一批数据前向传播：
   - import
   - argparse
   - Dataset / DataLoader
   - `SmallCNN`
   - 打印 `logits shape`
4. 然后继续本 checkpoint 的下一步：loss + optimizer + `initial loss`

## 不要做的事

- 不要让 agent 一次性写完整 MNIST 项目。
- 不要跳过 checkpoint。
- 不要把 `.venv` 当作迁移内容。
- 不要把 API key、DeepSeek 配置或浏览器登录态打包。

