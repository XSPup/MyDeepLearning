# Package Manifest

## 交接包内文件

| 文件 | 作用 |
|---|---|
| `README.md` | 总入口和阅读顺序。 |
| `task_plan.md` | 本次生成迁移包的计划和决策。 |
| `findings.md` | 当前核对到的事实。 |
| `progress.md` | 本次操作记录。 |
| `01_learning_goal_plan_progress.md` | 学习目标、计划、研究方向和当前进度。 |
| `02_resume_points_and_known_gaps.md` | 恢复点和已知差异，尤其是 MNIST。 |
| `03_skills_inventory.md` | 当前 skills、plugins 和迁移建议。 |
| `04_new_computer_setup_checklist.md` | 新电脑恢复命令和检查清单。 |
| `05_AGENT_START_HERE_PROMPT.md` | 给新电脑 agent 的启动提示词。 |
| `requirements_transfer.txt` | 新电脑重建 Python 环境的基础依赖。 |
| `reference_docs\future_network_ai_github_projects.md` | 未来网络 + AI 项目规划副本。 |
| `reference_docs\ML_DL_8_Month_Learning_Plan.md` | 8 个月学习计划副本。 |
| `reference_docs\SKILLS_GUIDE_current_machine.md` | 当前机器 skills guide 副本。 |

## 没有放进交接包的内容

| 内容 | 原因 |
|---|---|
| `.venv` | 体积大且不可跨电脑可靠迁移，应重建。 |
| DeepSeek API key / config | 包含本机认证信息或密钥来源，不应打包。 |
| 完整 `C:\Users\A\.agent-skills\skills` | 可能较大且路径依赖，新电脑建议重装；如需完整能力再单独复制。 |
| 浏览器登录态 / 插件账号连接 | 需要在新电脑重新登录。 |

