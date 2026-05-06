# 语音 / 音频 / 音乐论文速递
## 2026-05-02

> 实际对应 arXiv 更新日：**2026-05-02**  
> 检索范围：`cs.SD + eess.AS`  
> 只放按 ML 顶会审稿口径看，最值得多数读者花时间看的 **5 篇**

## 📋 总览

- 共收录 **5 篇** 相关论文
- 语音大模型：**1 篇**
- 语音/歌声生成：**1 篇**
- 音乐生成/理解：**1 篇**
- 其他音频方向：**2 篇**

今天真正值得看的主线有三条。第1条主线是 `MG-Former`，重点在 2 Related Work 2.1 3D Dance Generation 2.2 3D Gesture… 第2条主线是 `MindMelody`，重点在 2 Related Work 2.1 EEG Decoding 2.2 Affect-to-Plan 2.… 第3条主线是 `Multimodal Confidence Modeling in Audio-Visual Quality Assessment`，重点在 2 Methodology 3 Experimental Results 4 Ablation Studi…

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
| 音乐生成/理解 | 1 | MG-Former: A Transformer-Based Framework for Music-Driven 3D Conducting Gesture Generation | 8/10 | References License: CC BY 4.0 arXiv:2605.…, Tianzhi Jia Beijing Jiaotong University j…, 整体框架: 从全文抽到的是任务级框架，不再只报空泛大类。 |
| 语音大模型 | 2 | MindMelody: A Closed-Loop EEG-Driven System for Personalized Music Intervention | 7/10 | References License: arXiv.org perpetual n…, Driven by the escalating global burden of…, 整体框架: 语音/音频大模型主干，倾向统一建模或多模态对齐，不是传统单模块前端。 |
| 其他音频方向 | 3 | Multimodal Confidence Modeling in Audio-Visual Quality Assessment | 7/10 | References License: arXiv.org perpetual n…, In realistic streaming scenarios, distort…, 输入/条件: The Audio–Visual Mixer utilizes fr… |
| 其他音频方向 | 4 | Toward Fair Speech Technologies: A Comprehensive Survey of Bias and Fairness in Speech AI | 6/10 | References License: CC BY-SA 4.0 arXiv:26…, Huang-Cheng Chou is with the University o…, 整体框架: 从全文抽到的是任务级框架，不再只报空泛大类。 |
| 语音/歌声生成 | 5 | MelShield: Robust Mel-Domain Audio Watermarking for Provenance Attribution of AI Generated Synthesized Speech | 6/10 | References License: arXiv.org perpetual n…, Specifically, MelShield operates in the M…, 输入/条件: 2.3 Mel-Spectrogram 3 Problem Form… |

## 🎼 音乐生成 / 音乐理解

### [1] MG-Former: A Transformer-Based Framework for Music-Driven 3D Conducting Gesture Generation

- **评分**：8/10
- **作者/机构**：Ke Qiu, Yawen Qin, Tianzhi Jia, Xiaole Yang, Kaimin Wang, Kaixing Yang；暂无
- **论文链接**：http://arxiv.org/abs/2605.01197v1
- **PDF**：https://arxiv.org/pdf/2605.01197v1.pdf
- **代码链接**：暂无
- **Demo 链接**：https://huggingface.co/huggingface

#### 📌 简介
2 Related Work 2.1 3D Dance Generation 2.2 3D Gesture Generation 2.3 Conducting Motion Generation 3 Dataset 3.1 Motivation 3.2 Data Collection Pipeline 3.3 Audio and Temporal Alig…

#### ☠️ 毒舌点评
不像纯标题党，至少方法和实验都在往完整论文靠。但是否真创新，还得盯住它是不是把老模块重新拼了一遍。

#### 🔧 技术方案
- **模型解决的问题**：2 Related Work 2.1 3D Dance Generation 2.2 3D Gesture Generation 2.3 Conducting Motion Generation 3 Dataset 3.1 Motivation 3.2 Data Collect…
- **模型架构**：
  输入/条件：整体框架: 从全文抽到的是任务级框架，不再只报空泛大类。
  整体框架：关键模块: Report, GitHub, Issue, Title, Content
  关键模块：References License: CC BY 4.0 arXiv:2605.01197v1 [cs.SD] 02 May 2026 MG-Former: A Transformer-Based Framework for Music…
- **训练 / 推理策略**：训练细节没有空着，但自动抽取到的损失/增广/训练阶段仍不够稳定。

#### 📊 实验结果
- 数据集：已读实验段，但命名抽取不稳。
- 主要结果：对比基线: Experiments, Settings, Comparison, Study, Ablation
- baseline 对比：Experiments, Settings, Comparison, Study
- 是否开源：暂未明确


## 🤖 语音大模型 / 语音理解

### [2] MindMelody: A Closed-Loop EEG-Driven System for Personalized Music Intervention

- **评分**：7/10
- **作者/机构**：Yimeng Zhang, Yueru Sun, Haoyu Gu；暂无
- **论文链接**：http://arxiv.org/abs/2605.01235v1
- **PDF**：https://arxiv.org/pdf/2605.01235v1.pdf
- **代码链接**：暂无
- **Demo 链接**：https://huggingface.co/huggingface

#### 📌 简介
2 Related Work 2.1 EEG Decoding 2.2 Affect-to-Plan 2.3 Controllable Music 3 Method 3.1 Overall Framework 3.2 Affect Encoder 3.3 Intervention Planner 3.4 EEG Control Module 3.5 Tra…

#### ☠️ 毒舌点评
不像纯标题党，至少方法和实验都在往完整论文靠。但是否真创新，还得盯住它是不是把老模块重新拼了一遍。

#### 🔧 技术方案
- **模型解决的问题**：2 Related Work 2.1 EEG Decoding 2.2 Affect-to-Plan 2.3 Controllable Music 3 Method 3.1 Overall Framework 3.2 Affect Encoder 3.3 Interventio…
- **模型架构**：
  输入/条件：整体框架: 语音/音频大模型主干，倾向统一建模或多模态对齐，不是传统单模块前端。
  整体框架：关键模块: Report, GitHub, Issue, Title, Content
  关键模块：References License: arXiv.org perpetual non-exclusive license arXiv:2605.01235v1 [cs.SD] 02 May 2026 MindMelody: A Clos…
- **训练 / 推理策略**：训练细节没有空着，但自动抽取到的损失/增广/训练阶段仍不够稳定。

#### 📊 实验结果
- 数据集：Experiments, Setup, Datasets, Hyperparameters
- 主要结果：数据集: Experiments, Setup, Datasets, Hyperparameters, Metrics
- baseline 对比：已读实验段，但基线名抽取不稳。
- 是否开源：暂未明确


## 🔊 其他音频方向

### [3] Multimodal Confidence Modeling in Audio-Visual Quality Assessment

- **评分**：7/10
- **作者/机构**：Mayesha Maliha R. Mithila, Mylene C. Q. Farias；暂无
- **论文链接**：http://arxiv.org/abs/2605.01219v1
- **PDF**：https://arxiv.org/pdf/2605.01219v1.pdf
- **代码链接**：暂无
- **Demo 链接**：https://huggingface.co/huggingface

#### 📌 简介
2 Methodology 3 Experimental Results 4 Ablation Studies 5 Conclusion References License: arXiv.org perpetual non-exclusive license arXiv:2605.01219v1 [cs.MM] 02 May 2026 Multimoda…

#### ☠️ 毒舌点评
全文看下来不像完全糊弄，但也没到一眼封神。值不值得跟，主要看你是不是正做这条子方向。

#### 🔧 技术方案
- **模型解决的问题**：2 Methodology 3 Experimental Results 4 Ablation Studies 5 Conclusion References License: arXiv.org perpetual non-exclusive license arXiv:26…
- **模型架构**：
  输入/条件：输入/条件: The Audio–Visual Mixer utilizes frame-level, confidence-guided channel attention to gate fusion, modulating feat…
  整体框架：整体框架: 从全文抽到的是任务级框架，不再只报空泛大类。
  关键模块：关键模块: Report, GitHub, Issue, Title, Content
- **训练 / 推理策略**：损失/目标: In contrast, the audio may be degraded by coding distortion or packet loss, while visual quality is mostly preserved [ 2 ] .

#### 📊 实验结果
- 数据集：Experiments, AVQA, MCM-AVQA, Audio
- 主要结果：数据集: Experiments, AVQA, MCM-AVQA, Audio, Visual
- baseline 对比：已读实验段，但基线名抽取不稳。
- 是否开源：暂未明确

### [4] Toward Fair Speech Technologies: A Comprehensive Survey of Bias and Fairness in Speech AI

- **评分**：6/10
- **作者/机构**：Yi-Cheng Lin, Yun-Shao Tsai, Kuan-Yu Chen, Hsiao-Ying Huang, Huang-Cheng Chou, Hung-yi Lee；暂无
- **论文链接**：http://arxiv.org/abs/2605.01597v1
- **PDF**：https://arxiv.org/pdf/2605.01597v1.pdf
- **代码链接**：暂无
- **Demo 链接**：https://huggingface.co/huggingface

#### 📌 简介
I-A Uniqueness of speech modality in fairness I-B Difference from Prior Surveys I-C Main Contributions II Background II-A Social Bias II-A 1 The Mechanisms of Social Bias II-A 2 T…

#### ☠️ 毒舌点评
全文看下来不像完全糊弄，但也没到一眼封神。值不值得跟，主要看你是不是正做这条子方向。

#### 🔧 技术方案
- **模型解决的问题**：I-A Uniqueness of speech modality in fairness I-B Difference from Prior Surveys I-C Main Contributions II Background II-A Social Bias II-A…
- **模型架构**：
  输入/条件：整体框架: 从全文抽到的是任务级框架，不再只报空泛大类。
  整体框架：关键模块: Report, GitHub, Issue, Title, Content
  关键模块：References License: CC BY-SA 4.0 arXiv:2605.01597v1 [eess.AS] 02 May 2026 \useforestlibrary edges Toward Fair Speech Te…
- **训练 / 推理策略**：训练细节没有空着，但自动抽取到的损失/增广/训练阶段仍不够稳定。

#### 📊 实验结果
- 数据集：已读实验段，但命名抽取不稳。
- 主要结果：Per-group comparisons extend beyond ASR to SV using EER, FMR, and FNMR [ 149 , 91 ] , speaker diarization using DER [ 362 ] , deepfake detection usin…
- baseline 对比：Per-group, ASR, EER, FMR
- 是否开源：暂未明确


## 🗣️ TTS / 歌声生成

### [5] MelShield: Robust Mel-Domain Audio Watermarking for Provenance Attribution of AI Generated Synthesized Speech

- **评分**：6/10
- **作者/机构**：Yutong Jin, Qi Li, Lingshuang Liu, Jianbing Ni；暂无
- **论文链接**：http://arxiv.org/abs/2605.01515v1
- **PDF**：https://arxiv.org/pdf/2605.01515v1.pdf
- **代码链接**：暂无
- **Demo 链接**：https://huggingface.co/huggingface

#### 📌 简介
2 Preliminaries 2.1 TTS Pipelines and Neural Vocoders Diffusion-based vocoders. Relevance to this work.

#### ☠️ 毒舌点评
全文看下来不像完全糊弄，但也没到一眼封神。值不值得跟，主要看你是不是正做这条子方向。

#### 🔧 技术方案
- **模型解决的问题**：2 Preliminaries 2.1 TTS Pipelines and Neural Vocoders Diffusion-based vocoders.
- **模型架构**：
  输入/条件：输入/条件: 2.3 Mel-Spectrogram 3 Problem Formulation Security and Performance Objectives.
  整体框架：整体框架: 生成式声学建模主干，通常是 codec / diffusion / AR-NAR 一类。
  关键模块：关键模块: Report, GitHub, Issue, Title, Content
- **训练 / 推理策略**：训练细节没有空着，但自动抽取到的损失/增广/训练阶段仍不够稳定。

#### 📊 实验结果
- 数据集：Experiments, Experimental, Setup, Datasets
- 主要结果：数据集: Experiments, Experimental, Setup, Datasets, TTS
- baseline 对比：已读实验段，但基线名抽取不稳。
- 是否开源：暂未明确


## 最后结论

如果只让我排今天最值得优先看的 3 篇，会是：

1. **MG-Former**
References License: CC BY 4.0 arXiv:2605.01197v1 [cs.SD] 02 May 2026 MG-Former: A Transformer-Based Framework for Music…
2. **MindMelody**
References License: arXiv.org perpetual non-exclusive license arXiv:2605.01235v1 [cs.SD] 02 May 2026 MindMelody: A Clos…
3. **Multimodal Confidence Modeling in Audio-Visual Quality Assessment**
References License: arXiv.org perpetual non-exclusive license arXiv:2605.01219v1 [cs.MM] 02 May 2026 Multimodal Confide…
