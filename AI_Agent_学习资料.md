# AI Agent 学习计划 · 配套资料清单

> 浅浅 · 配套《AI_Agent_学习计划.md》使用 · 2026-09-28
> **用法：每层只跟一个主线资源，别同时开三本书。** 标了「主线」的是默认教材，「选读」是深挖时再看。
> 英文材料看不懂就先找中文翻译或 B 站搬运，不必硬啃原版。

---

## 第 2 层 · 模型层 · 理解 LLM

| 资料 | 说明 | 用法 |
|---|---|---|
| **Karpathy《Intro to Large Language Models》**（1 小时科普） | YouTube 原版：`youtube.com/watch?v=zjkBMFhNj_g`；B 站有中英字幕版（BV1AU421o7ob） | **主线 · 开场第一个看**。把"LLM 是什么"一次讲透，无数学 |
| **3Blue1Brown《But what is a GPT?》系列** | B 站有官方中文版 | 注意力机制的最佳直觉来源，全是可视化 |
| **Jay Alammar《The Illustrated Transformer》** | 搜"jalammar illustrated transformer" | 图解注意力经典文，配合 3B1B 看 |
| 论文《Lost in the Middle》（Liu et al., 2023） | 搜标题可下 PDF | 想搞懂"上下文中间遗忘"的证据时读 |
| Hugging Face LLM Course 第 1–2 章 | `huggingface.co/learn/llm-course`（有简体中文版：`huggingface.co/course/zh-CN/`） | 选读。想动手跑模型时用 |
| 李沐《动手学深度学习》（d2l.ai） | 中文免费在线书 | 选读。只有想往下挖数学时再看，现阶段不必 |

---

## 第 3 层 · 交互层 · 让模型动手

| 资料 | 说明 | 用法 |
|---|---|---|
| **Datawhale《llm-cookbook》** | `github.com/datawhalechina/llm-cookbook` | **主线 · 这一层的核心教材**。吴恩达 11 门大模型课的中文版，含可运行代码，覆盖 Prompt / Function Calling / RAG / 评估 |
| OpenAI Cookbook（Function Calling 部分） | `github.com/openai/openai-cookbook` | 官方示例，写代码时对照 |
| Anthropic 文档：Prompt Engineering 与 Tool Use | `docs.anthropic.com` | 写得好，可当参考手册随手查 |
| **MCP 官方文档** | `modelcontextprotocol.io` | 讲到 MCP 那节直接读官方 quickstart |
| Hugging Face MCP Course | `huggingface.co/learn/mcp-course` | MCP 视频课，免费，比啃文档轻松 |

---

## 第 4 层 · 记忆与检索层 ← 你在这里

| 资料 | 说明 | 用法 |
|---|---|---|
| **Datawhale《llm-universe》（动手学大模型应用开发）** | `github.com/datawhalechina/llm-universe` | **主线 · 中文**。Prompt → API → 知识库 → RAG 完整走一遍，和本层作业高度对应 |
| FAISS 官方 Getting started 与 wiki | `github.com/facebookresearch/faiss/wiki` | 做作业 2（调 nprobe）时读，中文资料少，直接看官方 |
| sentence-transformers 文档 | `sbert.net` | 向量化作业用，示例代码直接能跑 |
| Elasticsearch《Practical BM25》系列 | 搜"practical bm25 elastic" | BM25 与稀疏检索讲得最清楚的工程视角 |
| Qdrant 概念文档 | `qdrant.tech/documentation` | 向量索引概念讲得比多数教材好，选读 |
| 论文：RAG（Lewis et al., 2020） | 搜"RAG Lewis 2020 arxiv" | 选读。RAG 的源头论文 |
| 论文：SPLADE | 搜"SPLADE sparse learned" | 选读。接上次"学习型稀疏检索"那个话题 |

---

## 第 5 层 · 编排层

| 资料 | 说明 | 用法 |
|---|---|---|
| **Anthropic《Building Effective Agents》** | 搜标题，官方博客 | **主线 · 先读这篇再动手**。讲清什么时候该用工作流、什么时候用自主 Agent，正是本层过关标准要的东西 |
| 论文 ReAct（Yao et al., 2022） | arXiv: 2210.03629 | 主线。裸写 ReAct 循环前看前 3 页就够 |
| LangGraph 官方文档教程 | `langchain-ai.github.io/langgraph` | 作业 2（改写成状态图）用 |
| Hugging Face Agents Course | `huggingface.co/learn/agents-course` | 免费系统课，和作业节奏搭 |
| 《Don't Build Multi-Agents》（Cognition） | 搜标题 | 选读。给"多智能体热"泼冷水的名文，正好中和本层最常见的过度设计 |

---

## 第 6 层 · 评测与守护层

| 资料 | 说明 | 用法 |
|---|---|---|
| **OWASP Top 10 for LLM Applications** | `genai.owasp.org` | **主线 · 安全部分照着清单过** |
| RAGAS 文档 | `docs.ragas.io` | RAG 评估框架，作业 1（20 题自动跑分）直接用它 |
| Simon Willison 博客的 prompt injection 系列 | `simonwillison.net` | 这个领域最好的跟踪来源，选读 |
| OpenAI Cookbook 的 Evaluation 部分 | 同上 GitHub | 选读 |

---

## 通用手册区（随时查，不用通读）

- **Hugging Face Learn**：`huggingface.co/learn` —— 12 门免费课的总入口（LLM / Agents / MCP / 评估都有）。国内访问慢可以配 `hf-mirror.com` 镜像。
- **Datawhale 开源组织**：`github.com/datawhalechina` —— 中文开源课程集中地，llm-cookbook、llm-universe 都在这。
- **B 站「跟李沐学AI」**：论文精读系列。遇到读不下去的英文论文，先看李沐的讲解再回头读原文。

---

## 三条使用提醒

1. **资料是给计划打工的，不是反过来。** 每层先做作业，卡住了再回来翻资料；顺序倒过来就变成"收藏夹吃灰"。
2. **主线资料跟着勾选走。** 看完一个主线资源，就在学习计划 HTML 里勾掉对应知识点。
3. **别为"找更好的资料"拖延。** 主线资料 80 分就够了，补上 20 分的是你写的代码，不是再找一份 90 分的教程。
