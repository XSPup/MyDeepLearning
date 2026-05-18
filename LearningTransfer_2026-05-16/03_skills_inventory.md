# 当前 Skills 与插件清单

本文件记录的是 2026-05-16 当前这台机器上可见的 skills / plugins。换电脑后需要重新安装或复制，不能假设自动存在。

## Skill 根目录

| 类型 | 路径 | 说明 |
|---|---|---|
| 当前 Codex skills 入口 | `C:\Users\A\.codex\skills` | 其中多数是 junction，指向 canonical 目录。 |
| 当前 canonical skills | `C:\Users\A\.agent-skills\skills` | 本机主要可复用 skill 存放处。 |
| Codex system skills | `C:\Users\A\.codex\skills\.system` | Codex 自带系统 skill。 |
| DeepSeek skills 入口 | `C:\Users\A\.deepseek\skills` | DeepSeek TUI 当前也能看到 44 个 skill。 |
| 当前 guide 副本 | `reference_docs/SKILLS_GUIDE_current_machine.md` | 已复制进本迁移包。 |

## 当前启用插件

| 插件 | 用途 |
|---|---|
| Browser Use | 在 Codex 内置浏览器中打开、测试、截图本地网页或远程页面。 |
| Canva | 搜索、创建、编辑 Canva 设计。 |
| GitHub | 查看仓库、issue、PR、CI，并可辅助发 PR。 |
| Linear | 管理 Linear issue、项目和团队流程。 |
| Zotero | 连接 Zotero Desktop，搜索文献库、导出 BibTeX、插入引用。 |

插件状态通常依赖账号连接和本机安装，新电脑需要重新登录或重新启用。

## Codex system skills

| Skill | 用途 |
|---|---|
| `imagegen` | 生成或编辑位图图像。 |
| `openai-docs` | 查询 OpenAI 官方 API / 产品文档。 |
| `plugin-creator` | 创建本地 Codex plugin 结构。 |
| `skill-creator` | 创建或更新 Codex skill。 |
| `skill-installer` | 从 curated 列表或 GitHub 安装 skill。 |

## 本机 canonical skills

| Skill | 用途 |
|---|---|
| `abstract-checker` | 检查摘要是否忠实反映论文正文。 |
| `bibliography-checker` | 检查引用、参考文献和未支撑声明。 |
| `brainstorming` | 功能、组件、行为修改前的需求和设计澄清。 |
| `code-review` | 审查代码 diff、PR、bug、回归、安全和测试风险。 |
| `code-simplifier` | 在保持行为的前提下简化最近修改的代码。 |
| `dispatching-parallel-agents` | 将独立任务拆分给并行 agent。 |
| `executing-plans` | 按已有实施计划执行。 |
| `figma` | 从 Figma 获取设计上下文并转成代码。 |
| `finishing-a-development-branch` | 开发完成后做合并、PR 或清理决策。 |
| `long-horizon-agent` | 组织长时间、可恢复、带里程碑和验证的任务。 |
| `mcp-builder` | 构建 MCP server 和工具。 |
| `nature-citation` | 为 Nature/CNS 级写作寻找和导出支撑引用。 |
| `nature-data` | 准备 Nature 数据可用性声明和 FAIR 数据计划。 |
| `nature-figure` | 制作或审查 Nature 风格科学图。 |
| `nature-paper2ppt` | 从论文生成中文学术 PPT。 |
| `nature-polishing` | 把学术文字润色成 Nature 风格英文。 |
| `nature-reader` | 从论文 PDF/DOI/arXiv 生成双语、带图、可追溯 Markdown。 |
| `nature-response` | 写审稿意见逐点回复。 |
| `pdf` | 阅读、渲染、生成、检查 PDF。 |
| `planning-with-files` | 用 `task_plan.md`、`findings.md`、`progress.md` 做持久计划。 |
| `pptx` | 创建、读取、编辑、合并 PowerPoint。 |
| `ralph-loop` | 有明确完成标准时的自主迭代执行。 |
| `receiving-code-review` | 接收代码审查意见时先验证再改。 |
| `replication-archive` | 审查或构建研究复现包。 |
| `requesting-code-review` | 完成大改动后请求审查。 |
| `research-writing` | 研究设计、论文结构、摘要、引言、讨论等写作。 |
| `review-paper-code` | 审查论文代码的可复现性和逻辑一致性。 |
| `r-refactor` | 重构 R / ggplot / tidyverse 研究代码。 |
| `sci-figure-maker` | 生成可编辑科学图，优先 SVG/PDF/EPS/TikZ 和源脚本。 |
| `skill-creator` | 创建或更新通用 skill。 |
| `statistical-reviewer` | 审查统计方法、假设、证据强度和因果表述。 |
| `structural-editor` | 审查学术段落和章节结构。 |
| `subagent-driven-development` | 用子 agent 执行独立开发任务。 |
| `systematic-debugging` | 遇到 bug 或失败时系统诊断。 |
| `test-driven-development` | 写功能或修 bug 前先写测试。 |
| `top3-reviewer` | 以顶会/顶刊审稿标准检查贡献和逻辑。 |
| `ui-ux-pro-max` | Web / mobile UI/UX 设计和前端改进。 |
| `using-git-worktrees` | 用 git worktree 隔离功能开发。 |
| `using-superpowers` | Superpowers 元工作流，指导何时用其他 workflow skill。 |
| `verification-before-completion` | 在声称完成前运行验证命令并看输出。 |
| `webapp-testing` | 用浏览器/Playwright 思路验证 Web app。 |
| `writing-editor` | 编辑学术和技术文字的清晰度、语气和流畅度。 |
| `writing-plans` | 写实施计划。 |
| `writing-skills` | 编写、修改和验证 reusable skills。 |

## 插件贡献的 skills

| Skill | 插件 | 用途 |
|---|---|---|
| `browser-use:browser` | Browser Use | 操作 Codex 内置浏览器，尤其适合 localhost 和 file URL。 |
| `canva:canva-branded-presentation` | Canva | 根据 brief 或 outline 创建品牌化 Canva 演示文稿。 |
| `canva:canva-resize-for-all-social-media` | Canva | 把 Canva 设计批量改成社交媒体尺寸。 |
| `canva:canva-translate-design` | Canva | 翻译 Canva 设计文字并尽量保持布局。 |
| `github:github` | GitHub | 通用 GitHub 仓库、PR、issue 定向和摘要。 |
| `github:gh-address-comments` | GitHub | 处理 PR review comment。 |
| `github:gh-fix-ci` | GitHub | 调试和修复 GitHub Actions CI。 |
| `github:yeet` | GitHub | 提交本地改动、推送并开 draft PR。 |
| `linear:linear` | Linear | 读写 Linear tickets 和项目。 |
| `zotero:Zotero` | Zotero | 操作 Zotero Desktop 本地文献库和 BibTeX。 |

## 新电脑迁移建议

如果只想让新电脑“理解我们在做什么”，这个交接包已经够用。  
如果想让新电脑拥有同样的 skill 能力，还需要额外迁移或重装：

```text
C:\Users\A\.agent-skills\skills
C:\Users\A\.codex\skills\.system
C:\Users\A\.codex\plugins\cache
```

更保守的做法是在新电脑上重新安装 Codex / 插件 / skills，然后把本文件和 `reference_docs/SKILLS_GUIDE_current_machine.md` 作为对照。

