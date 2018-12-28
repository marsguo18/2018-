# AutoML
## Why AutoML?
- 算法调参支配的恐怖（求相对最优的参数）
- 调试不同格式的模型和服务端的关联

## What is AutoML?
自动机器学习（AutoML）是将机器学习应用于实际问题的端到端流程自动化的过程。

## When?
在2018年谷歌云全球NEXT大会（Google CloudNext 18）上，李飞飞宣布，谷歌AutoML Vision进入公共测试版，并推出了两款新的AutoML产品：AutoML Natural Language和AutoML Translation。

## 其他机器学习自动化
### [CustomVision.AI](https://www.customvision.ai)
- 2017年底，微软发布CustomVision.AI，涵盖图像、视频、文本和语音等各个领域。今年 1 月，他们又推出了完全自动化的平台 Microsoft Custom Vision Services（微软定制视觉服务）。[1]
### [OneClick.AI](https://www.oneclick.ai/zh-hans/)
- OneClick.AI 在2017 年年底正式上线，支持深度学习和传统机器学习算法，能处理结构化数据，以及混合了文字、图像、时间序列的非结构化内容。[2]
- OneClick.ai 基于通用的模型结构设计算法（Generalized Architecture Search，GAS），用于处理更复杂数据的分类和回归分析。GAS 支持自动特征工程和数据预处理，可与人类算法工程师一样，进行原始数据的观测，利用有监督学习从数据中积累相关领域的知识，提高了计算效率。

## AutoML的创造者
[Quoc Le](https://ai.google/research/people/QuocLe)
- 2011 年在斯坦福大学读博时，Le 和老师吴恩达以及谷歌大脑的研究人员一起，基于千万张 YouTube 图像开发了一个识别猫的无监督学习系统；
- 2014 年，Le 将深度学习技术应用在自然语言理解任务上，提出了能将文本转换为向量表征、基于循环神经网络的 Seq2Seq 学习模型，将机器翻译的前沿水平又向前推进了一步。
- 自 2014 年以来，Le 将目光转向了自动化机器学习（AutoML）。他认为可以把构建机器学习模型的过程需要反复的人工调整并达到最优想成是一个试错问题，继而通过机器学习解决。
- 2016 年，Le 与一位谷歌研究者合作发表了一篇开创性的论文《Neural Architecture Search with Reinforcement Learning》。其指出：让机器从一个定义空间中选取自己所需的组件来构建神经网络，然后使用一种试错技术，也就是强化学习来提升其准确度。


参考文献：
[1] [告别调参，AutoML新书发布](https://www.jiqizhixin.com/articles/2018-10-17-14?from=synced&keyword=AutoML). 机器之心, 2018.10.17<br>
[2] [让机器自己学习人工智能，「OneClick.ai」正打造自动化的深度学习人工智能平台](https://www.toutiao.com/a6561542535754285575/). 36氢, 2018.5.31