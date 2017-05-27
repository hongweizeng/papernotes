[A Neural Conversational Model](https://arxiv.org/pdf/1506.05869.pdf)

## Introduction

#### **_第一段：_**
1. end-to-end的进步在很多领域都取得了remarkable的发展。
2. 最近的一些工作都表明，神经网络不仅能做分类问题，还能将**复杂的结构**映射到其他复杂的结构。
3. 一个例子就是（Sutskever et al., 2014),在NLU方向的应用。
4. 改框架的主要好处就是几乎不需要特征工程就能达到或者超过state-of-the-art的结果。
5. 这个优点，允许研究者在领域知识不够（not be readily avilable）的task，或者规则太难设计的task上工作。

_myPost_：这里是总结Neural Network的背景和优点

#### **_第二段：_**
1. 会话模型能直接受益于this formulation，因为它需要mapping between queries and response。
2. this mapping很复杂，会话模型之前都被设计在非常狭窄的领域，主要工作就是特征工程。
3. In this work，我们把它看成给定上一个句子（们），预测下一个句子的任务的task。（Sutskever et al., 2014）.
4. We find that 这个方法在生成对话句子的流畅性和准确性上效果出奇的好（this approach can do surprisingly well on generating fluent and accurate replies to conversations.）

#### **_第三段：_**
1. 我们在IT helpdesk的对话数据集上测试了我们的模型，and find that 这个模型能**sometimes** 为用户解决问题并提供有用的答案。
2. 我们同样在一个来自有噪音的电影字幕的对话上做了实验， and find that 这个模型能够处理自然的对话 and **sometimes** 执行简单形式的常识推理。
3. In both cases，rnn相比于n-gram取得了更好的**perplexity**，并且捕捉了重要的长距离的关系。
4.从定性的角度看，我们的模型**sometimes**能够产生自然的对话。

_myPost_：
1. 常识推理什么的，都是瞎掰，或许碰巧数据集上存在而已，不过写作方式大胆，可以学习。
2. 长距离关系，rnn相比于n-gram是肯定有优势的，在作者本身的模型中如何体现的或许也没有，但是这个肯定的事情。（有点像废话？总不能算作者的工作，贡献吧、）

