# daily-llm

[写在开始之前的话](./PREFACE.md)

## CH.0 - 从兴趣出发而不是为了工作

> 我强烈建议每天都来翻看这一章节中的内容，它是我不断在全网搜集的科普向内容（图文、视频、讲座等），你可以利用一切碎片化的事件来根据你的兴趣或者干脆随机观看。
>
> CH.0中的内容大多都没有关联。我希望在这个章节中你可以先积累大模型相关的背景、历史及趣味常识，希望你能够Get到我想尽一切办法减低你的学习焦虑的初心🫡。


1. [图灵讲座：生成式人工智能的未来](https://youtu.be/2kSl0xkq2lM)

   迈克尔·伍尔德里奇教授关于生成式AI未来可能性及对社会影响的讨论，这是“AI如何打破互联网”图灵讲座系列的一部分。

2. [生成式人工智能简而言之——如何在人工智能时代生存和发展](https://youtu.be/2IK3DFHRFfw)


## CH.1 - 基础不牢地动山摇

> 当你在CH.0观看了10个以上的视频之后，我相信你已经对生成式大语言模型有了一个快速侧写的认知。
>
> 接下来我希望你用几天的时间，通篇阅读一下CH.1中的内容。它们是大模型领域的经典论文，涉及了多个方面，包括模型架构、训练方法、优化算法等。这些论文为大模型的发展奠定了基础或引领了重要的技术方向。
>
> 当然，阅读论文的过程确实是枯燥乏味且令人抓狂。我也并不对你做出学术界的要求，但是起码要通读一遍。相信我，这会在后面的实践中发挥出巨大的作用。


1. ["Attention is All You Need" by Vaswani et al. (2017)](https://arxiv.org/abs/1706.03762)

   介绍了Transformer模型，它是现代大型语言模型如GPT系列和BERT系列的基础。Transformer架构通过自注意力（self-attention）机制有效地处理序列数据，改变了自然语言处理（NLP）领域的研究和应用。

2. ["BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding" by Devlin et al. (2018)](https://arxiv.org/abs/1810.04805)
   
   提出了BERT模型，它采用双向Transformer预训练方法，显著提高了多项NLP任务的性能。BERT的出现标志着预训练+微调的方法成为NLP领域的标准范式。

3. ["Improving language understanding with unsupervised learning"](https://openai.com/research/language-unsupervised)
   
   讨论了使用transformers和无监督预训练相结合的方法，以及这种方法在多样化语言任务中取得了最先进的结果。它强调了这种可扩展、任务不可知的系统的有效性，并提到系统也将被公开。这种结合使用有监督学习方法和无监督预训练的方法非常有效，

4. "Language Models are Unsupervised Multitask Learners" by Radford et al. (OpenAI, 2019)
    
    继GPT之后介绍了GPT-2模型，它通过更大的模型和更多的数据，展示了语言模型在没有明确任务指导的情况下，仍然可以生成高质量文本和在多种NLP任务上表现出色。

5. "Scaling Laws for Neural Language Models" by Kaplan et al. (OpenAI, 2020)
   
   通过实验研究了模型规模、数据集大小和计算预算如何共同影响语言模型性能的规律，为设计和训练大型模型提供了理论指导。

6. "Improving Language Understanding by Generative Pre-Training" by Radford et al. (OpenAI, pre-GPT-3)

    GPT-1的论文标志着生成式预训练语言模型的开始。通过在大规模数据集上预训练，然后在具体任务上进行微调，显著提升了多项自然语言理解任务的性能。

7. "GPT-3: Language Models are Few-Shot Learners" by Brown et al. (OpenAI, 2020)

    展示了通过大规模扩展模型规模，语言模型可以进行少样本学习，即在几乎没有任务特定数据的情况下通过任务描述来完成任务。这标志着语言模型向更加通用的人工智能方向迈进了一步。

8. "T5: Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer" by Raffel et al. (2019)

    提出了T5模型，强调将所有文本处理任务统一为文本到文本的格式，探索了迁移学习的极限。这种方法简化了不同NLP任务之间的转换，使得模型能够更容易地在多个任务上共享知识。

9.  "ALBERT: A Lite BERT for Self-supervised Learning of Language Representations" by Lan et al. (2019)

    提出了ALBERT模型，通过参数共享和降低模型大小的策略，提高了模型训练的效率和性能。ALBERT对于理解如何在保持模型性能的同时减少资源消耗提供了重要的见解。

10. "XLNet: Generalized Autoregressive Pretraining for Language Understanding" by Yang et al. (2019)

    提出了XLNet，通过结合自回归语言模型和BERT的优点，改进了模型对上下文的理解能力。XLNet在多项NLP任务上设置了新的性能基准，展示了预训练语言模型的进一步演进。


---
## CH.2 - 窥一斑而知全豹

> 这一章节中的内容速通，视频可以倍速、文章可以速览。力求在最短的时间内将全部概念和术语知晓，这些内容最好在你的笔记中记录每一个新鲜事物出现的时间点，未来当你需要深入研究的时候可以直接Jump进来再重新精读。

1. [50 Days to AI/ML: from Zero to Hero (for non-CS background)](https://medium.com/@sibtainwahab/50-days-to-ai-ml-from-zero-to-hero-for-non-cs-background-6f256a7d03b7)
   
    提供了一个50天自学机器学习和深度学习的路线图，旨在帮助对这一领域感兴趣但没有技术背景的人迅速入门。路线图从基础的数学知识开始，然后逐步深入到Python编程、使用Numpy、Pandas、Matplotlib等库，再到深入学习机器学习和深度学习的核心概念，最后通过实践项目来巩固所学知识。文章强调了学习过程中对问题解决能力、学习意愿和获得相关证书的重要性，并指出不需要技术背景或计算机科学/人工智能学位就可以开始学习机器学习。整个路线图是作者根据个人经验整理的，目的是让读者能够在短时间内有效学习并进入机器学习和深度学习的领域。

---
## CH.99 - 方向不对努力白费

> 我推荐的全网可关注的Up主，排名不分先后。但是当你看到某个Up带有🔭标记，那么建议你将他/她的所有视频全部看完。

### 知乎

### YouTube

### BiliBili

### Medium

---

## CH.99 - 工欲善其事，必先利其器


---

## CH.100 - 按图索骥

> 这是搜集到的具有局部宏观的图片。每张图片会注明出处。

![alt generative-AI-in-a-nutshell](picture/generative-AI-in-a-nutshell.png "generative-AI-in-a-nutshell")

<p align="center"><a href="https://www.youtube.com/watch?v=2IK3DFHRFfw">图片出处</a></p>

---


### CONTRIBUTING
如果有更好的资源或课程，欢迎提交Issues。
如有内容侵权请联系我（ODUzMzU5NkBnbWFpbC5jb20=）。
