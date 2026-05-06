# 语音 / 音频 / 音乐论文速递
## 2026-05-06

> 实际对应 arXiv 更新日：**2026-05-05**  
> 检索范围：`cs.SD + eess.AS`  
> 只放按 ML 顶会审稿口径看，最值得多数读者花时间看的 **5 篇**

## 📋 总览

- 共收录 **5 篇** 相关论文
- 语音大模型：**1 篇**
- 语音/歌声生成：**1 篇**
- 音乐生成/理解：**2 篇**
- 其他音频方向：**1 篇**

今天真正值得看的主线有三条。第1条主线是 `DECKER`，重点在 2 Background and Related Works 2.1 Acoustic Emanation… 第2条主线是 `MiniMind-O Technical Report`，重点在 2 Related Work Omni and speech-text dialogue models. 第3条主线是 `PHALAR`，重点在 2 Related Works 2.1 Contrastive Representation Learni…

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
| 语音大模型 | 1 | DECKER: Domain-invariant Embedding for Cross-Keyboard Extraction and Recognition | 8/10 | References A Standardized Typing Corpus B…, Acoustic side-channel attacks (ASCA) on k…, 输入/条件: Introduction 2 Background and Rela… |
| 语音/歌声生成 | 2 | MiniMind-O Technical Report: An Open Small-Scale Speech-Native Omni Model | 7/10 | References A Module and Evaluation Detail…, It accepts text, speech, and image inputs…, 输入/条件: Multimodal feature alignment. |
| 音乐生成/理解 | 3 | PHALAR: Phasors for Learned Musical Audio Representations | 7/10 | Limitations and Failure Cases Future work…, 整体框架: 从全文抽到的是任务级框架，不再只报空泛大类。, 关键模块: Report, GitHub, Issue, Title, Conte… |
| 其他音频方向 | 4 | Deepfake Audio Detection Using Self-supervised Fusion Representations | 7/10 | References License: CC BY 4.0 arXiv:2605.…, To address this challenge, a dual-branch…, 输入/条件: To address this challenge, a dual-… |
| 音乐生成/理解 | 5 | APEX: Large-scale Multi-task Aesthetic-Informed Popularity Prediction for AI-Generated Music | 7/10 | Acknowledgments 8 AI Usage Statement Refe…, However, the explosive rise of AI-generat…, 输入/条件: Introduction 2 Related work 3 Prop… |

## 🤖 语音大模型 / 语音理解

### [1] DECKER: Domain-invariant Embedding for Cross-Keyboard Extraction and Recognition

- **评分**：8/10
- **作者/机构**：Bikrant Bikram Pratap Maurya, Nitin Choudhury, Daksh Agarwal, Arun Balaji Buduru；暂无
- **论文链接**：http://arxiv.org/abs/2605.03384v1
- **PDF**：https://arxiv.org/pdf/2605.03384v1.pdf
- **代码链接**：暂无
- **Demo 链接**：https://huggingface.co/huggingface

#### 📌 简介
2 Background and Related Works 2.1 Acoustic Emanations of Keystrokes 2.2 Multipath Propagation and Environmental Effects 2.3 Deep Learning for Acoustic Attacks 2.4 Language Models…

#### ☠️ 毒舌点评
不像纯标题党，至少方法和实验都在往完整论文靠。但是否真创新，还得盯住它是不是把老模块重新拼了一遍。

#### 🔧 技术方案
- **模型解决的问题**：2 Background and Related Works 2.1 Acoustic Emanations of Keystrokes 2.2 Multipath Propagation and Environmental Effects 2.3 Deep Learning…
- **模型架构**：
  输入/条件：输入/条件: Introduction 2 Background and Related Works 2.1 Acoustic Emanations of Keystrokes 2.2 Multipath Propagation and…
  整体框架：整体框架: 语音/音频大模型主干，倾向统一建模或多模态对齐，不是传统单模块前端。
  关键模块：关键模块: Report, GitHub, Issue, Title, Content
- **训练 / 推理策略**：训练细节没有空着，但自动抽取到的损失/增广/训练阶段仍不够稳定。

#### 📊 实验结果
- 数据集：已读实验段，但命名抽取不稳。
- 主要结果：DECKER: Domain-Invariant Modeling 6.4.1 KSN Ablation and Visualization Domain-classification accuracy.
- baseline 对比：Comparison
- 是否开源：暂未明确


## 🗣️ TTS / 歌声生成

### [2] MiniMind-O Technical Report: An Open Small-Scale Speech-Native Omni Model

- **评分**：7/10
- **作者/机构**：Jingyao Gong；暂无
- **论文链接**：http://arxiv.org/abs/2605.03937v1
- **PDF**：https://arxiv.org/pdf/2605.03937v1.pdf
- **代码链接**：**已开源** **代码已开源**: https://github.com/jingyaogong/minimind-o
- **Demo 链接**：https://huggingface.co/huggingface

#### 📌 简介
2 Related Work Omni and speech-text dialogue models. Discrete audio representation and speech generation.

#### ☠️ 毒舌点评
全文看下来不像完全糊弄，但也没到一眼封神。值不值得跟，主要看你是不是正做这条子方向。

#### 🔧 技术方案
- **模型解决的问题**：2 Related Work Omni and speech-text dialogue models.
- **模型架构**：
  输入/条件：输入/条件: Multimodal feature alignment.
  整体框架：整体框架: 生成式声学建模主干，通常是 codec / diffusion / AR-NAR 一类。
  关键模块：关键模块: Report, GitHub, Issue, Title, Content
- **训练 / 推理策略**：训练细节没有空着，但自动抽取到的损失/增广/训练阶段仍不够稳定。

#### 📊 实验结果
- 数据集：MiniMind-O, T2A, I2T, A2A
- 主要结果：数据集: MiniMind-O, T2A, I2T, A2A, Parquet
- baseline 对比：已读实验段，但基线名抽取不稳。
- 是否开源：是


## 🎼 音乐生成 / 音乐理解

### [3] PHALAR: Phasors for Learned Musical Audio Representations

- **评分**：7/10
- **作者/机构**：Davide Marincione, Michele Mancusi, Giorgio Strano, Luca Cerovaz, Donato Crisostomi, Roberto Ribuoli, Emanuele Rodolà；暂无
- **论文链接**：http://arxiv.org/abs/2605.03929v1
- **PDF**：https://arxiv.org/pdf/2605.03929v1.pdf
- **代码链接**：暂无
- **Demo 链接**：https://huggingface.co/huggingface

#### 📌 简介
2 Related Works 2.1 Contrastive Representation Learning in Audio 2.2 From Semantic Similarity to Structural Coherence 2.3 Complex-Valued Neural Networks (CVNNs) 3 Method 3.1 Harmo…

#### ☠️ 毒舌点评
不像纯标题党，至少方法和实验都在往完整论文靠。但是否真创新，还得盯住它是不是把老模块重新拼了一遍。

#### 🔧 技术方案
- **模型解决的问题**：2 Related Works 2.1 Contrastive Representation Learning in Audio 2.2 From Semantic Similarity to Structural Coherence 2.3 Complex-Valued Ne…
- **模型架构**：
  输入/条件：整体框架: 从全文抽到的是任务级框架，不再只报空泛大类。
  整体框架：关键模块: Report, GitHub, Issue, Title, Content
  关键模块：Limitations and Failure Cases Future work Broader impacts and potential misuse References A Complex-valued layers A.1 C…
- **训练 / 推理策略**：数据处理: Report Issue Back to Abstract Download PDF <a class="header-button toggle-icon" href="javascript:toggle Experiments 4.1 Experimental…

#### 📊 实验结果
- 数据集：Experiments, Experimental, Setup, Datasets
- 主要结果：数据集: Experiments, Experimental, Setup, Datasets, Sampling
- baseline 对比：Experiments, Experimental, Setup, Datasets
- 是否开源：暂未明确

### [4] APEX: Large-scale Multi-task Aesthetic-Informed Popularity Prediction for AI-Generated Music

- **评分**：7/10
- **作者/机构**：Jaavid Aktar Husain, Dorien Herremans；暂无
- **论文链接**：http://arxiv.org/abs/2605.03395v1
- **PDF**：https://arxiv.org/pdf/2605.03395v1.pdf
- **代码链接**：暂无
- **Demo 链接**：https://huggingface.co/huggingface

#### 📌 简介
2 Related work 3 Proposed APEX model 3.1 MERT Encoder 3.2 Multitask approach 3.2.1 Main task: Streams- and likes-score 3.2.2 Auxiliary tasks: Aesthetics scores 3.2.3 Combining los…

#### ☠️ 毒舌点评
不像纯标题党，至少方法和实验都在往完整论文靠。但是否真创新，还得盯住它是不是把老模块重新拼了一遍。

#### 🔧 技术方案
- **模型解决的问题**：2 Related work 3 Proposed APEX model 3.1 MERT Encoder 3.2 Multitask approach 3.2.1 Main task: Streams- and likes-score 3.2.2 Auxiliary task…
- **模型架构**：
  输入/条件：输入/条件: Introduction 2 Related work 3 Proposed APEX model 3.1 MERT Encoder 3.2 Multitask approach 3.2.1 Main task: Strea…
  整体框架：整体框架: 从全文抽到的是任务级框架，不再只报空泛大类。
  关键模块：关键模块: Report, GitHub, Issue, Title, Content
- **训练 / 推理策略**：训练细节没有空着，但自动抽取到的损失/增广/训练阶段仍不够稳定。

#### 📊 实验结果
- 数据集：Experimental, Dataset, Embedding, Training
- 主要结果：数据集: Experimental, Dataset, Embedding, Training, Input
- baseline 对比：已读实验段，但基线名抽取不稳。
- 是否开源：暂未明确


## 🔊 其他音频方向

### [5] Deepfake Audio Detection Using Self-supervised Fusion Representations

- **评分**：7/10
- **作者/机构**：Khalid Zaman, Qixuan Huang, Muhammad Uzair, Masashi Unoki；暂无
- **论文链接**：http://arxiv.org/abs/2605.03420v1
- **PDF**：https://arxiv.org/pdf/2605.03420v1.pdf
- **代码链接**：暂无
- **Demo 链接**：https://huggingface.co/huggingface

#### 📌 简介
II Dataset III Proposed Method III-A Data Augmentation III-B Model Architecture IV Results Discussion IV-A Experimental Setup IV-B Results and Discussion V Conclusion References L…

#### ☠️ 毒舌点评
不像纯标题党，至少方法和实验都在往完整论文靠。但是否真创新，还得盯住它是不是把老模块重新拼了一遍。

#### 🔧 技术方案
- **模型解决的问题**：II Dataset III Proposed Method III-A Data Augmentation III-B Model Architecture IV Results Discussion IV-A Experimental Setup IV-B Results…
- **模型架构**：
  输入/条件：输入/条件: To address this challenge, a dual-branch deepfake detection framework is proposed to jointly model speech and en…
  整体框架：整体框架: 从全文抽到的是任务级框架，不再只报空泛大类。
  关键模块：关键模块: Report, GitHub, Issue, Title, Content
- **训练 / 推理策略**：训练阶段: Two pretrained models, XLS-R for speech and BEATs for environmental sound, are used to extract complementary contextual representatio…

#### 📊 实验结果
- 数据集：Experimental, Setup, IV-B
- 主要结果：数据集: Experimental, Setup, IV-B, Results, Discussion
- baseline 对比：F1-score, EER
- 是否开源：暂未明确


## 最后结论

如果只让我排今天最值得优先看的 3 篇，会是：

1. **DECKER**
References A Standardized Typing Corpus B Metadata Schema C KSN Ablation and Visualization D License: CC BY 4.0 arXiv:2…
2. **MiniMind-O Technical Report**
References A Module and Evaluation Details B Qualitative Examples License: CC BY 4.0 arXiv:2605.03937v1 [cs.SD] 05 May…
3. **PHALAR**
Limitations and Failure Cases Future work Broader impacts and potential misuse References A Complex-valued layers A.1 C…
