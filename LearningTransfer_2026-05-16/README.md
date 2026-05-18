# MyDeepLearning 迁移交接包

生成时间：2026-05-16  
原工作区：`D:\MyDeepLearning`  
用途：把当前学习目标、计划、进度、技能清单和恢复步骤带到另一台电脑。

## 先读顺序

1. `05_AGENT_START_HERE_PROMPT.md`  
   给新电脑上的 Codex / DeepSeek / 其他 agent 看的启动提示词。
2. `01_learning_goal_plan_progress.md`  
   我们的总体目标、8 个月学习路线、未来网络 + AI 研究方向，以及当前进度。
3. `02_resume_points_and_known_gaps.md`  
   现在可以从哪里继续，以及当前工作区和旧记忆之间的差异。
4. `03_skills_inventory.md`  
   当前这台机器可用的 skills、插件、skill 根目录和迁移建议。
5. `04_new_computer_setup_checklist.md`  
   新电脑重建环境的命令清单。
6. `reference_docs/`  
   已复制进来的关键原始文档副本。

## 已包含的参考文档

- `reference_docs/future_network_ai_github_projects.md`
- `reference_docs/ML_DL_8_Month_Learning_Plan.md`
- `reference_docs/SKILLS_GUIDE_current_machine.md`

## 不建议直接打包迁移的内容

- `.venv/`：虚拟环境应在新电脑重新创建。
- `C:\Users\A\.deepseek\config.toml`：里面涉及本机配置和 API key 来源，不要直接分享或上传。
- API key、账号凭据、浏览器登录态：在新电脑重新登录或重新执行认证命令。

## 当前最重要的学习原则

我们不是让 agent 直接把学习项目做完，而是按教程式节奏推进：一次只给一个小步骤，用户自己写代码，agent 给解释、检查输出、保存 checkpoint。

