---
title: Agentic Engineering Patterns 总结
published: 2026-03-04T19:24:00.000+08:00
updated: 2026-03-04T19:24:00.000+08:00
description: Agentic Engineering Patterns 学习总结
cover: https://picsum.photos/800/600?random=3
tags:
  - Agent
category: Agent
draft: false
---
今日分享 Django 之父、AI 时代最值得关注的独立技术博主，Simon Willison最近发布的博客

📖 Agentic Engineering Patterns

作者：Simon Willison | 2026年2月发布

👉 原文：simonwillison.net/guides/agentic-engineering-patterns/

这是一套专门针对 Claude Code、OpenAI Codex 等 AI 编程 Agent 的实战工程模式指南，共 6 个核心模式：

1. 💰 Writing Code is Cheap Now（写代码变便宜了）

现在让 Agent 写代码的成本极低，不要犹豫，大胆让它写。

核心思想：不要把 AI 当搜索引擎用，直接让它干活。

2. 🗃️ Hoard Things You Know How To Do（把你会的东西存起来）

把常用的 prompt、脚本、操作流程积累下来复用。

核心思想：把 Agent 的成功经验沉淀成可复用的资产（比如 SKILL.md、AGENTS.md）——这和 OpenClaw 的 skill 体系思路完全一致！

3. 🔴🟢 Red/Green TDD（测试驱动开发）

先让 Agent 写失败的测试（红），再写实现让测试通过（绿）。

核心思想：用测试约束 Agent 行为，避免它乱改代码。

4. ✅ First Run the Tests（先跑测试）

开始一个新 Agent 会话时，先让它跑一遍现有测试。

核心思想：测试是 Agent 理解现有代码的最佳切入点，Agent 天然倾向于阅读测试文件来理解代码。

5. 🚶 Linear Walkthroughs（线性代码漫游）

让 Agent 从头到尾给你讲解一个代码库。

核心思想：当你接手陌生代码，或自己 vibe coded 完全忘了怎么回事时，让 Agent 做一个结构化讲解。

6. 💬 Interactive Explanations（交互式解释）

不要只是读文档，让 Agent 边解释边回答你的追问。

核心思想：把 Agent 当成一个能被追问的导师，而不是文档生成器。

总结一句话： 这篇文章的核心是——把 AI Agent 当真正的工程伙伴来用，而不是一个高级补全工具。积累 prompt、用测试约束、让它主动理解代码，是提升效果的关键。
