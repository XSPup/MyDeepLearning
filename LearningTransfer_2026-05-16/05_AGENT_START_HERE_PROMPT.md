# 给新电脑 Agent 的启动提示词

你正在接手 `MyDeepLearning` 学习工作区。请先阅读以下文件，再行动：

```text
LearningTransfer_2026-05-16\README.md
LearningTransfer_2026-05-16\01_learning_goal_plan_progress.md
LearningTransfer_2026-05-16\02_resume_points_and_known_gaps.md
LearningTransfer_2026-05-16\03_skills_inventory.md
LearningTransfer_2026-05-16\04_new_computer_setup_checklist.md
```

然后核对这些参考文档：

```text
LearningTransfer_2026-05-16\reference_docs\ML_DL_8_Month_Learning_Plan.md
LearningTransfer_2026-05-16\reference_docs\future_network_ai_github_projects.md
LearningTransfer_2026-05-16\reference_docs\SKILLS_GUIDE_current_machine.md
```

## 用户学习偏好

- 用户是在学习，不希望 agent 直接替他完成项目。
- 一次只给一个小步骤，然后给明确验证方式。
- 代码练习需要解释性注释，方便以后回看。
- 每个阶段结束要保存 checkpoint。
- 遇到环境问题先实际检查本机状态，不要从假设回答。
- 如果当前文件和记忆不一致，先说明差异，再给恢复方案。

## 当前主线

长期路线：8 个月 ML 到 DL 学习计划。  
研究方向：未来网络 + AI，可延伸到 GNN 路由、数字孪生、算力网络、O-RAN 异常检测、ICN 缓存、电信 LLM。  
当前最实际的下一步：恢复或重建 MNIST / PyTorch 入门练习。

## MNIST 记忆 checkpoint

旧记忆显示用户已经做到：

```text
logits shape = torch.Size([64, 10])
```

下一步不是完整训练循环，而是：

1. 添加 `CrossEntropyLoss`
2. 添加 `Adam`
3. 对第一批 batch 计算 loss
4. 打印 `initial loss`
5. 确认输出后再进入训练循环

但 2026-05-16 当前工作区没有找到 MNIST 项目文件，所以你必须先在新电脑上搜索或确认是否已随压缩包迁移。如果没有，就从这个 checkpoint 重建最小项目。

## 第一轮响应建议

请先做只读检查：

```powershell
Get-ChildItem -LiteralPath 'D:\MyDeepLearning' -Force
Get-ChildItem -LiteralPath 'D:\MyDeepLearning\LearningTransfer_2026-05-16' -Force
Get-ChildItem -LiteralPath 'D:\MyDeepLearning\OpenSourceProjectPractice' -Force
```

然后告诉用户：

- 当前工作区是否完整。
- MNIST 项目是否存在。
- 下一小步是什么。

