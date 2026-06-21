<div align="center">

# CB-Chat

**Controllable Bayesian Chat**

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Status: WIP](https://img.shields.io/badge/Status-WIP-orange)](https://github.com/yaoxinyaoxinyaoxin/CB-Chat)
[![Concept](https://img.shields.io/badge/Type-Concept%20%2F%20PoC-lightgrey)]()
[![Loop Engineering](https://img.shields.io/badge/Paradigm-Loop%20Engineering-blue)]()

**[English](#-english) · [中文](#-中文)**

</div>

> 🚧 **Work In Progress** — The core concepts have been defined, and the PoC implementation is still under active development and iteration.
> 🚧 **开发进行中** — 核心概念已基本明确，PoC 实现仍在持续开发与迭代中。
> **Everyone is a Bayesian · 人人都是贝叶斯**

---

<a id="-english"></a>

## 📑 Table of Contents

- [Overview](#-overview)
- [CB-Paradigm Derivatives](#-cb-paradigm-derivatives)
- [Core Philosophy](#-core-philosophy)
  - [The Three Control Categories](#-the-three-control-categories-of-controllable-bayesian-elements)
- [Logic Evaluation](#-logic-evaluation)
- [Key Features](#-key-features)
- [Philosophical Reflection](#-philosophical-reflection)
- [Loop Engineering](#-loop-engineering)

---

## 🌟 Overview

**CB-Chat (Controllable Bayesian Chat)** is a Bayesian-inspired AI Agent project built around visualizable and controllable interaction design. It aims to explore and alleviate the "uncertainty amplification" problem that Large Language Models (LLMs) face in complex multi-step reasoning — grounding this exploration in a synergistic framework of three control mechanisms: **Model Autonomous Control**, **Harness Feedback Control**, and **Human Correction Control**.

The working mechanism of LLMs is, in essence, to predict and sample from probability distributions, which inherently carries uncertainty. In multi-step reasoning processes, this uncertainty is further amplified. By contrast, the human user represents a relative "force of certainty" in this system.

**The core philosophy of this project is: through the design of the UI interaction layer, this human certainty is precisely directed to the true "target nodes" of the AI's reasoning chain, achieving effective control while avoiding meaningless consumption for both the AI and the human.**

- **Avoiding AI's consumption**: Preventing the AI from continuing meaningless reasoning and wasting tokens on incorrect probability branches after a semantic deviation occurs.
- **Avoiding human's consumption**: Through precise nodal intervention, allowing humans to achieve maximum correction benefits with minimal interaction costs.

Building upon this philosophy, CB-Chat can be understood as an AI Agent project centered on three interacting control mechanisms: **Model Autonomous Control** (the model's intrinsic ability to self-correct and suppress uncertainty without external assistance), **Harness Feedback Control** (automated verification and correction driven by engineering guardrails — static analysis, automated testing, script execution, and multimodal cross-validation), and **Human Correction Control** (targeted human intervention at key high-leverage nodes). The project explores how these three categories of control work in concert to determine the stability of multi-step, long-chain reasoning — and how their proportions shift dynamically as AI intelligence matures: the higher the intelligence level of the AI Agent, the higher the share of model autonomous control and harness feedback control, while the share of human correction control correspondingly decreases. At its core, CB-Chat investigates the path toward AI Agents where automated control mechanisms handle the vast majority of reasoning nodes, and humans ascend to the role of high-dimensional observers and probability-space navigators, intervening only at the few irreducibly high-leverage target nodes.

Building further on this, the project introduces the concept of **Dynamic Verifiability**: verification intensity should not be one-size-fits-all, but should be dynamically layered according to reasoning chain length and risk — relaxing verification for short-chain tasks to gain efficiency, and strengthening verification for long-chain tasks to ensure stability.

During the collaboration between humans and AI, this project attempts to shift the human role positioning at the UI interaction layer — elevating humans from low-level "prompt writers" to "observers and interveners of the probability space," thereby effectively combining human prior knowledge and dynamic intervention with AI's powerful reasoning capabilities.

---

## 🔬 CB-Paradigm Derivatives

> **⚠️ Special Note**
>
> This project serves as a Proof of Concept (PoC) prototype, aiming to intuitively explore and demonstrate this philosophy. **Its core "Dynamic Controllability" — preserving, at the permission level, the human ability to strongly intervene and correct probabilities at any AI reasoning node, while in actual operation prioritizing automatic correction by the verification network and concentrating human certainty on the small number of high-risk, high-leverage target nodes that are difficult to correct automatically — can be regarded as a new paradigm of intelligent collaboration (CB-Paradigm).**
>
> This "dynamic controllability" is not limited to chat. The following derived application scenarios map the **8-step dynamic loop** (Prior → Evidence → Posterior → Execute → Result → Verify → Feedback → Iterate) onto different AI infrastructure domains:

| Scenario | Positioning | Core Value |
|----------|-------------|------------|
| **CB-IDE** | AI coding tools (Cursor/Trae/Windsurf) | Each reasoning step maps to the dynamic loop: business conditions inject at **Evidence**, code generation at **Execute**, test runs at **Verify**, and failures feed back as new **Evidence** — the IDE itself becomes a multi-dimensional Harness. Human intervention focuses on architectural and business-logic target nodes where automated verification cannot reach. |
| **CB-Agent** | Fully automated agent loops | The agent loop runs autonomously through all 8 stages; the human ascends to a high-dimensional observer, intervening only at **identified target nodes** — where pre-set conditions cannot suppress emerging uncertainty, or where value judgment and goal arbitration are irreducibly required. As Model Autonomous Control and Harness Feedback Control mature, the proportion of Human Correction Control naturally declines. |
| **CB-Embodied** | Embodied control / physical-space decisions | Spatial presets = **Prior**; real-time sensor streams = continuous **Evidence**; physical execution = **Execute→Result**; cross-modal sensor fusion (visual, tactile, proprioceptive) = multi-dimensional **Verify**. Objective hard physical evidence holds **veto power** over erroneous hypotheses — applicable to robotics, assisted driving, and motion planning. |
| **CB-Loop** | Loop Engineering integration (Claude Code / Codex / Hermes Agent) | CB-Paradigm applied to autonomous coding agent loops: pre-set conditions govern the **Discover→Plan→Execute→Verify→Iterate** cycle, but when uncertainty escapes pre-set guardrails at mid-execution reasoning nodes, dynamic node-level human certainty injection activates — directly addressing the structural blind spot in pure Loop Engineering. |
---

## 💡 Core Philosophy

### The Pain Point: Uncertainty Amplification in Multi-Step Reasoning

In complex tasks, even the most advanced Large Language Models often possess contextual conditions (information from the user) that are less comprehensive and accurate than what the human users themselves hold. At the same time, the mechanism by which LLMs predict and sample from probability distributions inherently carries uncertainty. During automated multi-step reasoning by AI, without precise intervention, any minor uncertainty may be amplified as the depth of reasoning increases (error accumulation) — this is the core stability challenge facing AI Agents in long-horizon reasoning tasks.

### The Breakthrough: Humans as High-Dimensional Observers

Human intervention may remain a key path to mitigating this problem. The essence of CB-Chat is the combination of **"AI unfolding the space of possibilities" + "Humans using the force of certainty to guide AI convergence"** to avoid the amplification of uncertainty and gradually converge the space of posterior judgment. As AI capability, multimodal perception, and **Harness-based verification** continue to improve, the proportion of human involvement in low-level correction and local verification may gradually decrease; however, in complex tasks driven by human needs, goal definition, value judgment, and final arbitration are still primarily carried out by humans.

### Solution: Visualized and Controllable Bayesian-Inspired Updating

1. **Visualizing the Bayesian-Inspired Dynamic Loop**: At the interaction layer, visually breaking down the complete dynamic iteration cycle — **"prior → conditions/evidence → posterior judgment → execute → result → verify → feedback → (iterate)"** — making the full chain from cognition to execution to verification transparent. Here, "Bayesian" is used primarily as a cognitive and design framework rather than as a strict mathematical reconstruction of the model's internal state.

2. **Human Intervention & Control**: Allowing users to accurately limit the AI's direction of thought by controlling and modifying conditions, enabling the AI to explore only in specific, controlled directions.

3. **Hybrid Verification & Dynamic Control**: This does not mean increasing the burden on humans. During multi-turn conversations, this framework attempts to combine **Harness-based verification** (such as static code analysis, automated testing, and script execution validation) with dynamic human control. The underlying logic should first be safeguarded automatically by the Harness, while humans (the "Client") mainly update, modify, and revoke conditions at high-dimensional nodes such as "business value" and "architectural direction." In this context, "allowing intervention at any node" is better understood as a matter of **retained permission**, rather than a recommendation for **constant intervention everywhere**: in theory, any node can become the starting point of later deviation amplification, but as model capability and verification networks improve, most local deviations should ideally be detected and corrected automatically by the system. The nodes that truly require precise human intervention are often those deviations that cannot yet be effectively covered by the verification network, those that remain even after verification, or those high-leverage target nodes whose unchecked development may trigger a butterfly-effect-like chain amplification. Therefore, the system's ability to identify these key targets intelligently and at low cost, and to inject human certainty only when necessary, is central to improving overall stability and control efficiency.

4. **Active Hypothesis & Discriminative Questioning**: When human-provided prior information (prompts) is insufficient, the system avoids hastily forcing a single answer. Instead, the AI generates multiple candidate hypotheses internally and proactively asks highly discriminative questions to the human. Through the human's answers (providing new evidence), the AI can more quickly eliminate incorrect branches and retain reasonable hypotheses, upgrading "one-way prompting" to "two-way discrimination."

5. **Multimodal Cross-Validation & Veto Mechanism**: When text, execution results, logs, file structures, vision, audio, touch, or other sensor feedback are incorporated into the same loop, the system can use the Harness to cross-validate information across different dimensions. In multi-dimensional verification, objective "hard evidence" (such as a failed script or contradictory visual feedback) holds **"veto power"** over current prior hypotheses, immediately eliminating erroneous assumptions. When evidence support is inconsistent, the system suspends operation, prompting the need to gather more information, re-reason, and review. This mechanism not only relieves the verification pressure of any single dimension but also significantly reduces the frequency of continuous human intervention.

6. **Real-time Feedback & Correction Evolution**: The future form will move beyond today's "turn-based" correction. By capturing conditions in real time, it can enable near-real-time correction during the AI's streaming generation process. Just like face-to-face real-time interaction between humans, interrupting at any time, correcting at any time, and synchronizing in real time, it forms a tighter closed-loop control process.

7. **Dynamic Verifiability — Layered Verification**: The intensity of verification should not be uniform; it should be dynamically layered according to task complexity and risk. For short-chain tasks with few reasoning steps, where uncertainty is unlikely to amplify, verification requirements can be appropriately relaxed — excessive verification would only introduce unnecessary computational overhead and interaction cost. For large, multi-step, long-horizon projects, stricter verification mechanisms should be activated — including multi-dimensional cross-validation, comprehensive automated testing, and human review at critical nodes. This "verification-on-demand" layered design allows the system to concentrate finite verification resources on genuinely high-risk reasoning segments, achieving an optimal balance between control efficiency and outcome reliability.

### The Three Control Categories of Controllable Bayesian Elements

Building upon the seven design principles above, the Controllable Bayesian elements (prior information, conditions, evidence, etc.) can be further classified into three categories by their control source:

1. **Model Autonomous Control**: Corrections, verifications, and probability adjustments completed independently by the model through its own reasoning capabilities — including internal consistency checks, self-verification, and multi-path comparison. This represents the model's intrinsic ability to suppress uncertainty without external assistance.

2. **Harness Feedback Control**: Automated corrections driven by the engineering harness (Harness) — including static analysis, automated testing, script execution verification, and multimodal cross-validation. These system-level feedback loops provide objective, reproducible verification signals that can autonomously eliminate erroneous probability branches.

3. **Human Correction Control**: Interventions initiated by humans — including condition injection, evidence provision, direction locking, and final arbitration at key nodes. This represents the external "force of certainty" that the human, as the ultimate client and high-dimensional observer, contributes to the system.

These three categories together determine the stability of the model in multi-step, long-chain reasoning tasks. Crucially, **the higher the intelligence level of an AI Agent, the higher the proportion of the first two categories** (model autonomous control and harness feedback control), while the proportion of human correction control correspondingly decreases. This is not merely a design preference — it is a measurable indicator of AI capability maturation:

- A system where most corrections still depend on human intervention remains closer to the traditional tool paradigm.
- A system where model autonomous control and harness feedback control handle the vast majority of reasoning nodes, with humans intervening only at a small number of high-leverage target nodes, represents a genuinely higher level of intelligent collaboration.

In the ideal limit, an AI Agent with sufficiently advanced intelligence would autonomously handle nearly all reasoning nodes through model autonomous control and harness feedback control, with humans only needing to exercise their retained intervention rights at the very few nodes where value judgment, goal arbitration, or ethical accountability is irreducibly required. This proportion shift — the declining share of human correction control relative to the other two categories — is itself an important quantitative indicator of AI Agent intelligence evolution, and a core optimization objective of the CB-Paradigm.

---

## 🎯 Logic Evaluation

The core logic of this project borrows the **intuitive structure within Bayesian thinking** and extends it into a dynamic iteration cycle: from the cognitive framework of "Prior Knowledge + New Evidence = Posterior Cognition," further extended into the complete Agent execution chain — **"Prior → Conditions/Evidence → Posterior Judgment → Execute → Result → Verify → Feedback → (Iterate)"**. In this document, "Bayesian" is used mainly to describe a visualizable, intervenable, and verifiable human-AI collaboration framework, rather than to make a strict mathematical claim about the model's parameters or internal probability distribution.

- **The Verification Bottleneck of Single-Modality Systems & The Trend Toward Multimodality**: In pure-text or other single-dimensional systems, the model lacks information from other dimensions and external closed-loop verification. As a result, something that appears semantically plausible is not necessarily factually or task-wise verified. This creates a clear ceiling for verifiability and robustness in single-modality systems. Rich multimodal information and multi-dimensional cross-validation refer not only to checking final results across different dimensions, but also to mutual verification among inputs, intermediate results, and outputs across those dimensions, thereby forming a more stereoscopic verification network. This mechanism can effectively suppress the amplification of uncertainty, thereby reducing the frequency of human intervention and making the AI appear more intelligent and biomimetic. This is also one of the important underlying reasons why AI continues to evolve toward multimodality.

- **AI's Limitations**: Due to prompt limitations and the model's inherent probability distribution-based sampling mechanism, the AI's initial prior judgment is often too broad. During multi-step autoregressive generation, this intrinsic randomness can easily lead to the continued accumulation of semantic drift and hallucinations.

- **The Dynamic Role of Humans**: As "high-dimensional observers", humans possess rich tacit knowledge. As AI capability improves and the **Harness** takes over more low-level verification work, the proportion of direct human involvement in local decisions and low-level correction can gradually decrease. However, in goal definition, value judgment, and final arbitration, humans are still likely to remain essential for a considerable period of time. The key is not to make humans intervene frequently at every node, but to preserve their right to intervene at any node and to identify, as intelligently as possible, the true "target nodes" that require human certainty injection: nodes where the verification network cannot yet provide effective coverage, where deviations remain even after verification, or where a loss of control could trigger high-leverage chain amplification.

- **Key Target Identification & Stability at Minimum Cost**: From a system-design perspective, the more valuable goal is not simply to increase the number of human interventions, but to identify the small number of key nodes most likely to determine global stability with the lowest possible observation, verification, and interaction cost. If most ordinary nodes can already be automatically corrected by model capability and the verification network, then the upper bound of system stability will increasingly depend on whether the system can detect the few high-impact residual deviations in time and, when necessary, inject high-confidence human evidence or arbitration to prevent a local error from evolving into a butterfly-effect-like global drift in long-horizon tasks.

- **The Intelligence Ratio in Hybrid Systems & The Three Control Categories**: Within this framework, a more precise lens is to observe how the proportions of the three control categories shift dynamically as AI capability matures: the higher the share of **model autonomous control and harness feedback control**, the closer the system is to a genuinely high level of intelligent collaboration; the higher the share of **human correction control**, the closer the system remains to the traditional tool paradigm. Under acceptable result quality, verification capability, and responsibility boundaries, this proportion shift — whether the share of human correction control in correct decisions can steadily decline — is a core quantitative indicator of system intelligence.

- **Multimodality and Cross-Dimensional Verification**: When text, execution results, logs, file structures, vision, audio, touch, or other sensor feedback are incorporated into the same loop, the system can use the **Harness** to cross-validate across dimensions, thereby reducing the verification pressure of any single dimension and lowering the frequency of human intervention. Here, "verification" includes not only checking final results across dimensions, but also mutual validation among inputs, intermediate results, and outputs across different dimensions, thereby forming a more stereoscopic verification network. For example, in an IDE setting, code text, script execution, automated testing, output generation, and result validation can jointly verify whether a given hypothesis holds; in this sense, they themselves are part of the **Harness** and the multimodal, multi-dimensional verification mechanism.

- **Dynamic Verifiability & Layered Verification Strategy**: Not all reasoning nodes require the same intensity of verification. In short-chain tasks, model autonomous control is often sufficient on its own — excessive verification only reduces efficiency. In long-chain tasks, uncertainty accumulates and amplifies with each step, requiring harness feedback control and multi-dimensional cross-validation to progressively strengthen verification. This layered strategy is, at its core, a dynamic allocation of the three control resources: letting model autonomous control dominate in low-risk segments, and activating combined harness feedback control and human correction control in high-risk segments. This risk-graded allocation of verification resources is an important design principle for improving overall system efficiency and stability.

- **Human-AI Collaborative Convergence**: Through UI-level control, humans continuously input high-confidence evidence to prune reasoning paths, while AI continuously updates its judgment according to the **"prior → conditions/evidence → posterior judgment → execute → result → verify → feedback → (iterate)"** dynamic loop — where verification results are automatically fed back as new evidence, driving the next iteration. This logical closed-loop provides an operational path to help alleviate the difficulty large models face in achieving stable self-correction.

---

## 🚀 Key Features

- [ ] **Dynamic Loop Node Visualization**: Breaking down complex prompts into visual nodes for each stage of the complete dynamic loop — prior, conditions/evidence, posterior judgment, execution, result, verification, and feedback — covering the full chain from cognition to execution to verification.
- [ ] **Reasoning Direction Locking**: Forcing AI to explore along designated probability paths via drag-and-drop or parameter adjustment.
- [ ] **Dynamic Bayesian-Inspired Updating**: Real-time reflection of how AI judgment and reasoning paths change after new evidence is added.
- [ ] **Multi-step Correction & Backtracking**: Reverting to any probability fork point at any time, modifying conditions, and regenerating.
- [ ] **Active Hypothesis & Discriminative Questioning**: When information is insufficient, AI automatically generates multi-branch hypotheses and proactively asks humans for critical evidence.
- [ ] **Multimodal Evidence Loop & Veto Power**: Combining text, execution results, logs, and sensor feedback for cross-validation; objective "hard evidence" holds veto power over erroneous hypotheses, relieving the information bottleneck of single-modality systems.
- [ ] **Harness-Integrated Verification**: Bringing script execution, automated testing, and external tool feedback into the same verification loop to reduce the need for continuous human intervention.
- [ ] **Dynamic Verifiability — Layered Verification**: Dynamically adjust verification intensity based on reasoning step count and task risk — relaxed for short chains, strengthened for long chains — achieving an optimal balance between efficiency and stability.

---

## 🤔 Philosophical Reflection: Is This a Step Backward?

People might ask: **With the current industry trend pursuing "Fully Automated Agents (Auto-Agent)", does the CB-Paradigm's reintroduction of strong human intervention — reverting from full automation to "Human-in-the-loop" — represent a historical step backward?**

My perspective is: **This is perhaps not a step backward, but rather a "role ascension" in the evolution of human-AI collaboration.**

1. **The Cost of "Pseudo-Automation" is Loss of Control**: When executing long-chain, complex real-world tasks, the current so-called "full automation" of large language models often means running blindly on erroneous intermediate assumptions. In certain complex scenarios, full automation without human calibration can sometimes face challenges regarding confidence and yield.

2. **The Ascension of the Human Role, Not an Increase in Burden**: In the traditional "semi-automatic" era, humans were specific executors (workers). However, in the CB-Paradigm, with **model autonomous control** (the model's intrinsic self-correction capability) and the **Harness** handling low-level verification and correction, together with multimodal cross-validation, humans no longer need to continuously participate in low-level generative labor. Instead, they have the opportunity to be elevated to **"Navigators of the probability space"** and **"High-dimensional observers"**. AI is responsible for unfolding massive trees of possibilities, while humans only perform lightweight "pruning" and "condition injection" at critical nodes. As model capability and verification systems improve, the proportion of **model autonomous control and harness feedback control** steadily increases, and the frequency of human intervention naturally declines — yet the human role in high-level arbitration remains irreplaceable.

3. **The Ultimate Source of Certainty (The "Client" Law)**: Fundamentally, AI is merely a tool used to solve human needs. Since the initiator of the demand (the "Client") is human, the final basis for judging what is correct and valuable in a given task context should naturally be provided and arbitrated primarily by humans. Until the problem of entropy increase caused by AI's internal probability sampling mechanism is completely solved, human high-dimensional tacit knowledge will remain a major external source of certainty for complex systems. If one hopes to further push the human share of correct decision-making toward near zero, the obstacle will no longer be only a technical problem of uncertainty control, but will increasingly enter the domain of responsibility attribution and ethical accountability.

---

## 🔄 Loop Engineering

> **Loop Engineering** is the emerging 2025–2026 paradigm in AI Agent engineering: shifting from turn-by-turn prompt writing to designing autonomous agent loops — systems that discover work, plan, execute, verify, and iterate on a schedule until a verifiable stopping condition is met.

### Similarities: Where CB-Chat and Loop Engineering Converge

| Dimension | Shared Ground |
|-----------|---------------|
| **Verification as load-bearing** | Both recognize that a loop without verification is just automation (SonarSource). CB-Chat's **Harness Feedback Control** and Loop Engineering's **Verification Loop** serve the same function: automated, reproducible correctness checks. |
| **Multi-step reasoning stability** | Both address the core problem that single-pass LLM outputs degrade over long reasoning chains. Loop Engineering breaks tasks into Plan→Execute→Verify cycles; CB-Chat visualizes the full "prior→evidence→posterior→execute→result→verify→feedback" dynamic loop for each reasoning step. |
| **Human-in-the-Loop** | Both acknowledge that fully autonomous agents need human intervention at critical junctures. Loop Engineering's HITL pattern and CB-Chat's **Human Correction Control** share the same premise. |
| **Iteration until convergence** | Both reject one-shot prompting. CB-Chat's dynamic Bayesian updating and Loop Engineering's iterate-until-condition-met are the same underlying cyclic principle. |
| **Harness/Guardrails** | CB-Chat's **Harness** (engineering guardrails for verification) directly parallels the Loop Engineering "Harness" layer in the Orange Book's four-layer architecture. |

### The Key Difference: Pre-Set Conditions vs. Dynamic Mid-Course Intervention

This is where CB-Chat and Loop Engineering fundamentally diverge:

| | Loop Engineering | CB-Chat |
|---|---|---|
| **Core assumption** | Conditions and goals can be pre-defined sufficiently at design time | Pre-defined conditions are *never* sufficient for complex tasks — uncertainty will inevitably surface mid-execution |
| **Human intervention window** | Design time (set up the loop) + Approval time (binary: approve/reject) | **Any reasoning node at any time** — a continuous spectrum of intervention |
| **Intervention granularity** | Operation-level (approve/reject a tool call) | **Node-level** (modify priors, inject evidence, lock direction at specific reasoning nodes) |
| **Coverage of uncertainty** | Relies on pre-set conditions + verification to suppress uncertainty | Admits uncertainty cannot be fully suppressed → retains dynamic intervention capability at every node |
| **Conceptual essence** | An **automation engineering framework** — design the loop, then walk away | An **uncertainty management framework** — stay engaged at the resolution that matters |

The critical insight: **Loop Engineering pre-sets all conditions and goals, then lets the Agent explore autonomously within those boundaries. But pre-set conditions can never fully cover and suppress uncertainty in complex tasks.** When uncertainty inevitably surfaces mid-execution — at a reasoning node where no pre-set verification rule catches the semantic drift — Loop Engineering has no native mechanism to intervene with precision. The human must either wait until the loop completes (wasting tokens on incorrect branches) or kill the loop and restart (losing context).

CB-Chat is designed precisely for this gap: it covers **both** the pre-set phase (conditions, goals, verification rules) **and** the mid-course phase (dynamic node-level intervention when uncertainty escapes pre-set guardrails). This is not a complementary addition — it is a **conceptual superset**: CB-Chat's intervention model encompasses Loop Engineering's pre-set approach while extending it to real-time, node-granular, reasoning-level control.

### CB-Chat's Positioning in the Loop Engineering Landscape

```
Prompt Engineering  →  Agentic Workflows  →  Loop Engineering  →  CB-Paradigm
(one-shot)              (multi-step)          (autonomous loop)     (controllable loop)
                                                         │
                                              Pre-set conditions + autonomous execution
                                                         │
                                              ─ ─ ─ GAP ─ ─ ─
                                                         │
                                              Uncertainty escapes pre-set guardrails
                                              at mid-execution reasoning nodes
                                                         │
                                                         ▼
                                              CB-Chat: dynamic node-level
                                              human certainty injection
```

This is why CB-Chat is not merely "Loop Engineering with a better UI." It addresses a **structural blind spot** in the Loop Engineering paradigm: the assumption that pre-defined conditions and verification rules can anticipate and contain all forms of uncertainty in complex, long-horizon reasoning tasks.

---

<a id="-中文"></a>

## 📑 目录

- [项目简介](#-项目简介)
- [CB-Paradigm 衍生场景](#-cb-paradigm-衍生场景)
- [核心思想](#-核心思想)
  - [可控制贝叶斯要素的三类控制](#-可控制贝叶斯要素的三类控制)
- [核心逻辑评估](#-核心逻辑评估)
- [核心特性](#-核心特性)
- [哲学思考](#-哲学思考)
- [Loop Engineering](#-loop-engineering-1)

---

## 🌟 项目简介

**CB-Chat (Controllable Bayesian Chat)** 是一个受贝叶斯思想启发的 AI Agent 项目，围绕可视化与可控制的交互设计展开。它旨在探索和缓解大语言模型（LLM）在复杂多步推理中面临的"不确定性放大"问题——并将这一探索构建于**模型自主控制、Harness 反馈控制、人为修正控制**三类机制的协同框架之上。

大语言模型的工作机制，本质上是基于概率分布进行预测与采样，因此先天带有不确定性。在多步骤的推导过程中，这种不确定性会被进一步放大。相比之下，人类用户在这个系统中代表着一种相对的"确定性力量"。

**本项目的核心思想在于：通过 UI 交互层的设计，将这种人类的确定性力量精准引导至 AI 推理链条的真正"靶点"上，从而实现对 AI 的有效控制，同时避免 AI 与人类双向的无意义消耗。**

- **避免 AI 的消耗**：防止 AI 在发生语义偏移后，继续在错误的概率分支上进行毫无意义的推理与 Token 浪费。
- **避免人类的消耗**：通过精准的节点干预，让人类用最小的交互代价，获得最大的纠偏收益。

在这一思想基础上，CB-Chat 可被理解为一个围绕三种相互作用控制机制构建的 AI Agent 项目：**模型自主控制**（模型在无需外部辅助的情况下自我纠偏与抑制不确定性的内在能力）、**Harness 反馈控制**（由静态分析、自动化测试、脚本运行验证、多模态交叉验证等工程护栏驱动的自动验证与纠正），以及**人为修正控制**（人类在关键高杠杆节点上的精准干预）。本项目探索这三类控制如何协同作用，共同决定多步骤、长程推理的稳定性——以及随着 AI 智能的成熟，三者的占比如何动态变化：AI Agent 的智能程度越高，模型自主控制与 Harness 反馈控制的占比越高，人为修正控制的占比则相应下降。CB-Chat 的核心探索方向在于：通往一种 AI Agent 形态，其中自动控制机制覆盖绝大多数推理节点，而人类升维为高维观测者与概率空间的导航员，仅在极少数不可化约的高杠杆靶点介入。

在此基础上，本项目进一步提出**动态可验证性（Dynamic Verifiability）**的概念：验证的强度不应一刀切，而应根据推理链的长度与风险进行动态分层——短链任务放宽验证以换取效率，长链任务加码验证以保障稳定。

在人类与 AI 的协作过程中，本项目试图在 UI 层改变人类的角色定位——将人类从底层的"提示词编写者"升维为"概率空间的观测者与干预者"，从而将人类的先验知识、动态干预与 AI 的强大推理能力有效结合。

---

## 🔬 CB-Paradigm 衍生场景

> **⚠️ 特别说明**
>
> 开发的这项应用是一个概念验证（Proof of Concept）原型，旨在直观探讨和展示这一思想。**其核心的"动态可控性（Dynamic Controllability）"——即允许人类在权限层面保留对 AI 任意推理节点进行强干预与概率修正的能力，但在实际运行中优先依赖验证网络自动纠偏，并将人类的确定性注入聚焦于少量高风险、高杠杆、难以自动校正的关键节点（靶点）——可被视为一种新的智能协同范式（CB-Paradigm）。**
>
> 这一"动态可控"思想并不局限于对话。以下衍生应用场景将 **8 步动态循环**（先验 → 条件/证据 → 后验判断 → 执行 → 结果 → 验证 → 反馈 → 迭代）映射到不同的 AI 基础设施领域：

| 场景 | 定位 | 核心价值 |
|------|------|----------|
| **CB-IDE** | AI 编程工具（Cursor/Trae/Windsurf） | 每个推理步骤映射到动态循环：业务条件在 **Evidence** 阶段注入，代码生成在 **Execute** 阶段，测试运行在 **Verify** 阶段，失败结果作为新 **Evidence** 反馈——IDE 本身成为多维 Harness。人类介入聚焦于自动化验证无法覆盖的架构与业务逻辑层面的靶点。 |
| **CB-Agent** | 全自动智能体循环 | Agent 在全部 8 个阶段自主运行；人类升维为高维观测者，仅在**识别到的靶点**介入——即预设条件无法压制的不确定性浮现处、或价值判断与目标裁决不可化约处。随着模型自主控制与 Harness 反馈控制增强，人为修正控制的占比自然下降。 |
| **CB-Embodied** | 具身控制 / 物理空间决策 | 空间预设 = **Prior**；实时传感流 = 持续的 **Evidence**；物理执行 = **Execute→Result**；跨模态传感融合（视觉、触觉、本体感知）= 多维度 **Verify**。客观物理硬证据对错误假设具有**一票否决权**——适用于机器人、辅助驾驶、运动规划。 |
| **CB-Loop** | Loop Engineering 集成（Claude Code / Codex / Hermes Agent） | CB-Paradigm 应用于自主编程 Agent 循环：预设条件主导 **Discover→Plan→Execute→Verify→Iterate** 周期，但当不确定性在执行中途溢出预设护栏时，动态节点级人类确定性注入激活——直接填补纯 Loop Engineering 的结构性盲区。 |
---

## 💡 核心思想

### 痛点：多步推理中的不确定性放大

在复杂任务中，即便是最先进的大语言模型，其获取的上下文条件（来自用户的信息）在完整性与准确性上也往往低于人类用户本身。与此同时，大语言模型基于概率分布进行预测与采样的机制，本身天然带有不确定性。在 AI 进行多步骤的自动化推理时，如果缺乏精准的干预，任何微小的不确定性都可能随着推理深度的增加而被不断放大（误差累积）——这正是长程推理任务中 AI Agent 面临的核心稳定性挑战。

### 破局：人类作为高维的观测者

人类的介入或许是缓解这一问题的关键途径。CB-Chat 的本质是通过 **"AI 展开可能性空间" + "人类利用确定性力量引导 AI 收敛"** 的组合，来避免不确定性被放大，并促使后验判断的空间逐步收敛。随着 AI 能力、多模态感知与 **Harness（工程护栏）** 验证能力的提升，人类在低层纠错与局部验证中的参与比例可以逐步下降，但在人类需求主导的复杂任务中，目标定义、价值判断与最终裁决仍主要由人类承担。

### 解决方案：可视化与可控的贝叶斯式更新

1. **可视化贝叶斯式动态循环**：在交互层将对话和推理过程中的完整动态迭代循环——「先验 → 条件/证据 → 后验判断 → 执行 → 结果 → 验证 → 反馈 →（迭代）」——进行可视化拆解，让黑盒推理从认知到执行再到验证的全链路变得更加透明。这里的"贝叶斯"主要作为设计框架中的认知表达，而非对底层模型内部状态的严格数学还原。

2. **人类干预与控制**：允许用户通过控制和修改条件，准确限定 AI 的思考方向，让 AI 仅在特定、受控的方向上进行探索。

3. **混合验证与动态控制**：这并非意味着增加人类的负担。在多轮对话中，本框架尝试将 **Harness（工程护栏）** 验证（如静态代码检查、自动化测试、脚本运行验证）与人类的动态控制相结合。底层逻辑优先交由 Harness 自动兜底，而人类（甲方）主要在"业务价值、架构方向"等高维节点上，动态地更新、修改和撤销条件。这里所说的"允许干预任意节点"，更接近一种**权限保留**而非**默认处处介入**：因为理论上任意节点都可能成为后续偏移放大的起点，但随着模型能力与验证网络的增强，大多数局部偏移应优先由系统自动识别并纠正；真正需要人类精准介入的，往往是那些暂时无法被验证网络有效验证的偏移、已经过验证但仍然残留的偏移，或一旦放任发展就可能产生"蝴蝶效应式"连锁放大的高杠杆节点（靶点）。因此，系统能否以较低成本智能识别这些关键靶点，并在必要时引入人类的确定性力量，是提升整体稳定性与控制效率的关键。

4. **主动假设与鉴别提问**：当人类输入的先验信息（提示词）不足时，系统不会急于强行输出单一答案。相反，AI 会在内部展开多种可能的候选假设，并主动向人类提出极具鉴别力的问题。通过人类对这些问题的回答（提供新证据），AI 能够更快速地排除错误分支并保留合理假设，从而将"单向提示"升级为"双向鉴别"。

5. **多模态交叉验证与一票否决机制**：当文本、运行结果、日志、文件结构、视觉、听觉、触觉或其他传感反馈被纳入同一闭环时，系统可以借助 Harness 对不同维度的信息进行交叉验证。在多维验证中，客观的"硬证据"（如报错的脚本、矛盾的视觉反馈）对当前的先验假设具有 **"一票否决权"**，可以直接排除该错误假设；而当多方证据支持不一致时，系统会悬停并提示重新收集信息、重新推理与复盘。这种机制不仅缓解了单一维度验证的压力，也极大降低了人类持续介入的频率。

6. **实时反馈与修正演进**：未来形态将突破现有的"回合制（Turn-based）"校正。通过实时的条件捕捉，实现 AI 在流式生成（Streaming）过程中的近实时修正。如同人类之间面对面的实时互动一样，随时打断、随时纠偏、实时同频，形成更紧密的闭环控制。

7. **动态可验证性——分层验证机制**：验证的强度不应是均匀的，而应根据任务的复杂度与风险进行动态分层。对于推理步骤较少、不确定性不易放大的短链任务，验证要求可以适当放宽——过度验证反而会引入不必要的计算开销与交互成本；对于大型、多步骤的长程项目，则应启动更为严格的验证机制——包括多维交叉验证、自动化测试全覆盖、关键节点的人工复核等。这种「按需验证」的分层设计，使得系统能够在保障稳定性的前提下，将有限的验证资源聚焦于真正高风险的推理环节，从而在控制效率与结果可靠性之间取得最优平衡。

### 可控制贝叶斯要素的三类控制

在上述七项设计原则的基础上，可控制的贝叶斯要素（如先验信息、条件、证据等），可以按控制来源进一步分为三类：

1. **模型自主控制**：由模型通过自身推理能力独立完成的纠偏、验证与概率调整——包括内部一致性检查、自我验证、多路径对比等。这代表了模型在无需外部辅助的情况下，内在地抑制不确定性的能力。

2. **Harness 反馈控制**：由工程护栏（Harness）驱动的自动化纠正——包括静态分析、自动化测试、脚本运行验证、多模态交叉验证等系统级反馈。这些反馈回路提供客观、可复现的验证信号，能够自主排除错误的概率分支。

3. **人为修正控制**：由人类主动发起的干预——包括关键节点的条件注入、证据提供、方向锁定与最终裁决。这代表了人类作为最终需求方和高维观测者，向系统中注入的外部确定性力量。

这三类控制共同决定了模型在多步骤、长程推理任务中的稳定性。关键在于，**AI Agent 的智能程度越高，前两者（模型自主控制与 Harness 反馈控制）的占比越高**，人为修正控制的占比则相应下降。这不仅是一种设计偏好，更是 AI 能力成熟度的可度量标志：

- 若大多数纠偏仍依赖人类干预，系统更接近传统工具范式。
- 若模型自主控制与 Harness 反馈控制已能覆盖绝大多数推理节点，人类仅在少量高杠杆靶点介入，则代表了真正更高水平的智能协同。

在理想极限下，一个智能程度足够高的 AI Agent，应能通过模型自主控制与 Harness 反馈控制自主处理近乎所有推理节点，人类仅需在价值判断、目标裁决或伦理责任等不可化约的极少数节点中，行使其保留的干预权限。这一比例变化——人为修正控制相对于前两类的持续下降——本身就是衡量 AI Agent 智能演进的重要量化指标，也是 CB-Paradigm 的核心优化目标。

---

## 🎯 核心逻辑评估

本项目的核心逻辑借用了**贝叶斯思想中的直观结构**并进行了动态迭代扩展：从「先验知识 + 新证据 = 后验认知」的认知框架，进一步延伸为覆盖完整 Agent 执行链路的**「先验 → 条件/证据 → 后验判断 → 执行 → 结果 → 验证 → 反馈 →（迭代）」**动态循环。在本文中，"贝叶斯"主要用于描述一种可视化、可干预、可验证的人机协同框架，而不是对底层模型参数或内部概率分布的严格数学声明。

- **单一模态的验证瓶颈与多模态的演进趋势**：在纯文本或其他单一维度系统中，模型缺乏来自其他维度的信息与外部闭环验证，因此"语义上看起来合理"并不等于"事实或任务上已经被验证"。这使得单一模态系统在可验证性与稳健性上存在明显上限。而丰富的多模态信息与多维度的交叉验证，所指的并不只是不同维度最终结果之间的验证，还包括不同维度中的输入信息、中间结果与输出结果之间的相互校验，从而形成更立体的验证网络。这种机制能够有效抑制不确定性的放大，从而减少人类的干预频率，使得 AI 表现得更加智能与仿生。这也是 AI 持续朝多模态方向演进的重要底层逻辑之一。

- **AI 的局限性**：由于提示词的局限以及模型本身基于概率分布的采样机制，AI 初始的先验判断往往过于宽泛。在多步自回归生成过程中，这种内在的随机性容易导致语义偏移和幻觉的持续累积。

- **人类角色的动态变化**：人类作为"高维观测者"，拥有最丰富的隐性知识（Tacit Knowledge）。随着 AI 能力提升以及 **Harness** 承担更多底层验证任务，人类直接参与局部决策与低层纠错的比例可以逐步下降；但在目标定义、价值判断与最终裁决层面，人类在相当长一段时间内仍将发挥关键作用。这里的关键并不在于让人类频繁介入所有节点，而在于保留对任意节点的干预权限，并尽可能智能地识别那些真正需要人类注入确定性的"关键靶点"——即验证网络暂时无法覆盖、经过验证后仍残留偏移、或一旦失控就可能引发连锁放大的高杠杆节点。

- **关键靶点识别与最小代价稳定性**：从系统设计角度看，更有价值的目标不是简单增加人工参与次数，而是以尽可能小的观测、验证与交互成本，识别最可能决定全局稳定性的少数关键节点。若大多数常规节点已经能够被模型能力与验证网络自动纠偏，那么系统的稳定性上限将越来越取决于：能否及时发现那些少量但高影响的残余偏移，并在必要时引入人类的高置信度证据或裁决，以避免局部误差在长链路任务中演化为"蝴蝶效应式"的全局偏移。

- **混合系统中的智能化比例与三类控制**：在这一框架下，一个更精确的观察视角，是看三类控制的占比如何随 AI 能力成熟而动态演变：**模型自主控制与 Harness 反馈控制**的占比越高，说明系统越接近高水平的智能协同；**人为修正控制**的占比越高，系统则越接近传统工具范式。在结果质量、验证能力与责任边界可接受的前提下，这一比例变化——人为修正控制在正确决策中的占比能否持续下降——是衡量系统智能化水平的核心量化指标。

- **多模态与跨维验证**：当文本、运行结果、日志、文件结构、视觉、听觉、触觉或其他传感反馈被纳入同一闭环时，系统可以借助 **Harness** 对不同维度进行交叉验证，从而缓解单一维度验证的压力，并降低人类介入频率。这里的"验证"不仅包括不同维度最终结果之间的核对，也包括不同维度中的输入信息、中间结果与输出结果之间的相互校验，从而形成更立体的验证网络。例如在 IDE 场景中，代码文本、脚本运行、自动化测试、结果输出与结果验证，可以共同构成对"某个假设是否成立"的多维验证；从这个角度看，它们本身就是 **Harness** 与多模态、多维验证机制的一部分。

- **动态可验证性与分层验证策略**：并非所有推理节点都需要同等强度的验证。短链任务中，模型自主控制往往已足够兜底，过度验证反而降低效率；长链任务中，不确定性随步数累积放大，需要 Harness 反馈控制与多维交叉验证逐层加码。这一分层策略，本质上是对三类控制资源的动态配置：在低风险区段，让模型自主控制占据主导；在高风险区段，激活 Harness 反馈控制与人为修正控制的组合验证。这种按风险梯度的验证资源分配，是提升系统整体效率与稳定性的重要设计原则。

- **人机协同收敛**：通过 UI 层面的控制，人类不断输入高置信度的证据以剪枝推理路径；AI 则依据「先验 → 条件/证据 → 后验判断 → 执行 → 结果 → 验证 → 反馈 →（迭代）」的动态循环框架持续更新判断——验证结果自动回注为新证据，驱动下一轮迭代。这套逻辑闭环为缓解大模型难以稳定自我纠偏的问题提供了一种可操作路径。

---

## 🚀 核心特性

- [ ] **动态循环节点可视化**：将复杂的 Prompt 拆解为可视化的完整动态循环节点——先验、条件/证据、后验判断、执行、结果、验证、反馈——覆盖从认知到执行到验证的全链路。
- [ ] **推理方向锁定**：通过拖拽或参数调整，强制 AI 沿着指定概率路径探索。
- [ ] **动态贝叶斯式更新**：实时反映新证据加入后，AI 判断与推理路径的变化。
- [ ] **多步纠偏回溯**：随时回退到任意概率分叉点，修改条件重新生成。
- [ ] **主动假设与鉴别提问**：在信息不足时，AI 自动生成多分支假设，并主动向人类发问以获取关键证据。
- [ ] **多模态证据闭环与一票否决**：联合文本、运行结果、日志与传感反馈进行交叉验证，客观"硬证据"可一票否决错误假设，缓解单一模态的信息瓶颈。
- [ ] **Harness 集成验证**：将脚本运行、自动化测试与外部工具反馈纳入同一验证闭环，降低人类持续介入频率。
- [ ] **动态可验证性——分层验证**：根据推理步骤数量与任务风险，动态调整验证强度——短链放宽、长链加码，实现效率与稳定性的最优平衡。

---

## 🤔 哲学思考：这是否是一种倒退？

人们可能会问：**目前的行业趋势都在追求"全自动智能体（Auto-Agent）"，CB-Paradigm 重新引入人类的强干预，将全自动退回到"半自动（Human-in-the-loop）"，这是否是一种历史的倒退？**

我的理解是：**这或许并非倒退，而是人机协同演进过程中的一种"角色升维"。**

1. **"假全自动"的代价是失控**：当前的大语言模型在执行长链路、复杂的真实业务时，所谓的"全自动"往往意味着在错误的中间假设上盲目狂奔。在某些复杂场景下，缺乏人类校准的全自动有时会面临置信度与良率的挑战。

2. **人类角色的升维，而非增加负担**：在传统的"半自动"时代，人类是具体的执行者（工人）；而在 CB-Paradigm 中，借助 **模型自主控制**（模型内在的自我纠偏能力）与 **Harness（工程护栏）** 处理底层验证与纠错，并结合多模态交叉验证，人类不再需要持续参与底层的生成劳动。人类有机会被升维为**"概率空间的导航员（Navigator）"**与**"高维观测者"**。AI 负责展开庞大的可能性推理树，人类仅在关键节点进行轻量级的"剪枝"与"条件注入"。随着模型能力与验证系统的提升，**模型自主控制与 Harness 反馈控制**的占比不断提高，人类介入的频率自然下降，但其在高维裁决中的作用仍然不可替代。

3. **确定性的最终来源（"甲方"定律）**：从根本上说，AI 只是解决人类需求的工具。既然需求的提出者（甲方）是人类，那么判定"什么是正确的、什么是有价值的"这一任务语境中的最终裁决依据，天然就应该主要由人类来提供和裁决。在彻底解决 AI 内部概率采样机制带来的熵增问题之前，人类的高维隐性知识，将始终是复杂系统的重要外部确定性来源。若希望将人类在正确决策中的占比进一步压低到接近于零，其障碍也将不再只是技术上的不确定性控制问题，而会进一步进入责任归属与伦理承担的问题域。

---

## 🔄 Loop Engineering

> **Loop Engineering（循环工程）**是 2025–2026 年在 AI Agent 工程领域兴起的新范式：从逐轮编写 Prompt，转向设计自主运行的 Agent 循环系统——该系统自动发现任务、规划、执行、验证，并在调度器上持续迭代，直至达到可验证的停止条件。

### 相同点：CB-Chat 与 Loop Engineering 的共性

| 维度 | 共同立场 |
|------|---------|
| **验证的承重地位** | 两者都认为"没有验证的循环只是自动化"（SonarSource）。CB-Chat 的 **Harness 反馈控制**与 Loop Engineering 的 **Verification Loop** 服务于同一目标：自动化、可复现的正确性检查。 |
| **多步推理的稳定性** | 两者都针对同一个核心问题：LLM 的单次输出在长推理链中会持续退化。Loop Engineering 将任务拆解为 Plan→Execute→Verify 循环；CB-Chat 将每个推理步骤可视化为完整的「先验→证据→后验→执行→结果→验证→反馈」动态循环节点。 |
| **Human-in-the-Loop** | 两者都承认全自主 Agent 需要在关键节点引入人类干预。Loop Engineering 的 HITL 模式与 CB-Chat 的 **人为修正控制**共享同一前提。 |
| **迭代至收敛** | 两者都拒绝一次性 Prompt。CB-Chat 的动态贝叶斯更新与 Loop Engineering 的"迭代至条件满足"是同一循环原理。 |
| **Harness / 工程护栏** | CB-Chat 的 **Harness**（工程验证护栏）与 Orange Book 四层架构中的 Harness 层直接对应。 |

### 关键区别：预设条件 vs. 中途动态介入

这是 CB-Chat 与 Loop Engineering 的根本分歧：

| | Loop Engineering | CB-Chat |
|---|---|---|
| **核心假设** | 条件和目标可以在设计阶段被充分预设 | 预设条件在复杂任务中**永远不可能完备**——不确定性必然在执行中途浮现 |
| **人类介入的时间窗口** | 设计时（设置 Loop）+ 审批时（二元：批准/拒绝） | **任意推理节点、任意时刻**——一个连续的介入谱系 |
| **介入粒度** | 操作级（批准/拒绝某个工具调用） | **节点级**（在特定推理节点上修改先验、注入证据、锁定方向） |
| **对不确定性的覆盖** | 依赖预设条件 + 验证环来压制不确定性 | 承认不确定性不可完全压制 → 保留每个节点的动态介入通道 |
| **概念本质** | **自动化工程框架**——设计好 Loop 后离开 | **不确定性管理框架**——在真正重要的精度上保持介入 |

核心洞察：**Loop Engineering 先设置好所有条件和目标，然后让 Agent 在边界内自主探索。但预设条件永远无法在复杂任务中完全覆盖并抑制不确定性。**当不确定性在执行中途不可避免地浮现——在某个预设验证规则无法捕获语义漂移的推理节点上——Loop Engineering 缺乏原生的精准介入机制。人类要么等待循环跑完（在错误分支上浪费 Token），要么杀死循环并重启（丢失上下文）。

CB-Chat 恰恰是为填补这一空白而设计的：它同时覆盖**预设阶段**（条件、目标、验证规则）**和运行中途阶段**（当不确定性溢出预设护栏时，进行动态节点级介入）。这不是一种互补补充——而是一种**概念上的超集**：CB-Chat 的介入模型包含了 Loop Engineering 的预设方法，并将其扩展至实时、节点粒度、推理级别的控制。

### CB-Chat 在 Loop Engineering 谱系中的定位

```
Prompt Engineering  →  Agentic Workflows  →  Loop Engineering  →  CB-Paradigm
(单次提示)              (多步骤)               (自主循环)            (可控循环)
                                                         │
                                              预设条件 + 自主执行
                                                         │
                                              ─ ─ ─ 空白区 ─ ─ ─
                                                         │
                                              不确定性在执行中途
                                              溢出预设护栏
                                                         │
                                                         ▼
                                              CB-Chat：动态节点级
                                              人类确定性注入
```

这就是为什么 CB-Chat 不仅是"带有更好 UI 的 Loop Engineering"。它解决的是 Loop Engineering 范式中一个**结构性的盲区**：假设预设条件和验证规则可以预见并遏制复杂长程推理任务中的所有不确定性形式。

---

## 📜 License & Citation · 许可与引用

This project is released under the **MIT License**, allowing others to use, modify, and distribute the related code and documentation as long as the original copyright notice and license text are preserved.

If this project, its conceptual framing (such as **CB-Chat**, **CB-Paradigm**, and related derived concepts), or its documentation is helpful to your work, attribution is appreciated. This request is made mainly in the spirit of academic and open-source courtesy and **is not a mandatory requirement of the MIT License itself**.

For formal citation, please refer to the [`CITATION.cff`](CITATION.cff) file in the root of the repository.

---

本项目采用 **MIT License** 发布，以便他人在保留原始版权与许可声明的前提下使用、修改和分发相关代码与文档。

如果本项目、其概念框架（如 **CB-Chat**、**CB-Paradigm** 及相关衍生概念）或其文档表达对你的工作有帮助，欢迎注明来源。需要说明的是，这一署名请求主要是出于学术与开源协作礼仪的考虑，**并不是 MIT 协议本身的强制条款**。

如需正式引用本项目，建议参考仓库根目录中的 [`CITATION.cff`](CITATION.cff)。
