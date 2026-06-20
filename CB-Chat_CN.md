# CB-Chat &nbsp; [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE) [![Status: WIP](https://img.shields.io/badge/Status-WIP-orange)](https://github.com/yaoxinyaoxinyaoxin/CB-Chat) [![Concept](https://img.shields.io/badge/Type-Concept%20%2F%20PoC-lightgrey)]()

> **人人都是贝叶斯 · Everyone is a Bayesian**
>
> 将人类从「提示词编写者」升维为「概率空间的观测者与干预者」——通过 UI 交互层精准引导 LLM 推理收敛。
>
> Elevating humans from *prompt writers* to *probability-space navigators* — guiding LLM reasoning convergence through UI-level intervention.

---

📖 [Read in English](README.md) · [阅读英文版](README.md)


## 🧭 一页速览 / At a Glance

| 维度 | 内容 |
|------|------|
| **痛点** | LLM 多步推理中的不确定性逐级放大（误差累积） |
| **破局** | 人类作为「高维观测者」注入确定性力量 |
| **机制** | 可视化贝叶斯框架（先验→证据→后验）+ Harness 自动验证 + 多模态交叉验证 |
| **范式** | **CB-Paradigm**：动态可控的人机协同，权限保留而非处处介入 |
| **衍生产品** | CB-IDE / CB-Agent / CB-Embodied |
| **定位** | 概念验证原型（PoC），非生产系统 |

<details>
<summary>📖 English Version</summary>

| Dimension | Content |
|-----------|---------|
| **Pain Point** | Uncertainty amplification in LLM multi-step reasoning (error accumulation) |
| **Breakthrough** | Humans as "high-dimensional observers" injecting certainty |
| **Mechanism** | Visual Bayesian framework (Prior→Evidence→Posterior) + Harness auto-verification + multimodal cross-validation |
| **Paradigm** | **CB-Paradigm**: dynamic controllable human-AI collaboration with retained permission, not constant intervention |
| **Derivatives** | CB-IDE / CB-Agent / CB-Embodied |
| **Status** | Proof of Concept (PoC), not production |

</details>

---

## 💡 核心思想 / Core Philosophy

### 问题：不确定性放大

LLM 基于概率分布预测与采样，先天带不确定性。多步自回归生成中，微小误差随推理深度被不断放大。

<details>
<summary>English</summary>

LLMs predict and sample from probability distributions, inherently carrying uncertainty. In multi-step autoregressive generation, minor errors are amplified as reasoning depth increases.

</details>

### 方案：AI 展开空间，人类引导收敛

**AI 展开可能性空间 + 人类利用确定性力量引导收敛 = 避免不确定性放大**

人类的角色从底层「提示词编写者」→「概率空间的高维观测者」。Harness（工程护栏）处理底层验证，人类仅在高杠杆节点注入确定性。

<details>
<summary>English</summary>

**AI unfolds the space of possibilities + Humans use the force of certainty to guide convergence = Avoid uncertainty amplification**

Human role shifts from low-level "prompt writer" → "high-dimensional observer of probability space." The Harness handles low-level verification; humans inject certainty only at high-leverage nodes.

</details>

### 六大机制

| # | 机制 | 说明 |
|---|------|------|
| 1 | **可视化贝叶斯要素** | 先验、证据（似然）、后验判断的可视化拆解 |
| 2 | **人类干预与控制** | 通过条件修改精准限定 AI 探索方向 |
| 3 | **混合验证与动态控制** | Harness 自动兜底 + 人类高维节点介入（权限保留，非处处干预） |
| 4 | **主动假设与鉴别提问** | 信息不足时 AI 展开多假设，主动提问获取关键证据 |
| 5 | **多模态交叉验证与一票否决** | 硬证据（报错脚本、矛盾视觉反馈）可直接否决错误假设 |
| 6 | **实时反馈与修正演进** | 从回合制→流式近实时修正，随时打断、纠偏 |

<details>
<summary>English — Six Mechanisms</summary>

| # | Mechanism | Description |
|---|-----------|-------------|
| 1 | **Visual Bayesian Elements** | Visual breakdown of prior, evidence (likelihood), and posterior judgment |
| 2 | **Human Intervention & Control** | Precisely constrain AI exploration by modifying conditions |
| 3 | **Hybrid Verification & Dynamic Control** | Harness auto-safeguard + human intervention at high-dim nodes (retained permission, not constant intervention) |
| 4 | **Active Hypothesis & Discriminative Questioning** | AI generates multi-branch hypotheses and proactively asks for critical evidence when information is insufficient |
| 5 | **Multimodal Cross-Validation & Veto** | Hard evidence (failed scripts, contradictory visual feedback) holds veto power over erroneous hypotheses |
| 6 | **Real-time Feedback & Correction** | From turn-based → near-real-time streaming correction |

</details>

---

## 🔬 CB-Paradigm 衍生场景

| 场景 | 定位 | 核心价值 |
|------|------|----------|
| **CB-Chat** | 对话应用 | UI 层的人类概率空间导航 |
| **CB-IDE** | AI 编程工具（Cursor/Trae/Windsurf） | 每步动态注入业务条件，代码+测试+运行=多维验证闭环 |
| **CB-Agent** | 全自动智能体 | 人类作为高维贝叶斯观测节点随时注入新条件 |
| **CB-Embodied** | 具身控制 / 物理空间决策 | 空间预设+实时反馈校正，机器人/辅助驾驶/运动规划 |

<details>
<summary>English — CB-Paradigm Derivatives</summary>

| Scenario | Positioning | Core Value |
|----------|-------------|------------|
| **CB-Chat** | Chat application | UI-layer human probability-space navigation |
| **CB-IDE** | AI coding tools (Cursor/Trae/Windsurf) | Dynamic business-condition injection at each step; code+test+execution = multi-dim verification loop |
| **CB-Agent** | Fully automated agents | Human as high-dim Bayesian observation node, injecting conditions at any time |
| **CB-Embodied** | Embodied control / physical-space decisions | Spatial presets + real-time feedback correction; robotics, assisted driving, motion planning |

</details>

---

## 🚀 特性清单 / Feature Checklist

- [ ] 条件节点可视化 · Visualized Condition Nodes
- [ ] 推理方向锁定 · Reasoning Direction Locking
- [ ] 动态贝叶斯式更新 · Dynamic Bayesian-Inspired Updating
- [ ] 多步纠偏回溯 · Multi-step Correction & Backtracking
- [ ] 主动假设与鉴别提问 · Active Hypothesis & Discriminative Questioning
- [ ] 多模态证据闭环与一票否决 · Multimodal Evidence Loop & Veto Power
- [ ] Harness 集成验证 · Harness-Integrated Verification

---

## 🎯 逻辑评估要点 / Key Logic Points

- **单一模态瓶颈**：「语义合理」≠「事实验证」。多模态交叉验证形成立体验证网络，抑制不确定性放大
- **AI 局限性**：概率采样+提示词局限 → 语义偏移与幻觉持续累积
- **人类角色动态变化**：Harness 承担底层验证，人类占比下降但高维裁决仍关键
- **关键靶点识别**：以最小交互成本识别决定全局稳定性的高杠杆节点
- **智能化比例指标**：AI 正确决策与自动闭环比例稳步提升 = 系统智能化标志
- **『甲方定律』**：判定「什么是正确的、什么是有价值的」——最终裁决权天然在人类

<details>
<summary>English — Key Logic Points</summary>

- **Single-Modality Bottleneck**: "Semantically plausible" ≠ "factually verified." Multimodal cross-validation forms a stereoscopic verification network, suppressing uncertainty amplification.
- **AI Limitations**: Probability sampling + prompt limitations → continued accumulation of semantic drift and hallucinations.
- **Dynamic Human Role**: Harness handles low-level verification; human proportion decreases but high-dim arbitration remains critical.
- **Key Target Identification**: Identify high-leverage nodes determining global stability with minimal interaction cost.
- **Intelligence Ratio**: Steady increase in AI correct decisions and automatic closed-loop ratio = sign of system intelligence.
- **The "Client" Law**: Judging "what is correct, what is valuable" — the final arbitration right naturally belongs to humans.

</details>

---

## 🤔 哲学之问：这是倒退吗？

> 行业追求「全自动 Agent」，CB-Paradigm 重新引入人类强干预——这是否是倒退？

**不是。这是人机协同的「角色升维」，而非倒退。**

1. **「假全自动」的代价是失控**：缺乏人类校准的长链路任务中，LLM 在错误中间假设上盲目狂奔
2. **人类角色升维，而非增加负担**：人类从执行者→概率空间导航员，仅在高杠杆节点轻量干预
3. **确定性的最终来源**：AI 是工具，需求的提出者（甲方）是人类。只要概率采样的熵增未解决，人类高维隐性知识就是最重要的外部确定性来源

<details>
<summary>English — Philosophical Reflection</summary>

> The industry pursues "Fully Automated Agents." CB-Paradigm reintroduces strong human intervention — is this a step backward?

**No. This is "role ascension" in human-AI collaboration, not regression.**

1. **The cost of "pseudo-automation" is loss of control**: In long-chain tasks without human calibration, LLMs run blindly on erroneous intermediate assumptions.
2. **Human role ascension, not burden increase**: Humans shift from executors → probability-space navigators, intervening lightly only at high-leverage nodes.
3. **The ultimate source of certainty**: AI is a tool; the "Client" who defines needs is human. Until probability-sampling entropy is solved, human high-dimensional tacit knowledge remains the most important external certainty source.

</details>

---

## 📜 许可与引用 / License & Citation

本项目以 [MIT License](LICENSE) 发布。如需正式引用，请参考 [`CITATION.cff`](CITATION.cff)。

This project is released under the [MIT License](LICENSE). For formal citation, see [`CITATION.cff`](CITATION.cff).

