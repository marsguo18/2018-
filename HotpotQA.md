# 2. HotpotQA 属于哪一类数据集
新型问答数据集：HotpotQA

现有的问答（QA）数据集无法训练可执行**复杂推理和提供答案解释**的QA系统。HotpotQA由此而生。
## Seq2Seq
## 目前主流的问答数据集：SQuAD
[SQuAD](https://rajpurkar.github.io/SQuAD-explorer/) 全称为：Stanford Question Answering Dataset (SQuAD)，斯坦福问答数据集。目前主流的问答数据集对**多信息进行多步推理**能力可能较为欠缺
## 多信息推理尝试
- Facebook发布的[bAbI数据集](https://research.fb.com/downloads/babi/)：数据通过人造模版生成而不是源于真实文本，实际场景性能低。
- [TriviaQA](#)：附带多个相关文件来获取答案。但文件的增多不能保证一定用到多信息推理
- [QAngaroo](http://qangaroo.cs.ucl.ac.uk)：利用知识图谱技术构建需要多步推理才能回答的问题。但问题和答案受限于知识图谱。
## 新型问答数据集：HotpotQA
1. 问题的答案必须要基于**多个支持文档**；
2. 问题**多样化**，不局限于任何已有的知识库或知识模式；
3. 提供句子级别的**支持推理线索**（supporting fact），允许 QA 系统用强大的监督进行推理，并对预测结果进行解释；
4. 提供了新型模拟比较型问题，来测试 QA 系统提取相关线索、执行必要对比的能力。


# Seq2Seq
## Seq2Seq技术要素
1. 用语言模型生成词向量
2. 用于语义编辑的LSTM模型
3. Attention机制
4. 深度学习借力知识图谱
5. 准确性评价函数BLEU
## 以中文句子翻译为英文句子为例
### 用语言模型生成词向量
把中文词先翻成一个词向量（一种数字语言）
### 用于语义编辑的LSTM模型
对这个词向量再编辑，变成一个语义表示的方式
### Attention机制
Attention机制决定词向量转到英语时，哪些词汇是最适当的
### 深度学习借力知识图谱
最初，Attention只能看出字面意思，没有先验的知识。把知识图谱融入Attention里，就可以有先验的知识。
### 准确性评价函数BLEU
对训练完的模型进行评价
## 用语言模型生成词向量密不可分的三个人
1. 徐伟：于1998年提出语言模型
2. Yoshua Bengio：奠定了怎么用语言模型和词向量的整个方法论
3. Tomas Mikolov：做出词向量

