# 语音 / 音频 / 音乐论文速递
## 2026-05-03

> 实际对应 arXiv 更新日：**2026-05-03**  
> 检索范围：`cs.SD + eess.AS`  
> 只放按 ML 顶会审稿口径看，最值得多数读者花时间看的 **5 篇**

## 📋 总览

- 共收录 **5 篇** 相关论文
- 语音大模型：**1 篇**
- 语音前端：**1 篇**
- 音乐生成/理解：**3 篇**

今天真正值得看的主线有三条。第1条主线是 `TMD-Bench`，重点在 2 Related Work 2.1 Music-Driven Human Motion Synthesi… 第2条主线是 `Khala`，重点在 1.1 Background and Motivation 1.2 Key Challenges 1.3… 第3条主线是 `Mitigating Multimodal LLMs Hallucinations via Relevance Propagation at Inference Time`，重点在 2 Related Work 3 Method 3.1 Notation and Setup 3.2 Re…

## 精选入选规则

- **新意（0-3）**：有没有新方法、新任务设定或明确新范式
- **影响力（0-3）**：是不是主线问题，不是特别窄的小点
- **证据强度（0-2）**：实验、对比、消融、结论是否站得住
- **受众匹配度（0-2）**：是否贴近语音大模型、语音识别、TTS、音乐生成、音频系统

分数校准：

- **6**：可读，但偏 incremental
- **7**：接近 strong accept，不是随手送分
- **8+**：当天明显强稿才配拿

## 总览表

| 方向 | 序号 | 论文 | 评分 | 关键词 |
|---|---:|---|---:|---|
| 音乐生成/理解 | 1 | TMD-Bench: A Multi-Level Evaluation Paradigm for Music-Dance Co-Generation | 8/10 | References A Dataset Construction Details…, Audio–video data processing for rhythmic…, 整体框架: 从全文抽到的是任务级框架，不再只报空泛大类。 |
| 音乐生成/理解 | 2 | Khala: Scaling Acoustic Token Language Models Toward High-Fidelity Music Generation | 7/10 | References License: arXiv.org perpetual n…, In this work, we explore an alternative v…, 输入/条件: Introduction 1.1 Background and Mo… |
| 语音大模型 | 3 | Mitigating Multimodal LLMs Hallucinations via Relevance Propagation at Inference Time | 7/10 | References A Layer-wise Relevance Propaga…, LRP for softmax normalization., 整体框架: 语音/音频大模型主干，倾向统一建模或多模态对齐，不是传统单模块前端。 |
| 语音前端 | 4 | Spoken Language Identification with Pre-trained Models and Margin Loss | 6/10 | Acknowledgments References License: arXiv…, Zhihua Liang Weiwu School of Computer Sci…, 整体框架: 前端鲁棒建模 + 下游识别/增强/分离目标联合优化。 |
| 音乐生成/理解 | 5 | RenCon 2025: Revival of the Expressive Performance Rendering Competition | 5/10 | Acknowledgments 11 Ethical Standards Refe…, 整体框架: 从全文抽到的是任务级框架，不再只报空泛大类。, 关键模块: Report, GitHub, Issue, Title, Conte… |

## 🎼 音乐生成 / 音乐理解

### [1] TMD-Bench: A Multi-Level Evaluation Paradigm for Music-Dance Co-Generation

- **评分**：8/10
- **作者/机构**：Xiaoda Yang, Majun Zhang, Changhao Pan, Nick Huang, Yang Yuguang, Fan Zhuo, Pengfei Zhou, Jin Zhou；暂无
- **论文链接**：http://arxiv.org/abs/2605.01809v1
- **PDF**：https://arxiv.org/pdf/2605.01809v1.pdf
- **代码链接**：暂无
- **Demo 链接**：https://huggingface.co/huggingface

#### 📌 简介
2 Related Work 2.1 Music-Driven Human Motion Synthesis 2.2 Unified Audio-Video Joint Generation 3 TMD-Bench 3.1 Audio Evaluation 3.2 Video Evaluation 3.3 Audio–Visual Alignment Ev…

#### ☠️ 毒舌点评
大模型味很重，关键不是会不会讲故事，而是有没有把语音侧真正难点啃下来。没有硬消融就别急着神化。

#### 🔧 技术方案
- **模型解决的问题**：2 Related Work 2.1 Music-Driven Human Motion Synthesis 2.2 Unified Audio-Video Joint Generation 3 TMD-Bench 3.1 Audio Evaluation 3.2 Video…
- **模型架构**：
  输入/条件：整体框架: 从全文抽到的是任务级框架，不再只报空泛大类。
  整体框架：关键模块: Report, GitHub, Issue, Title, Content
  关键模块：References A Dataset Construction Details Pure-music data processing.
- **训练 / 推理策略**：训练细节没有空着，但自动抽取到的损失/增广/训练阶段仍不够稳定。

#### 📊 实验结果
- 数据集：Experiments, Dataset, Processing, Experimental
- 主要结果：数据集: Experiments, Dataset, Processing, Experimental, Settings
- baseline 对比：已读实验段，但基线名抽取不稳。
- 是否开源：暂未明确

### [2] Khala: Scaling Acoustic Token Language Models Toward High-Fidelity Music Generation

- **评分**：7/10
- **作者/机构**：Jiafeng Liu, Yuanliang Dong, Hongjia Liu, Yuqing Cheng, Zhancheng Guo, Huijing Liang, Wenbo Zhan, Yuming Sun；暂无
- **论文链接**：http://arxiv.org/abs/2605.01790v1
- **PDF**：https://arxiv.org/pdf/2605.01790v1.pdf
- **代码链接**：暂无
- **Demo 链接**：https://huggingface.co/huggingface

#### 📌 简介
1.1 Background and Motivation 1.2 Key Challenges 1.3 Overview of Our Approach 1.4 Contributions 2 Related Work 2.1 Audio Representations for Music Generation 2.2 Music Generation…

#### ☠️ 毒舌点评
这个方向最怕花哨 pipeline 换皮。要看它是否真的解决了音质、可控性或泛化，而不是只挑顺手样本。

#### 🔧 技术方案
- **模型解决的问题**：1.1 Background and Motivation 1.2 Key Challenges 1.3 Overview of Our Approach 1.4 Contributions 2 Related Work 2.1 Audio Representations fo…
- **模型架构**：
  输入/条件：输入/条件: Introduction 1.1 Background and Motivation 1.2 Key Challenges 1.3 Overview of Our Approach 1.4 Contributions 2 R…
  整体框架：整体框架: 从全文抽到的是任务级框架，不再只报空泛大类。
  关键模块：关键模块: Report, GitHub, Issue, Title, Content
- **训练 / 推理策略**：训练细节没有空着，但自动抽取到的损失/增广/训练阶段仍不够稳定。

#### 📊 实验结果
- 数据集：已读实验段，但命名抽取不稳。
- 主要结果：Experiments 6.1 Human Arena Evaluation 6.2 Ablations on Alignment and Initialization 7 Discussion 8 Conclusion References License: arXiv.org perpetua…
- baseline 对比：已读实验段，但基线名抽取不稳。
- 是否开源：暂未明确

### [3] RenCon 2025: Revival of the Expressive Performance Rendering Competition

- **评分**：5/10
- **作者/机构**：Huan Zhang, Taegyun Kwon, Anders Friburg, Junyan Jiang, Hayeon Bang, Hyeyoon Cho, Gus Xia, Akira Maezawa；暂无
- **论文链接**：http://arxiv.org/abs/2605.02059v1
- **PDF**：https://arxiv.org/pdf/2605.02059v1.pdf
- **代码链接**：暂无
- **Demo 链接**：https://huggingface.co/huggingface

#### 📌 简介
2 Past Competitions 3 Competition Design 3.1 Phase 1: Preliminary Round (Online) 3.2 Phase 2: Live Contest 3.2.1 Venue Details 3.2.2 Disklavier Calibration 4 Evaluation 4.1 Prelim…

#### ☠️ 毒舌点评
这个方向最怕花哨 pipeline 换皮。要看它是否真的解决了音质、可控性或泛化，而不是只挑顺手样本。

#### 🔧 技术方案
- **模型解决的问题**：2 Past Competitions 3 Competition Design 3.1 Phase 1: Preliminary Round (Online) 3.2 Phase 2: Live Contest 3.2.1 Venue Details 3.2.2 Diskla…
- **模型架构**：
  输入/条件：整体框架: 从全文抽到的是任务级框架，不再只报空泛大类。
  整体框架：关键模块: Report, GitHub, Issue, Title, Content
  关键模块：10 Acknowledgments 11 Ethical Standards References License: CC BY 4.0 arXiv:2605.02059v1 [cs.MM] 03 May 2026 \setcopyri…
- **训练 / 推理策略**：训练细节没有空着，但自动抽取到的损失/增广/训练阶段仍不够稳定。

#### 📊 实验结果
- 数据集：已读实验段，但命名抽取不稳。
- 主要结果：实验段已读取，但自动抽到的硬指标和对比项仍偏弱。
- baseline 对比：已读实验段，但基线名抽取不稳。
- 是否开源：暂未明确


## 🤖 语音大模型 / 语音理解

### [4] Mitigating Multimodal LLMs Hallucinations via Relevance Propagation at Inference Time

- **评分**：7/10
- **作者/机构**：Itai Allouche, Joseph Keshet；Mitigating Multimodal LLMs Hallucinations via Relevance Propagation at Inference Time /
- **论文链接**：http://arxiv.org/abs/2605.01766v1
- **PDF**：https://arxiv.org/pdf/2605.01766v1.pdf
- **代码链接**：暂无
- **Demo 链接**：https://huggingface.co/huggingface

#### 📌 简介
2 Related Work 3 Method 3.1 Notation and Setup 3.2 Relevance and Problem Formulation 3.3 Inference-Time Optimization 4 Experiments 4.1 Vision Benchmarks 4.2 Audio Benchmarks 4.3 M…

#### ☠️ 毒舌点评
大模型味很重，关键不是会不会讲故事，而是有没有把语音侧真正难点啃下来。没有硬消融就别急着神化。

#### 🔧 技术方案
- **模型解决的问题**：2 Related Work 3 Method 3.1 Notation and Setup 3.2 Relevance and Problem Formulation 3.3 Inference-Time Optimization 4 Experiments 4.1 Visi…
- **模型架构**：
  输入/条件：整体框架: 语音/音频大模型主干，倾向统一建模或多模态对齐，不是传统单模块前端。
  整体框架：关键模块: Report, GitHub, Issue, Title, Content
  关键模块：References A Layer-wise Relevance Propagation for Transformer Models LRP- ϵ \epsilon rule.
- **训练 / 推理策略**：训练细节没有空着，但自动抽取到的损失/增广/训练阶段仍不够稳定。

#### 📊 实验结果
- 数据集：Experiments, Vision, Benchmarks, Audio
- 主要结果：数据集: Experiments, Vision, Benchmarks, Audio, Modality
- baseline 对比：已读实验段，但基线名抽取不稳。
- 是否开源：暂未明确


## 🧩 语音前端 / ASR / 检测

### [5] Spoken Language Identification with Pre-trained Models and Margin Loss

- **评分**：6/10
- **作者/机构**：Zhihua Fang, Liang He, Weiwu Jiang；暂无
- **论文链接**：http://arxiv.org/abs/2605.01905v1
- **PDF**：https://arxiv.org/pdf/2605.01905v1.pdf
- **代码链接**：**已开源** **代码已开源**: https://github.com/PunkMale/TidyLang2026
- **Demo 链接**：https://huggingface.co/huggingface

#### 📌 简介
2 Preliminaries 2.1 Challenge Description and Dataset 2.2 Baseline System 3 Method 3.1 Pre-trained ECAPA-TDNN Encoder 3.2 Margin-based Classification Heads 3.2.1 Additive Angular…

#### ☠️ 毒舌点评
全文看下来不像完全糊弄，但也没到一眼封神。值不值得跟，主要看你是不是正做这条子方向。

#### 🔧 技术方案
- **模型解决的问题**：2 Preliminaries 2.1 Challenge Description and Dataset 2.2 Baseline System 3 Method 3.1 Pre-trained ECAPA-TDNN Encoder 3.2 Margin-based Clas…
- **模型架构**：
  输入/条件：整体框架: 前端鲁棒建模 + 下游识别/增强/分离目标联合优化。
  整体框架：关键模块: Report, GitHub, Issue, Title, Content
  关键模块：6 Acknowledgments References License: arXiv.org perpetual non-exclusive license arXiv:2605.01905v1 [cs.SD] 03 May 2026…
- **训练 / 推理策略**：损失/目标: Report Issue Back to Abstract Download PDF <a class="header-button toggle-icon" href="javascript:toggle Experiments 4.1 Experimental…

#### 📊 实验结果
- 数据集：Experimental, Tidy-X, EER
- 主要结果：数据集: Experimental, Tidy-X, EER
- baseline 对比：Compared, EER
- 是否开源：是


## 最后结论

如果只让我排今天最值得优先看的 3 篇，会是：

1. **TMD-Bench**
References A Dataset Construction Details Pure-music data processing.
2. **Khala**
References License: arXiv.org perpetual non-exclusive license arXiv:2605.01790v1 [cs.SD] 03 May 2026 Khala: Scaling Aco…
3. **Mitigating Multimodal LLMs Hallucinations via Relevance Propagation at Inference Time**
References A Layer-wise Relevance Propagation for Transformer Models LRP- ϵ \epsilon rule.
