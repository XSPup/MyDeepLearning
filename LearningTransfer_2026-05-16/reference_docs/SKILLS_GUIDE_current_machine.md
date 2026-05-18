# Shared Agent Skills Guide

Canonical skills directory:

```text
C:\Users\A\.agent-skills\skills
```

Entry directories:

```text
C:\Users\A\.codex\skills
C:\Users\A\.deepseek\skills
C:\Users\A\.claude\skills
```

The entry directories use Windows junctions that point to the canonical directory. Install or edit skills in the canonical directory first, then add junctions for any agent-specific entry directory if needed.

## How To Invoke

Use natural language plus the skill name:

```text
Use $planning-with-files to plan this task before editing.
Use $ui-ux-pro-max to redesign this frontend.
Use $code-review to review my current diff.
Use $webapp-testing to verify the app in a browser.
```

If an agent does not support `$skill-name`, say:

```text
Read C:\Users\A\.agent-skills\skills\<skill-name>\SKILL.md and follow that workflow.
```

## Top 10 Mapping From The Screenshot

| Screenshot name | Installed skill(s) | What it does | Typical use |
|---|---|---|---|
| Superpowers | `using-superpowers` plus `brainstorming`, `writing-plans`, `test-driven-development`, `systematic-debugging`, `verification-before-completion`, and related Superpowers skills | Structured software-development workflows from brainstorming through TDD, implementation, review, and verification | "Use $using-superpowers and $test-driven-development to build this feature." |
| Planning with Files | `planning-with-files` | Stores task plans, findings, and progress in markdown files so context survives long sessions | "Use $planning-with-files before starting this multi-step migration." |
| UI UX Pro Max | `ui-ux-pro-max` | Frontend/product design guidance with many style directions, palettes, and UX rules | "Use $ui-ux-pro-max to make this dashboard feel more polished." |
| Code Review | `code-review`, plus Superpowers `requesting-code-review` and `receiving-code-review` | Review diffs for bugs, regressions, security, tests, and confidence-ranked findings | "Use $code-review on my current changes." |
| Code Simplifier | `code-simplifier` | Simplifies recently changed code while preserving behavior | "Use $code-simplifier on the files I just edited." |
| Webapp Testing | `webapp-testing` | Uses browser/Playwright-style checks for frontend flows, screenshots, console errors, and regressions | "Use $webapp-testing to verify the checkout flow." |
| Ralph Loop | `ralph-loop` | Sets up autonomous iterative execution with clear completion criteria and verification gates | "Use $ralph-loop only after we have binary pass/fail criteria." |
| MCP Builder | `mcp-builder` | Guides creation of Model Context Protocol servers and tools | "Use $mcp-builder to create an MCP server for this API." |
| PPTX | `pptx` | Creates, reads, edits, combines, and analyzes PowerPoint decks | "Use $pptx to generate a 10-slide deck from this outline." |
| Skill Creator | `skill-creator`, plus Superpowers `writing-skills` | Creates and improves skills with valid `SKILL.md` structure | "Use $skill-creator to make a reusable workflow skill." |

## Full Inventory

| Skill | Role | Use when |
|---|---|---|
| `abstract-checker` | Checks abstract faithfulness against the paper body | Reviewing or drafting abstracts from a manuscript |
| `bibliography-checker` | Audits citations, bibliography entries, and claim support | Checking `.bib` files, missing references, or citation accuracy |
| `brainstorming` | Superpowers ideation workflow | Designing features, workflows, APIs, or components before implementation |
| `code-review` | Local adapted code review workflow | Reviewing diffs, PRs, security risks, tests, and regressions |
| `code-simplifier` | Local adapted simplification/refactor workflow | Reducing duplication, nesting, and complexity after implementation |
| `dispatching-parallel-agents` | Superpowers parallel-work planning | Splitting independent tasks across agents or workstreams |
| `executing-plans` | Superpowers plan execution | Executing an already written plan step by step |
| `figma` | Figma design-to-code workflow | Reading Figma context, screenshots, variables, and assets |
| `finishing-a-development-branch` | Superpowers branch wrap-up | Checking a completed branch before merge or handoff |
| `long-horizon-agent` | Durable long-task control plane | Creating `prompt.md`, `plans.md`, `implement.md`, and `documentation.md` for long runs |
| `mcp-builder` | Official MCP server-building guide | Building MCP tools, resources, prompts, or integration servers |
| `nature-citation` | Nature/CNS citation workflow | Finding, validating, and exporting supporting citations |
| `nature-data` | Nature data availability and FAIR workflow | Writing Data Availability statements or repository plans |
| `nature-figure` | Nature-style scientific figures | Creating polished multi-panel figures and journal-ready plots |
| `nature-paper2ppt` | Paper-to-PPT workflow | Turning a scientific paper into a Chinese presentation deck |
| `nature-polishing` | Nature-style academic English polishing | Polishing abstracts, introductions, results, discussions, and Chinese drafts |
| `nature-reader` | Bilingual paper reading workflow | Building source-grounded Markdown reading notes from papers |
| `nature-response` | Reviewer-response workflow | Drafting point-by-point responses to reviewers and editors |
| `pdf` | PDF reading, rendering, extraction, and generation | Working with PDFs where layout matters |
| `planning-with-files` | Persistent markdown planning | Managing complex tasks with `task_plan.md`, `findings.md`, and `progress.md` |
| `pptx` | PowerPoint creation and editing | Creating, parsing, editing, combining, or summarizing `.pptx` decks |
| `ralph-loop` | Autonomous loop protocol | Running iterative tasks with explicit success criteria and verification gates |
| `receiving-code-review` | Superpowers review intake | Handling reviewer comments without blindly applying bad suggestions |
| `replication-archive` | Reproducibility package workflow | Building or auditing paper replication archives |
| `requesting-code-review` | Superpowers review request workflow | Asking another agent or reviewer to inspect completed work |
| `research-writing` | Academic research writing workflow | Structuring papers, abstracts, introductions, related work, and experiments |
| `review-paper-code` | Research-code review | Checking paper code for reproducibility and paper-to-code consistency |
| `r-refactor` | R/ggplot research-code refactor | Cleaning R scripts, Quarto/R Markdown, tidyverse pipelines, or figures |
| `sci-figure-maker` | Editable scientific figure generation | Creating SVG/PDF/EPS/PGFPlots/TikZ scientific figures |
| `skill-creator` | Skill creation guide | Creating or updating reusable agent skills |
| `statistical-reviewer` | Statistical-methods review | Checking p-values, confidence intervals, causal claims, ablations, and evidence strength |
| `structural-editor` | Academic structure editing | Reviewing section order, paragraph logic, and transitions |
| `subagent-driven-development` | Superpowers subagent execution | Executing independent implementation tasks with specialized agents |
| `systematic-debugging` | Superpowers debugging workflow | Diagnosing bugs, test failures, and unexpected behavior systematically |
| `test-driven-development` | Superpowers TDD workflow | Writing tests before implementation for features and bug fixes |
| `top3-reviewer` | Harsh top-tier paper review | Checking novelty, contribution, framing, and reviewer objections |
| `ui-ux-pro-max` | High-polish UI/UX design guidance | Designing or revising frontend interfaces, landing pages, dashboards, and mobile UI |
| `using-git-worktrees` | Superpowers worktree workflow | Isolating risky or parallel feature work in Git worktrees |
| `using-superpowers` | Superpowers meta skill | Starting coding work with Superpowers workflow discovery |
| `verification-before-completion` | Superpowers completion gate | Verifying claims before saying work is done |
| `webapp-testing` | Web app browser testing | Running or designing Playwright-style frontend verification |
| `writing-editor` | Academic/technical prose editing | Improving clarity, flow, and accessibility of prose |
| `writing-plans` | Superpowers planning workflow | Writing implementation plans before code changes |
| `writing-skills` | Superpowers skill-authoring workflow | Writing, editing, or verifying reusable skills |

## Notes For Agents

- Prefer the most specific skill that fits the task.
- Do not stack many skills unless each one contributes a distinct workflow.
- For coding tasks, combine `planning-with-files` or `long-horizon-agent` with `verification-before-completion` when the task is long or risky.
- For frontend tasks, use `ui-ux-pro-max` for design direction and `webapp-testing` for browser verification.
- For research-paper tasks, choose the Nature/research skills before generic writing skills.
- `ralph-loop` is powerful but should only be used with clear pass/fail criteria and iteration limits.
- `code-review` and `code-simplifier` are local-adapted skills, not Anthropic-hosted services.
