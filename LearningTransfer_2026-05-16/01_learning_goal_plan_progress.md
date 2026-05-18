# 学习目标、计划与当前进度

## 总体目标

长期目标是从机器学习基础逐步进入深度学习和未来网络 + AI 研究实践。当前学习不是只看课程，而是边学边做可复现、可扩展的开源项目，最终形成可以用于论文选题、实验复现和个人作品集的项目线。

## 8 个月学习路线

主计划文件：`reference_docs/ML_DL_8_Month_Learning_Plan.md`

阶段安排：

| 阶段 | 主题 | 目标 |
|---|---|---|
| Month 1 | 传统 ML 基础闭环 | 理解数据、训练、验证、误差、简单模型。 |
| Month 2 | sklearn、树模型、分类项目 | 能完成一个完整分类项目并解释结果。 |
| Month 3 | 数据处理、特征工程、无监督学习 | 能独立处理表格数据和聚类/降维任务。 |
| Month 4 | 神经网络基础 | 从线性模型过渡到神经网络表达。 |
| Month 5 | PyTorch 系统入门 | 掌握 Dataset、DataLoader、模型、loss、optimizer、训练循环。 |
| Month 6 | CNN、序列模型、实验管理 | 进入图像/序列任务和实验记录。 |
| Month 7 | Attention、Transformer、NLP 入门 | 理解注意力机制和现代 DL 架构。 |
| Month 8 | 综合项目与作品集 | 做出一个未来网络 + AI 方向的可展示项目。 |

## 研究方向主线

主规划文件：`reference_docs/future_network_ai_github_projects.md`

当前推荐的未来网络 + AI 方向：

| 方向 | 为什么适合 |
|---|---|
| GNN 网络数字孪生 + RL 路由优化 | 有明确图结构，适合做论文式实验和消融。 |
| 算力网络切片与边缘计算联合编排 | 贴近算力网络和任务调度，和近期网络研究方向匹配。 |
| O-RAN xApp 异常检测与自智运维 | 更接近系统和运维智能化，容易形成 demo。 |
| ICN / CDN 内容缓存智能优化 | 任务边界清晰，适合做强化学习或预测缓存策略。 |
| 网络遥测基础模型与电信 LLM 微调 | 更前沿，但对数据和算力要求更高，适合作为后期扩展。 |

## 当前已有项目

| 项目 | 路径 | 当前定位 |
|---|---|---|
| 简单线性回归 notebook | `OpenSourceProjectPractice\simple-linear-regression-notebook` | 入门回归项目，适合复习最小二乘和 notebook 环境。 |
| Iris KNN from scratch | `OpenSourceProjectPractice\iris-knn-from-scratch` | 手写 KNN 入门，适合练习距离函数、预测函数、准确率计算。 |
| Interactive Neuron Demo | `OpenSourceProjectPractice\interactive-neuron-demo` | 浏览器打开的单神经元可视化，用于理解权重、偏置、sigmoid。 |

## 当前学习工作方式

- 一次只推进一个小步骤。
- 用户自己写代码，agent 只给下一步、解释和检查。
- 每个阶段要有可验证输出，例如脚本运行结果、loss 值、accuracy 或截图。
- 重要 checkpoint 要写入文件，避免换电脑或换会话后丢失进度。

## 最近最应该继续的任务

如果目标是继续深度学习入门，优先恢复 MNIST / PyTorch 练习。当前记忆中的下一步是：在已能产生 `logits shape = torch.Size([64, 10])` 的基础上，加 `CrossEntropyLoss` 和 `Adam`，计算第一批数据的 `initial loss`。

但当前磁盘未找到 MNIST 项目文件，所以新电脑上应先做两件事：

1. 确认压缩包里是否有 `mnist-digit-recognition` 或 `mnist-from-scratch-guide.md`。
2. 如果没有，就按 `02_resume_points_and_known_gaps.md` 的 checkpoint 重建。

