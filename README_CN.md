# 从零构建推理模型

本仓库包含了开发LLM推理模型的代码，是书籍《[*从零构建推理模型*]》(https://mng.bz/lZ5B)的官方代码仓库。


<br>
<br>

<a href="https://mng.bz/lZ5B"><img src="https://sebastianraschka.com/images/reasoning-from-scratch-images/cover.webp?123" width="250px"></a>

（印刷版彩色印刷）

<br>

在《[*从零构建推理模型*]》(https://mng.bz/lZ5B)中，您将学习和理解推理型大型语言模型（LLM）的工作原理。

推理是近年来改进LLM最令人兴奋和重要的进展之一，但如果只听到"推理"这个术语并从理论上了解它，这也是最容易误解的。这就是为什么本书采用实践方法。我们将从预训练的基线LLM开始，然后自己在代码中逐步添加推理能力，这样您就能确切地看到它是如何工作的。

本书中描述的方法将引导您完成开发自己的小型但功能完备的推理模型的过程，以教育为目的。它反映了创建大规模推理模型（如DeepSeek R1、GPT-5 Thinking等）所使用的方法。此外，本书还包括加载现有预训练模型权重的代码。

- 官方[源代码仓库链接](https://github.com/rasbt/reasoning-from-scratch)
- [Manning出版社网站](https://mng.bz/lZ5B)上的书籍链接
- Amazon.com上的书籍页面（待定）
- ISBN 9781633434677



<br>
<br>

要下载本仓库的副本，请点击[下载ZIP](https://github.com/rasbt/reasoning-from-scratch/archive/refs/heads/main.zip)按钮或在终端中执行以下命令：

```bash
git clone --depth 1 https://github.com/rasbt/reasoning-from-scratch.git
```

<br>


> **提示：**
> 第2章提供了有关安装Python、管理Python包和设置编码环境的其他提示。

<br>
<br>

## 目录（进行中）

[![Linux代码测试](https://github.com/rasbt/reasoning-from-scratch/actions/workflows/tests-linux.yml/badge.svg)](https://github.com/rasbt/reasoning-from-scratch/actions/workflows/tests-linux.yml)
[![macOS代码测试](https://github.com/rasbt/reasoning-from-scratch/actions/workflows/tests-macos.yml/badge.svg)](https://github.com/rasbt/reasoning-from-scratch/actions/workflows/tests-macos.yml)
[![Windows代码测试](https://github.com/rasbt/reasoning-from-scratch/actions/workflows/tests-windows.yml/badge.svg)](https://github.com/rasbt/reasoning-from-scratch/actions/workflows/tests-windows.yml)

| 章节标题                                                     | 主要代码                                                     |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| 第1章：理解推理模型                                         | 无代码                                                       |
| 第2章：使用预训练LLM生成文本                                 | - [ch02_main.ipynb](ch02/01_main-chapter-code/ch02_main.ipynb)<br/>- [ch02_exercise-solutions.ipynb](ch02/01_main-chapter-code/ch02_exercise-solutions.ipynb) |
| 第3章：评估推理模型                                         | - [ch03_main.ipynb](ch03/01_main-chapter-code/ch03_main.ipynb)<br/>- [ch03_exercise-solutions.ipynb](ch03/01_main-chapter-code/ch03_exercise-solutions.ipynb) |
| 第4章：通过推理时间缩放改进推理                             | - [ch04_main.ipynb](ch04/01_main-chapter-code/ch04_main.ipynb)<br/>- [ch04_exercise-solutions.ipynb](ch04/01_main-chapter-code/ch04_exercise-solutions.ipynb) |
| 第5章：通过自改进进行推理时间缩放                           | - [ch05_main.ipynb](ch05/01_main-chapter-code/ch05_main.ipynb)<br/>- [ch05_exercise-solutions.ipynb](ch05/01_main-chapter-code/ch05_exercise-solutions.ipynb) |
| 第6章：使用强化学习训练推理模型                             | 待定                                                         |
| 第7章：改进强化学习中的策略优化                             | 待定                                                         |
| 第8章：蒸馏推理模型以实现高效推理                           | 待定                                                         |
| 附录A：参考文献和进一步阅读                                 | 无代码                                                       |
| 附录B：练习解答                                             | 代码和解答在每个章节的子文件夹中                             |
| 附录C：Qwen3 LLM源代码                                       | - [chC_main.ipynb](chC/01_main-chapter-code/chC_main.ipynb)  |
| 附录D                                                       | 待定                                                         |
| 附录E                                                       | 待定                                                         |
| 附录F：LLM评估的常见方法                                     | - [chF_main.ipynb](chF/01_main-chapter-code/chF_main.ipynb)  |

<br>
&nbsp;

以下心智模型总结了本书涵盖的主要技术。

<img src="https://sebastianraschka.com/images/reasoning-from-scratch-images/mental-model.webp" width="650px">



<br>



&nbsp;
## 配套书籍

请注意，《*从零构建推理模型*》是一本专注于改进LLM推理方法的独立书籍。

本书中，我们在一个预训练的开源基线LLM（Qwen3）上工作，在此基础上从头编码应用推理方法。这包括推理时间缩放、强化学习和蒸馏。

然而，如果您对理解传统基线LLM的实现方式感兴趣，您可能会喜欢我的上一本书，《[*从零构建大型语言模型*]》(https://amzn.to/4fqvn0D)。

<a href="https://amzn.to/4fqvn0D"><img src="https://sebastianraschka.com/images/LLMs-from-scratch-images/cover.jpg?123" width="120px"></a>

- [Amazon链接](https://amzn.to/4fqvn0D)
- [Manning链接](http://mng.bz/orYv)
- [GitHub仓库](https://github.com/rasbt/LLMs-from-scratch)


&nbsp;
## 硬件要求

本书主要章节中的代码设计为在消费级硬件上在合理的时间内运行，不需要专用服务器硬件。这种方法确保了广泛的受众可以参与其中。此外，代码在可用时自动利用GPU。也就是说，第2-4章在CPU和GPU上都能很好地运行。对于第5章和第6章，如果您想复制章节中的结果，建议使用GPU。

（请参阅[setup_tips](ch02/https://github.com/rasbt/reasoning-from-scratch/blob/main/ch02/01_main-chapter-code/python-instructions.md)文档以获取其他建议。）

&nbsp;
## 练习

本书的每一章都包含几个练习。解答在附录B中总结，相应的代码笔记本在本仓库的主要章节文件夹中可用（例如， [`ch02/01_main-chapter-code/ch02_exercise-solutions.ipynb`](ch02/01_main-chapter-code/ch02_exercise-solutions.ipynb)）。


&nbsp;
## 额外材料

几个文件夹包含作为对感兴趣读者的额外奖励的可选材料：

- **第2章：使用预训练LLM生成文本**
  - [可选的Python设置和云GPU推荐](ch02/02_setup-tips)
  - [使用LLM的GPU优化版本](ch02/03_optimized-LLM)
  - [在Windows上使用`torch.compile()`](ch02/04_torch-compile-windows)
  - [运行推理并与模型对话](ch02/05_use_model)
- **第3章：评估LLM**
  - [MATH-500验证器脚本](ch03/02_math500-verifier-scripts)

- **第4章：通过推理时间缩放改进推理**
  - [MATH-500推理缩放脚本](ch04/02_math500-inference-scaling-scripts)

- **附录F：LLM评估的常见方法**
  - [MMLU评估方法](chF/02_mmlu)
  - [LLM排行榜](chF/03_leaderboards)
  - [LLM作为裁判](chF/04_llm-judge)


&nbsp;
## 问题、反馈和为本仓库做贡献

我欢迎各种反馈，最好通过[Manning讨论论坛](https://livebook.manning.com/forum?product=raschka2&page=1)或[GitHub讨论](https://github.com/rasbt/reasoning-from-scratch/discussions)分享。同样，如果您有任何问题或只是想交流想法，请随时在论坛中发布。

请注意，由于本仓库包含对应印刷书籍的代码，我目前无法接受会扩展主要章节内容的贡献，因为这会引入与实体书的偏差。保持一致有助于确保每个人的顺畅体验。

&nbsp;
## 引用

如果您发现本书或代码对您的研究有用，请考虑引用它。

芝加哥格式引用：

> Raschka, Sebastian. *从零构建推理模型*. Manning, 2025. ISBN: 9781633434677.

BibTeX条目：

```
@book{build-llms-from-scratch-book,
  author       = {Sebastian Raschka},
  title        = {Build A Reasoning Model (From Scratch)},
  publisher    = {Manning},
  year         = {2025},
  isbn         = {9781633434677},
  url          = {https://mng.bz/lZ5B},
  github       = {https://github.com/rasbt/reasoning-from-scratch}
}
```
