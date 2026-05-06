# 语音 / 音频 / 音乐论文速递
## 2026-05-01

> 实际对应 arXiv 更新日：**2026-05-01**  
> 检索范围：`cs.SD + eess.AS`  
> 只放按 ML 顶会审稿口径看，最值得多数读者花时间看的 **5 篇**

## 📋 总览

- 共收录 **5 篇** 相关论文
- 音乐生成/理解：**1 篇**
- 其他音频方向：**4 篇**

今天真正值得看的主线有三条。第1条主线是 `MedMosaic`，重点在 remain domain-specialized, with distinct model famili… 第2条主线是 `GaMMA`，重点在 In this paper, we propose GaMMA, a state-of-the-art (… 第3条主线是 `MMAudio-LABEL`，重点在 2 MMAudio-LABEL 2.1 Overview 2.2 Model Architecture 2…

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
| 其他音频方向 | 1 | MedMosaic: A Challenging Large Scale Benchmark of Diverse Medical Audio | 9/10 | s audio from GigaSpeech (Chen et al., 202…, Despite their diversity, these datasets d…, 输入/条件: Introduction remain domain-special… |
| 音乐生成/理解 | 2 | GaMMA: Towards Joint Global-Temporal Music Understanding in Large Multimodal Models | 9/10 | HTML 正文未形成可用抽取结果，当前只能暂时回退到 abstract，不把宣传句…, 信息不足，不能严肃下结构结论。 |
| 其他音频方向 | 3 | MMAudio-LABEL: Audio Event Labeling via Audio Generation for Silent Video | 8/10 | References License: arXiv.org perpetual n…, Practical applications, such as sound pro…, 整体框架: 从全文抽到的是任务级框架，不再只报空泛大类。 |
| 其他音频方向 | 4 | MMAudioReverbs: Video-Guided Acoustic Modeling for Dereverberation and Room Impulse Response Estimation | 8/10 | References License: arXiv.org perpetual n…, However, we hypothesize that such V2A mod…, 输入/条件: Introduction 2 Related Work 2.1 V2… |
| 其他音频方向 | 5 | Fast Text-to-Audio Generation with One-Step Sampling via Energy-Scoring and Auxiliary Contextual Representation Distillation | 8/10 | s and Future Work References A Energy-dis…, B Energy-distance loss calculation C Text…, 整体框架: 从全文抽到的是任务级框架，不再只报空泛大类。 |

## 🔊 其他音频方向

### [1] MedMosaic: A Challenging Large Scale Benchmark of Diverse Medical Audio

- **评分**：9/10
- **作者/机构**：Harshit Rajgarhia, Shuubham Ojha, Asif Shaik, Akhil Pothanapalli, Rachuri Lokesh, Abhishek Mukherji, Prasanna Desikan；暂无
- **论文链接**：http://arxiv.org/abs/2605.00969v1
- **PDF**：https://arxiv.org/pdf/2605.00969v1.pdf
- **代码链接**：暂无
- **Demo 链接**：https://huggingface.co/huggingface

#### 📌 简介
remain domain-specialized, with distinct model families for environmental sounds, speech, or music (e.g., Pengi (Desh- Reasoning over complex, structured inputs has become a mukh…

#### ☠️ 毒舌点评
全文看下来不像完全糊弄，但也没到一眼封神。值不值得跟，主要看你是不是正做这条子方向。

#### 🔧 技术方案
- **模型解决的问题**：remain domain-specialized, with distinct model families for environmental sounds, speech, or music (e.g., Pengi (Desh- Reasoning over compl…
- **模型架构**：
  输入/条件：输入/条件: Introduction remain domain-specialized, with distinct model families for environmental sounds, speech, or music…
  整体框架：整体框架: 从全文抽到的是任务级框架，不再只报空泛大类。
  关键模块：关键模块
- **训练 / 推理策略**：训练细节没有空着，但自动抽取到的损失/增广/训练阶段仍不够稳定。

#### 📊 实验结果
- 数据集：Such, Open-ended, Voice-based, Scalable
- 主要结果：数据集: Such, Open-ended, Voice-based, Scalable, Gemini-2
- baseline 对比：已读实验段，但基线名抽取不稳。
- 是否开源：暂未明确

### [2] MMAudio-LABEL: Audio Event Labeling via Audio Generation for Silent Video

- **评分**：8/10
- **作者/机构**：Kazuya Tateishi, Akira Takahashi, Atsuo Hiroe, Hirofumi Takeda, Shusuke Takahashi, Yuki Mitsufuji；LABEL: Audio Event Labeling via Audio Generation for Silent Video /
- **论文链接**：http://arxiv.org/abs/2605.00495v1
- **PDF**：https://arxiv.org/pdf/2605.00495v1.pdf
- **代码链接**：暂无
- **Demo 链接**：http://www.bibsonomy.org/BibtexHandler?requTask=upload&amp;url=https://arxiv.org/abs/2605.00495&amp;description=MMAudio-LABEL:

#### 📌 简介
2 MMAudio-LABEL 2.1 Overview 2.2 Model Architecture 2.3 Objective Functions 3 Experiments 3.1 Dataset and Downstream Tasks 3.2 Implementation Details 3.3 Results 4 Conclusion Refe…

#### ☠️ 毒舌点评
全文看下来不像完全糊弄，但也没到一眼封神。值不值得跟，主要看你是不是正做这条子方向。

#### 🔧 技术方案
- **模型解决的问题**：2 MMAudio-LABEL 2.1 Overview 2.2 Model Architecture 2.3 Objective Functions 3 Experiments 3.1 Dataset and Downstream Tasks 3.2 Implementati…
- **模型架构**：
  输入/条件：整体框架: 从全文抽到的是任务级框架，不再只报空泛大类。
  整体框架：关键模块: Report, GitHub, Issue, Title, Content
  关键模块：References License: arXiv.org perpetual non-exclusive license arXiv:2605.00495v1 [cs.SD] 01 May 2026 MMAudio-LABEL: Aud…
- **训练 / 推理策略**：训练细节没有空着，但自动抽取到的损失/增广/训练阶段仍不够稳定。

#### 📊 实验结果
- 数据集：Experiments, Dataset, Downstream, Tasks
- 主要结果：数据集: Experiments, Dataset, Downstream, Tasks, Implementation
- baseline 对比：Our
- 是否开源：暂未明确

### [3] MMAudioReverbs: Video-Guided Acoustic Modeling for Dereverberation and Room Impulse Response Estimation

- **评分**：8/10
- **作者/机构**：Akira Takahashi, Ryosuke Sawata, Shusuke Takahashi, Yuki Mitsufuji；暂无
- **论文链接**：http://arxiv.org/abs/2605.00431v1
- **PDF**：https://arxiv.org/pdf/2605.00431v1.pdf
- **代码链接**：暂无
- **Demo 链接**：http://www.bibsonomy.org/BibtexHandler?requTask=upload&amp;url=https://arxiv.org/abs/2605.00431&amp;description=MMAudioReverbs:

#### 📌 简介
2 Related Work 2.1 V2A Generation and Multimodal Foundations 2.2 Room Acoustics with Audio and Visual Cues 3 Method 3.1 Backbone and Conditioning Framework 3.2 Unified Flow Formul…

#### ☠️ 毒舌点评
全文看下来不像完全糊弄，但也没到一眼封神。值不值得跟，主要看你是不是正做这条子方向。

#### 🔧 技术方案
- **模型解决的问题**：2 Related Work 2.1 V2A Generation and Multimodal Foundations 2.2 Room Acoustics with Audio and Visual Cues 3 Method 3.1 Backbone and Condit…
- **模型架构**：
  输入/条件：输入/条件: Introduction 2 Related Work 2.1 V2A Generation and Multimodal Foundations 2.2 Room Acoustics with Audio and Visu…
  整体框架：整体框架: 从全文抽到的是任务级框架，不再只报空泛大类。
  关键模块：关键模块: Report, GitHub, Issue, Title, Content
- **训练 / 推理策略**：训练阶段: Report Issue Back to Abstract Download PDF <a class="header-button toggle-icon" href="javascript:toggle Experiments 4.1 Setup Pretrai…

#### 📊 实验结果
- 数据集：已读实验段，但命名抽取不稳。
- 主要结果：实验段已读取，但自动抽到的硬指标和对比项仍偏弱。
- baseline 对比：已读实验段，但基线名抽取不稳。
- 是否开源：暂未明确

### [4] Fast Text-to-Audio Generation with One-Step Sampling via Energy-Scoring and Auxiliary Contextual Representation Distillation

- **评分**：8/10
- **作者/机构**：Kuan-Po Huang, Bo-Ru Lu, Byeonggeun Kim, Mihee Lee, Zalan Fabian, Renard Korzeniowski, Qingming Tang, Greg Ver Steeg；暂无
- **论文链接**：http://arxiv.org/abs/2605.00329v1
- **PDF**：https://arxiv.org/pdf/2605.00329v1.pdf
- **代码链接**：暂无
- **Demo 链接**：https://huggingface.co/huggingface

#### 📌 简介
2 Related Work 2.1 Autoregressive models with sampling head 2.2 Few-step sampling 2.3 Generative Models with Energy-Distance Scoring 2.4 Representation Distillation 3 Method 3.1 B…

#### ☠️ 毒舌点评
全文看下来不像完全糊弄，但也没到一眼封神。值不值得跟，主要看你是不是正做这条子方向。

#### 🔧 技术方案
- **模型解决的问题**：2 Related Work 2.1 Autoregressive models with sampling head 2.2 Few-step sampling 2.3 Generative Models with Energy-Distance Scoring 2.4 Re…
- **模型架构**：
  输入/条件：整体框架: 从全文抽到的是任务级框架，不再只报空泛大类。
  整体框架：关键模块: Report, GitHub, Issue, Title, Content
  关键模块：s and Future Work References A Energy-distance Interpretation.
- **训练 / 推理策略**：训练细节没有空着，但自动抽取到的损失/增广/训练阶段仍不够稳定。

#### 📊 实验结果
- 数据集：Experimental, Setup, Datasets, Model
- 主要结果：数据集: Experimental, Setup, Datasets, Model, Configurations
- baseline 对比：Experimental, Setup, Datasets, Model
- 是否开源：暂未明确


## 🎼 音乐生成 / 音乐理解

### [5] GaMMA: Towards Joint Global-Temporal Music Understanding in Large Multimodal Models

- **评分**：9/10
- **作者/机构**：Zuyao You, Zhesong Yu, Mingyu Liu, Bilei Zhu, Yuan Wan, Zuxuan Wu；暂无
- **论文链接**：http://arxiv.org/abs/2605.00371v1
- **PDF**：https://arxiv.org/pdf/2605.00371v1.pdf
- **代码链接**：暂无
- **Demo 链接**：https://huggingface.co/huggingface

#### 📌 简介
In this paper, we propose GaMMA, a state-of-the-art (SoTA) large multimodal model (LMM) designed to achieve comprehensive musical content un... ⚠️ 仅基于 abstract 判断。

#### ☠️ 毒舌点评
更像资源/基准补齐，不一定炸裂，但如果数据真开源，实用价值通常高于花哨结构。仅基于 abstract，先别急着吹。

#### 🔧 技术方案
- **模型解决的问题**：In this paper, we propose GaMMA, a state-of-the-art (SoTA) large multimodal model (LMM) designed to achieve comprehensiv...
- **模型架构**：
  输入/条件：信息不足，不能严肃下结构结论。
  整体框架：自动抽取仍偏弱。
  关键模块：HTML 正文未形成可用抽取结果，当前只能暂时回退到 abstract，不把宣传句当结论。
- **训练 / 推理策略**：HTML 和 PDF 文本抽取都没形成可用训练段，当前不乱写。

#### 📊 实验结果
- 数据集：已读实验段，但命名抽取不稳。
- 主要结果：HTML 和 PDF 文本抽取都没形成可用实验段，这篇暂时不能给出合格精读。
- baseline 对比：已读实验段，但基线名抽取不稳。
- 是否开源：暂未明确


## 最后结论

如果只让我排今天最值得优先看的 3 篇，会是：

1. **MedMosaic**
s audio from GigaSpeech (Chen et al., 2021), and read speech from LibriSpeech.
2. **GaMMA**
HTML 正文未形成可用抽取结果，当前只能暂时回退到 abstract，不把宣传句当结论。
3. **MMAudio-LABEL**
References License: arXiv.org perpetual non-exclusive license arXiv:2605.00495v1 [cs.SD] 01 May 2026 MMAudio-LABEL: Aud…
