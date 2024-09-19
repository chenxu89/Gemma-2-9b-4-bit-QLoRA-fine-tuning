# 项目简介

## 概述
本项目使用QLoRA技术（即结合了量化 和 LoRA 技术），旨在在资源有限的情况下对预训练大模型进行高效微调，如移动设备或嵌入式设备，并将微调后的模型用在了一个文本分类任务的推理上。包含了完整的训练和推理过程。

## 时间
2024.09.18-2024.09.19

## 主要工作和收获
- 使用 QLoRA 技术在资源有限的情况下对大规模预训练模型进行高效微调
- 使用了多GPU并行推理技术
- 使用了交差验证
- 使用了TTA（测试时增强）技术，提升模型在测试阶段的泛化能力，进一步提高推理结果的鲁棒性
- 做了一个文本分类任务的推理

## 技术栈
Gemma 2，QLoRA微调，混合精度训练，TTA（测试时增强），多GPU并行推理，交叉验证

##  数据集
[lmsys-chatbot-arena](https://www.kaggle.com/competitions/lmsys-chatbot-arena)

## 结果

> 我没有参加下面这个比赛，只是学习目的，下面是原作者的参赛结果，供参考

比赛地址：[LMSYS - Chatbot Arena Human Preference Predictions](https://www.kaggle.com/competitions/lmsys-chatbot-arena)

比赛简介和推理任务：
我们使用了从 Chatbot Arena 收集的大型数据集，用户在该平台与两个匿名 LLM 进行对话，并选择他们更喜欢的回答。在这次竞赛中，你的任务是预测用户在这些对决中更倾向于哪个回应。

原作者提交后的结果如下：效果非常好，击败了之前所有人的提交结果（0.98-1）

| 子集 | 对数损失 |
| - | - |
| 评估集 | 0.9371 |
| LB | 0.941 |

## kaggle地址
[[Training] Gemma-2 9b 4-bit QLoRA fine-tuning](https://www.kaggle.com/code/chenxucool/training-gemma-2-9b-4-bit-qlora-fine-tuning)

[[Inference] Gemma-2 9b 4-bit QLoRA](https://www.kaggle.com/code/chenxucool/inference-gemma-2-9b-4-bit-qlora)

## csdn地址
[【AI小项目6】QLoRA针对资源受限设备上的大模型微调和文本分类任务的推理](https://blog.csdn.net/weixin_43221845/article/details/142313255?sharetype=blogdetail&sharerId=142313255&sharerefer=PC&sharesource=weixin_43221845&spm=1011.2480.3001.8118)

## 参考
[[Training] Gemma-2 9b 4-bit QLoRA fine-tuning](https://www.kaggle.com/code/emiz6413/training-gemma-2-9b-4-bit-qlora-fine-tuning)
[[Inference] Gemma-2 9b 4-bit QLoRA](https://www.kaggle.com/code/emiz6413/inference-gemma-2-9b-4-bit-qlora/notebook)
