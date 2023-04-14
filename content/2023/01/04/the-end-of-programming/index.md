---
title: "编程的终结"
date: 2023-01-04T07:09:47+08:00
updated: 2023-01-04T07:09:47+08:00
taxonomies:
  tags: []
extra:
  source: https://cacm.acm.org/magazines/2023/1/267976-the-end-of-programming/fulltext
  hostname: cacm.acm.org
  author: Matt Welsh
  original_title: "The End of Programming"
  original_lang: en
---

___

By Matt Welsh  
Communications of the ACM, January 2023, Vol. 66 No. 1, Pages 34-35  
10.1145/3570220  
[Comments (8)](https://cacm.acm.org/magazines/2023/1/267976-the-end-of-programming/fulltext#comments)

通过马特威尔士 ACM 通讯，2023 年 1 月，第 1 卷。 66 第 1 期，第 34-35 页 10.1145/3570220 评论 (8)

![/end text, hands typing on a keyboard, illustration](121922_CACMpg34_The-End-of2.large.jpg "/end text, hands typing on a keyboard, illustration")

Credit: Ursa Major 图片来源：大熊座

<iframe title="vimeo-player" src="https://player.vimeo.com/video/775827887?h=9319126ed2" width="360" height="255" frameborder="0" allowfullscreen="" data-immersive-translate-mark="1"></iframe>

I came of age in the 1980s, programming personal computers such as the Commodore VIC-20 and Apple \]\[e at home. Going on to study computer science (CS) in college and ultimately getting a Ph.D. at Berkeley, the bulk of my professional training was rooted in what I will call "classical" CS: programming, algorithms, data structures, systems, programming languages. In Classical Computer Science, the ultimate goal is to reduce an idea to a program written by a human—source code in a language like Java or C++ or Python. Every idea in Classical CS—no matter how complex or sophisticated, from a database join algorithm to the mind-bogglingly obtuse Paxos consensus protocol—can be expressed as a human-readable, human-comprehendible program.

我在 1980 年代成年，在家里为 Commodore VIC-20 和 Apple \]\[e 等个人电脑编程。继续在大学学习计算机科学 (CS) 并最终获得博士学位。在伯克利，我的大部分专业培训都植根于我称之为“经典”CS 的领域：编程、算法、数据结构、系统、编程语言。在经典计算机科学中，最终目标是将一个想法简化为由人类编写的程序——使用 Java、C++ 或 Python 等语言编写的源代码。经典 CS 中的每一个想法——无论多么复杂或复杂，从数据库连接算法到令人难以置信的迟钝的 Paxos 共识协议——都可以表达为人类可读、人类可理解的程序。

When I was in college in the early 1990s, we were still in the depths of the AI Winter, and AI as a field was likewise dominated by classical algorithms. My first research job at Cornell University was working with Dan Huttenlocher, a leader in the field of computer vision (and now Dean of the MIT Schwarzman College of Computing). In Huttenlocher's Ph.D.-level computer vision course in 1995 or so, we never once discussed anything resembling deep learning or neural networks—it was all classical algorithms like Canny edge detection, optical flow, and Hausdorff distances. Deep learning was in its infancy, not yet considered mainstream AI, let alone mainstream CS.

20 世纪 90 年代初我上大学的时候，我们还处于 AI 寒冬的深处，AI 作为一个领域同样被经典算法所统治。我在康奈尔大学的第一份研究工作是与计算机视觉领域的领导者 Dan Huttenlocher（现任麻省理工学院苏世民计算学院院长）一起工作。在 Huttenlocher 1995 年左右的博士级计算机视觉课程中，我们从未讨论过任何类似于深度学习或神经网络的东西——它都是经典算法，如 Canny 边缘检测、光流和 Hausdorff 距离。深度学习处于起步阶段，尚未被视为主流 AI，更不用说主流 CS 了。

Of course, this was 30 years ago, and a lot has changed since then, but one thing that has not really changed is that CS is taught as a discipline with data structures, algorithms, and programming at its core. I am going to be amazed if in 30 years, or even 10 years, we are still approaching CS in this way. Indeed, I think CS as a field is in for a pretty major upheaval few of us are really prepared for.

当然，这是 30 年前的事了，从那以后发生了很多变化，但有一点没有真正改变，那就是 CS 是作为一门以数据结构、算法和编程为核心的学科来教授的。如果 30 年甚至 10 年后，我们仍然以这种方式接近 CS，我会感到惊讶。事实上，我认为 CS 作为一个领域正在经历一场相当大的剧变，但我们中很少有人真正做好准备。

**Programming will be obsolete.** I believe the conventional idea of "writing a program" is headed for extinction, and indeed, for all but very specialized applications, most software, as we know it, will be replaced by AI systems that are _trained_ rather than _programmed._ In situations where one needs a "simple" program (after all, not everything should require a model of hundreds of billions of parameters running on a cluster of GPUs), those programs will, themselves, be generated by an AI rather than coded by hand.

编程将过时。我相信“编写程序”的传统想法即将消失，事实上，除了非常专业的应用程序之外，大多数软件，正如我们所知，将被经过训练而不是编程的 AI 系统所取代。在需要“简单”程序的情况下（毕竟，并非所有事情都需要在 GPU 集群上运行数千亿个参数的模型），这些程序本身将由 AI 生成，而不是手动编码.

I do not think this idea is crazy. No doubt the earliest pioneers of computer science, emerging from the (relatively) primitive cave of electrical engineering, stridently believed that all future computer scientists would need to command a deep understanding of semiconductors, binary arithmetic, and microprocessor design to understand software. Fast-forward to today, and I am willing to bet good money that 99% of people who are writing software have almost no clue how a CPU actually works, let alone the physics underlying transistor design. By extension, I believe the computer scientists of the future will be so far removed from the classic definitions of "software" that they would be hard-pressed to reverse a linked list or implement Quicksort. (I am not sure I remember how to implement Quicksort myself.)

我不认为这个想法很疯狂。毫无疑问，计算机科学的最早先驱，从（相对）原始的电气工程洞穴中脱颖而出，坚定地认为所有未来的计算机科学家都需要对半导体、二进制算法和微处理器设计有深刻的理解，才能理解软件。快进到今天，我敢打赌 99% 的软件编写人员几乎不知道 CPU 的实际工作原理，更不用说晶体管设计背后的物理原理了。推而广之，我相信未来的计算机科学家将与“软件”的经典定义相去甚远，以至于他们很难反转链表或实现快速排序。 （我不确定自己是否记得如何实现 Quicksort。）

AI coding assistants such as CoPilot are only scratching the surface of what I am describing. It seems totally obvious to me that _of course_ all programs in the future will ultimately be written by AIs, with humans relegated to, at best, a supervisory role. Anyone who doubts this prediction need only look at the very rapid progress being made in other aspects of AI content generation, such as image generation. The difference in quality and complexity between DALL-E v1 and DALL-E v2—announced only 15 months later—is staggering. If I have learned anything over the last few years working in AI, it is that it is _very_ easy to underestimate the power of increasingly large AI models. Things that seemed like science fiction only a few months ago are rapidly becoming reality.

CoPilot 等 AI 编码助手只是触及了我所描述内容的表面。在我看来，显然未来所有程序最终都将由 AI 编写，而人类充其量只能充当监督角色。任何怀疑这一预测的人只需要看看人工智能内容生成的其他方面正在取得的非常迅速的进展，例如图像生成。 DALL-E v1 和 DALL-E v2（仅在 15 个月后发布）在质量和复杂性方面的差异是惊人的。如果我在过去几年从事 AI 工作中学到了什么，那就是很容易低估越来越大的 AI 模型的力量。几个月前还只是科幻小说的事物正在迅速成为现实。

So I am not just talking about things like Github's CoPilot replacing programmers.<sup><a href="https://cacm.acm.org/magazines/2023/1/267976-the-end-of-programming/fulltext#R1">1</a></sup> I am talking about _replacing the entire concept of writing programs with training models._ In the future, CS students are not going to need to learn such mundane skills as how to add a node to a binary tree or code in C++. That kind of education will be antiquated, like teaching engineering students how to use a slide rule.

所以我不只是在谈论像 Github 的 CoPilot 取代程序员这样的事情。1 我在谈论用训练模型取代编写程序的整个概念。将来，CS 学生将不需要学习如何向二叉树添加节点或使用 C++ 编写代码等世俗技能。那种教育将会过时，就像教工科学生如何使用计算尺一样。

The engineers of the future will, in a few keystrokes, fire up an instance of a four-quintillion-parameter model that already encodes the full extent of human knowledge (and then some), ready to be given any task required of the machine. The bulk of the intellectual work of getting the machine to do what one wants will be about coming up with the right examples, the right training data, and the right ways to evaluate the training process. Suitably powerful models capable of generalizing via few-shot learning will require only a few good examples of the task to be performed. Massive, human-curated datasets will no longer be necessary in most cases, and most people "training" an AI model will not be running gradient descent loops in PyTorch, or anything like it. They will be teaching by example, and the machine will do the rest.

未来的工程师只需敲几下键盘，就可以启动一个四五千万亿参数模型的实例，该模型已经编码了人类知识的全部范围（然后是一些），准备好接受机器所需的任何任务。让机器做我们想做的事的大部分智力工作将是提出正确的例子、正确的训练数据和评估训练过程的正确方法。能够通过少样本学习进行概括的适当强大的模型将只需要执行任务的几个好例子。在大多数情况下，将不再需要大量人工管理的数据集，而且大多数“训练”AI 模型的人不会在 PyTorch 或类似的东西中运行梯度下降循环。他们将以身作则，机器将完成剩下的工作。

In this new computer science—if we even call it computer science at all—the machines will be so powerful and already know how to do so many things that the field will look like less of an engineering endeavor and more of an an educational one; that is, _how to best educate the machine_, not unlike the science of how to best educate children in school. Unlike (human) children, though, these AI systems will be flying our airplanes, running our power grids, and possibly even governing entire countries. I would argue that the vast majority of Classical CS becomes irrelevant when our focus turns to teaching intelligent machines rather than directly programming them. Programming, in the conventional sense, will in fact be dead.

在这门新的计算机科学中——如果我们称它为计算机科学的话——机器将非常强大，并且已经知道如何做很多事情，以至于这个领域看起来更像是一个教育领域，而不是一个工程领域；也就是说，如何最好地教育机器，与如何最好地教育学校儿童的科学不同。然而，与（人类）儿童不同的是，这些人工智能系统将驾驶我们的飞机，运行我们的电网，甚至可能管理整个国家。我认为，当我们的重点转向教授智能机器而不是直接对它们进行编程时，绝大多数经典 CS 变得无关紧要。传统意义上的编程实际上已经死了。

___

> _I think CS as a field is in for a pretty major upheaval few of us are really prepared for._
> 
> 我认为 CS 作为一个领域正在经历一场相当大的剧变，我们中很少有人真正做好准备。

___

**How does all of this change how we think about the field of computer science?** The new atomic unit of computation becomes not a processor, memory, and I/O system implementing a von Neumann machine, but rather a massive, pre-trained, highly adaptive AI model. This is a seismic shift in the way we think about computation—not as a predictable, static process, governed by instruction sets, type systems, and notions of decidability. AI-based computation has long since crossed the Rubicon of being amenable to static analysis and formal proof. We are rapidly moving toward a world where the fundamental building blocks of computation are temperamental, mysterious, adaptive agents.

所有这些如何改变我们对计算机科学领域的看法？新的原子计算单元不再是实现冯诺依曼机器的处理器、内存和 I/O 系统，而是一个大规模的、预训练的、高度自适应的人工智能模型。这是我们对计算的思考方式的巨大转变——不再是一个可预测的静态过程，由指令集、类型系统和可判定性概念控制。基于 AI 的计算早已跨越了适用于静态分析和形式证明的 Rubicon。我们正在迅速走向一个计算的基本构建块是喜怒无常、神秘的自适应代理的世界。

This shift is underscored by the fact that _nobody actually understands how large AI models work._ People are publishing research papers<sup><a href="https://cacm.acm.org/magazines/2023/1/267976-the-end-of-programming/fulltext#R3">3</a>,<a href="https://cacm.acm.org/magazines/2023/1/267976-the-end-of-programming/fulltext#R4">4</a>,<a href="https://cacm.acm.org/magazines/2023/1/267976-the-end-of-programming/fulltext#R5">5</a></sup> actually _discovering new behaviors_ of existing large models, even though these systems have been "engineered" by humans. Large AI models are capable of doing things that they have not been explicitly trained to do, which should scare the living daylights out of Nick Bostrom<sup><a href="https://cacm.acm.org/magazines/2023/1/267976-the-end-of-programming/fulltext#R2">2</a></sup> and anyone else worried (rightfully) about an superintelligent AI running amok. We currently have no way, apart from empirical study, to determine the limits of current AI systems. As for future AI models that are orders of magnitude larger and more complex—good luck!

没有人真正了解大型 AI 模型的工作原理这一事实突显了这种转变。人们正在发表研究论文3、4、5，实际上是在发现现有大型模型的新行为，即使这些系统是由人类“设计”的。大型 AI 模型能够做它们没有经过明确训练可以做的事情，这应该会吓跑 Nick Bostrom2 和其他任何担心超级智能 AI 横行的人（理所当然地）。目前，除了实证研究外，我们没有办法确定当前人工智能系统的局限性。至于未来更大、更复杂的人工智能模型——祝你好运！

The shift in focus from programs to models should be obvious to anyone who has read any modern machine learning papers. These papers barely mention the code or systems underlying their innovations; the building blocks of AI systems are much higher-level abstractions like attention layers, tokenizers, and datasets. A time traveler from even 20 years ago would have a hard time making sense of the _three sentences_ in the (75-page!) GPT-3 paper<sup><a href="https://cacm.acm.org/magazines/2023/1/267976-the-end-of-programming/fulltext#R3">3</a></sup> describing the actual software built for the model: "We use the same model and architecture as GPT-2, including the modified initialization, pre-normalization, and reversible tokenization described therein, with the exception that we use alternating dense and locally banded sparse attention patterns in the layers of the transformer, similar to the Sparse Transformer. To study the dependence of ML performance on model size, we train eight different sizes of model, ranging over three orders of magnitude from 125 million parameters to 175 billion parameters, with the last being the model we call GPT-3. Previous work suggests that with enough training data, scaling of validation loss should be approximately a smooth power law as a function of size; training models of many different sizes allows us to test this hypothesis both for validation loss and for downstream language tasks."

对于任何阅读过任何现代机器学习论文的人来说，焦点从程序到模型的转变应该是显而易见的。这些论文几乎没有提及其创新背后的代码或系统；人工智能系统的构建块是更高层次的抽象，如注意力层、分词器和数据集。即使是 20 年前的时间旅行者也很难理解（75 页！）GPT-3 论文3 中描述为该模型构建的实际软件的三个句子：“我们使用与 GPT 相同的模型和架构-2，包括其中描述的修改后的初始化、预归一化和可逆标记化，除了我们在变换器的层中使用交替密集和局部带状稀疏注意模式，类似于稀疏变换器。研究依赖性ML 在模型大小上的性能，我们训练了八种不同大小的模型，范围超过三个数量级，从 1.25 亿个参数到 1750 亿个参数，最后一个是我们称为 GPT-3 的模型。以前的工作表明，在有足够的训练数据的情况下，验证损失的缩放应该近似于作为大小函数的平滑幂律；许多不同大小的训练模型允许我们针对验证损失和下游测试这个假设m 语言任务。”

This shift in the underlying definition of computing presents a huge opportunity, and plenty of huge risks. Yet I think it is time to accept that this is a very likely future, and evolve our thinking accordingly, rather than just sit here waiting for the meteor to hit.

这种计算基本定义的转变带来了巨大的机遇，同时也带来了大量巨大的风险。然而，我认为现在是时候接受这是一个很有可能的未来，并相应地改变我们的想法，而不是坐在这里等待流星撞击。

![uf1.jpg](uf1.jpg)  
**Figure. Watch the author discuss this work in the exclusive _Communications_ video. [https://cacm.acm.org/videos/end-of-programming](https://cacm.acm.org/videos/end-of-programming)  
数字。观看作者在独家通讯视频中讨论这项工作。 https://cacm.acm.org/videos/end-of-programming  
**

[Back to Top](https://cacm.acm.org/magazines/2023/1/267976-the-end-of-programming/fulltext#PageTop) 回到顶部

### References

1\. Berger, E. Coping with copilot. SIGPLAN _PL Perspectives_ Blog, 2022; [https://bit.ly/3XbJv5J](https://bit.ly/3XbJv5J)  
1\. Berger, E. 应对副驾驶。 SIGPLAN PL 观点博客，2022 年； [https://bit.ly/3XbJv5J](https://bit.ly/3XbJv5J)  

2\. Bostrom, N. _Superintelligence: Paths, Dangers, Strategies._ Oxford University Press, 2014.  
2\. Bostrom, N. 超级智能：路径、危险、策略。牛津大学出版社，2014 年。  

3\. Brown, T. et al. Language models are few-shot learners. 2020; [https://bit.ly/3Eh1DT5](https://bit.ly/3Eh1DT5)  
3\. Brown, T. 等人。语言模型是少样本学习者。 2020; [https://bit.ly/3Eh1DT5](https://bit.ly/3Eh1DT5)  

4\. Kojima, T. et al. Large language models are zero-shot reasoners. 2022; [https://bit.ly/3Ohmlqo](https://bit.ly/3Ohmlqo)  
4\. Kojima, T. 等人。大型语言模型是零样本推理机。 2022; [https://bit.ly/3Ohmlqo](https://bit.ly/3Ohmlqo)  

5\. Nye, M. et al. Show your work: Scratchpads for intermediate computation with language models. 2021; [https://bit.ly/3TLnfMY](https://bit.ly/3TLnfMY)  
5\. Nye, M. 等人。展示您的作品：使用语言模型进行中间计算的便签本。 2021; [https://bit.ly/3TLnfMY](https://bit.ly/3TLnfMY)  

[Back to Top](https://cacm.acm.org/magazines/2023/1/267976-the-end-of-programming/fulltext#PageTop) 回到顶部

### Author

**Matt Welsh** ([mdw@mdw.la](mailto:mdw@mdw.la)) is the CEO and co-founder of Fixie.ai, a recently founded startup developing AI capabilities to support software development teams. He was previously a professor of computer science at Harvard University, a director of engineering at Google, an engineering lead at Apple, and the SVP of Engineering at OctoML. He received his Ph.D. from UC Berkeley back in the days when AI was still not playing chess very well.

Matt Welsh (mdw@mdw.la) 是 Fixie.ai 的首席执行官兼联合创始人，Fixie.ai 是一家最近成立的初创公司，致力于开发 AI 功能以支持软件开发团队。他曾担任哈佛大学计算机科学教授、谷歌工程总监、苹果工程主管以及 OctoML 工程高级副总裁。他获得了博士学位。来自加州大学伯克利分校，那时候 AI 下国际象棋还不是很好。

___

Copyright held by author.  
Request permission to (re)publish from the owner/author.

版权归作者所有。 向所有者/作者请求（重新）发布的许可。

The Digital Library is published by the Association for Computing Machinery. Copyright © 2023 ACM, Inc.  
数字图书馆由计算机协会出版。版权所有 © 2023 ACM, Inc.  

___

## Comments

___

##### Ken Kahn

Agree. But even "The bulk of the intellectual work of getting the machine to do what one wants will be about coming up with the right examples, the right training data, and the right ways to evaluate the training process." might be more than what will be needed. Why wouldn't future systems largely automate this?

同意。但即使是“让机器做我们想做的事情的大部分智力工作也将是提出正确的例子、正确的训练数据以及评估训练过程的正确方法。”可能比需要的更多。为什么未来的系统不会在很大程度上实现自动化？

Also that sounds more like engineering that computer SCIENCE. Maybe a good fraction of future computer science researchers will be focussed on figuring how these systems work by analysing the behavior of small subsets of their neural networks.

这听起来更像是计算机科学的工程。也许未来的计算机科学研究人员中有很大一部分将专注于通过分析神经网络的小子集的行为来弄清楚这些系统是如何工作的。

___

##### Howard Golden

December 22, 2022 06:00

Remember Ed Yourdons prediction in 1992 (see https://en.m.wikipedia.org/wiki/Decline\_and\_Fall\_of\_the\_American\_Programmer). Matt Walshs prediction may or may not be accurate, but the timeframe isnt always clear.

___

##### Simson Garfinkel

December 23, 2022 11:53

I dont think that AI means the end of programming, but I do think that it will change the way we teach computer science.

Already it is clear that we need to be teaching all kinds of new skills, such as prompt engineering and the theory and practice of data annotation. We also need to teach how to use AI to build more complex systems. Just as todays computer science students dont need to know how to implement a language like Python but need to know how to use it, CS students of the future will need to know how to use AI effectively, and that will sure be improved with formal education.

Its also clear that computer science departments will need to be at the forefront of socio-technical issues, including understanding and counteracting systematic bias in AI systems, improving access to these systems, and making sure that the benefits of AI are shared by all. These may seem like soft social science issues, but over the past decade, weve learned that its simply not possible to address these issues without a firm grounding in computer science.

Improving cybersecurity and developing approaches for respecting privacy while making use of private data are two other areas where the need for strong education and research will continue. Yes, cybersecurity defenders make use of AI, but so do attackers: we will need the combination of human-AI teams to stay ahead of attackers. In terms of privacy, it seems unlikely that AI is likely to develop fundamentally new technical or legal approaches for protecting privacy, but we will certainly need them to keep up with the technologys challenges.

I am confident that AI will only increase the demand for CS graduates.

Simson Garfinkel

___

##### Ian Arawjo

December 27, 2022 10:05

When FORTRAN was introduced, the authors claimed that it would "virtually eliminate coding." Did it? No, but it changed what the term "coding" meant. AI tools will similarly change was "programming" means. Is that the "end" of "programming," though? Highly unlikely it is.

(See https://www.softwarepreservation.org/projects/FORTRAN/BackusEtAl-Preliminary%20Report-1954.pdf -- "Since FORTRAN should virtually eliminate coding and debugging, it should be possible to solve problems for less than half the cost that would be required without such a system.")

___

##### Tobias Pfeffer

December 28, 2022 03:10

I agree that AI models could very well displace humans as authors of simple and complex software components. However, I would argue that already today writing the actual code is only a small part of my daily work as an software engineer. Much of it is indeed spent discussing (and also finding) the correct requirements (or stories), devising the architecture, writing documentation and generally thinking about how to keep the code base maintainable. Thus, I think that "the bulk of the intellectual work of getting the machine to do what one wants will be about coming up with the right examples, the right training data, and the right ways to evaluate the training process" is probably very true, but I would say that that is already a large part of what I do as a software engineer - although maybe in a different form.

___

##### Martin Wheatman

December 30, 2022 01:53

I quite agree that the days of the programmer may indeed be numbered. However, there is another option, between the JavaScript chatbots scraping values from speech-to-text output, and (the promise of) neural nets being the true arbiter of context. And this is from one who learned Basic on an Exidy Sorcerer, took an undergraduate CS in the 1980s, and gained a PhD albeit during a 40 year career as a lowly programmer. Do you remember, in Classical CS, how the idea of programming inexorably lead to context-free languages?

The alternative is to use speech, which is certainly an information bearing medium, as a Turing Complete mechanism, by embedding an orthogonal boolean signal (Ok, . or Sorry, ) to act as a conditional, and to create loops by recursion. This follows the symbolic logic of C. S. Peirce as applied by Ogden and Richards in 1923, and the Pragmatic linguistics in the 1950s. More detail on how this works is further detailed in:  
https://www.researchgate.net/publication/365243696\_Happy\_100th\_Anniversary\_Semiotic\_Triangle

However, what this solves is the age-old problem of software engineering: the need for a written artifact. Even the above article alludes to writing a program and neural-nets requiring a few keystrokes, it comes so easily! The inductive process the creation of meaning can be described, or programmed by voice, by what an utterance implies. This too is simple science and so is evidenced by open experiment: a simple demonstration, currently with 504 unit test examples, is available at https://bitbucket.org/martinwheatman/enguage/src/develop/ (and at a similar location on github!)

It took 100 years to get from the idea of Babbages Analytic Engine to Turings idea for the Universal Machine. Perhaps it is fitting that Ogden and Richards published their Meaning of Meaning in 1923? It is here, it is now. Enjoy.

___

##### Alexander Repenning

January 01, 2023 04:50

Having used ChatGPT to help me writing code for a complex project, not just some toy CS intro examples, I found many cases where ChatGPT provided some amazingly great support beyond other resources such as StackOverflow. But, as others have found themselves, it can also produce answers that are simply wrong and do so with great confidence. In some cases it took me a long time to debug. My more general insights are these:

1) New Skills. CS competence models of the past have focused on the ability of students to ANSWER QUESTIONS. In the post-GPT era competence may need to be reconceptualized as ability to POSE QUESTIONS. The quality of an answer produced by ChatGPT is somewhat proportional to the quality of the question posed. And to ask meaningful follow up questions. Making effective use of tools such as ChatGPT develops a modern form of dialectic. This is a good thing. Entering the workforce and working in teams, past students will have to be able to master this kind of dialectic to work with fellow humans as well as with AI. In the long run, this kind of competence is likely to be more important than knowing some detail regarding a certain algorithm or specific programming language.

2) Shift in CS University Education. Working on real projects professional programmers already find value added by current AI programming support systems such as Copilot and ChatGPT. This value will only go up over time. It makes no sense to hide or forbid these systems in (not only CS) education. These systems provide new kinds of affordances that we do not fully appreciate yet. Our current mechanisms of CS skill assessment will not work well in the post-GPT era. Like it or not, students will use these new tools but in contrast to Google/StackOverflow-based approaches, there are no anti plagiarism tools to support educators. Tricky times ahead. A shift towards more project-oriented, higher level skills could help. Project portfolios instead of low level coding exams. If you want to become an architect you would not be judged how well you can hammer in a nail either.

3) Shift towards Explicative Programming in K-12 Education. Maybe The End of Programming will come to K-12 education as long as programming is only considered a recruiting mechanism for the CS education pipeline. To this day, programming is still not well received in K-12 education mostly because it does not provide measurable benefits towards non-CS subjects relevant to schools. In the post-GPT era K-12 programming with this career oriented focus, will become an even harder sell. Explicative Programming (), in contrast, is about the use of programming to develop the understanding of powerful ideas in other disciplines such as STEM, music and art by building interesting artifacts. Programming as instrument of thought is about thinking WITH computers. This kind of programming is will not end. It is about to begin.

___

##### Daniel Bilar

January 02, 2023 08:10

Practitioner's experience and comment

"I'm a pretty decent programmer. Good enough that I've made a career out of it and none of my code will (likely) ever make it to the Daily WTF. But there are programming concepts that I've always struggled to understand because frankly, the documentation is obtuse and hard to parse, and it wasn't really worth my time.

For instance, the Wikipedia entry on monads is frankly just obnoxious to read. I program in elisp a bit, so trying to understand monads is mostly about satisfying some curiosity, but something about the article just doesn't click with me and I have to move through it really slowly.

I asked ChatGPT to explain it to me in simple terms, and it did a good job. It even provided an example in JavaScript. Then I asked it to provide an example in elisp and it did that too. I'm not super concerned about correctness of the code, as long as it's generally okay, and it seems to have done an okay job.

I've also asked it to document some elisp functions that I've always thought were poorly described (emacs' documentation can really be hit or miss) and it really did a great job.

I'm not so arrogant as to say that these models won't one day generate a lot of good, usable code, but I honestly think that this ability to collate a tonne of data and boil it down to something understandable could fill in the gaps in a lot of documentation. The longest, most tedious parts of my job very often boil down to research for some engine-specific feature that I need, or some sort of weird platform quirk. For publicly available engines like Unreal, this will honestly improve my productivity quite a lot."

___

Displaying **all 8** comments

###### Article Contents:

-   [Article](https://cacm.acm.org/magazines/2023/1/267976-the-end-of-programming/fulltext#body-1)
-   [References](https://cacm.acm.org/magazines/2023/1/267976-the-end-of-programming/fulltext#references)
-   [Author](https://cacm.acm.org/magazines/2023/1/267976-the-end-of-programming/fulltext#authorinfo)