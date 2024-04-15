---
title: programming_bottomup
pubDate: 1993-04
---

> 原文：https://www.paulgraham.com/progbot.html 

            
1993年

编程风格中长期以来的一个原则是程序的功能部分不应该过于庞大。如果程序的某个组成部分增长到难以理解的阶段，它就会变得复杂，就像大城市隐藏逃犯一样容易掩盖错误。这样的软件将难以阅读、难以测试和难以调试。

根据这个原则，一个大型程序必须分割成若干部分，而程序越大，分割得越细。如何分割一个程序？传统方法称为“自顶向下设计：”你说“程序的目的是做这七件事，所以我将它分成七个主要子程序。第一个子程序要做这四件事，所以它反过来将有四个自己的子程序”，依此类推。这个过程持续进行，直到整个程序具有正确的粒度--每个部分足够大以执行实质性工作，但又足够小以被理解为一个单一单元。

有经验的 Lisp 程序员以不同的方式分割他们的程序。除了自顶向下设计，他们遵循一种可以称为“自底向上设计”的原则--根据问题改变语言。在 Lisp 中，你不仅仅是朝着语言编写程序，你还会朝着程序构建语言。当你编写程序时，你可能会想“我希望 Lisp 有这样那样的操作符。” 于是你去写它。之后你意识到使用新的操作符会简化程序的另一部分的设计，依此类推。语言和程序一起演化。就像两个交战国家之间的边界一样，语言和程序之间的边界被画出并重新绘制，直到最终停在问题的自然边界--山川之间。最终，你的程序看起来就好像语言是为它设计的。当语言和程序彼此很好地契合时，你将得到清晰、简洁和高效的代码。

值得强调的是，自底向上设计并不仅仅意味着用不同的顺序编写相同的程序。当你自底向上工作时，你通常会得到一个不同的程序。你将得到一个更大的语言，具有更抽象的操作符，以及一个更小的程序在其中编写。你将得到一个拱门，而不是横梁。

在典型的代码中，一旦你提取出仅仅是簿记的部分，剩下的会更短；你构建语言的层次越高，你就不必从顶部向下到达的距离就越短。这带来了几个优势：

1. 通过让语言做更多的工作，自底向上设计产生了更小、更灵活的程序。一个较短的程序不必分成那么多组件，少了组件意味着更容易阅读或修改的程序。更少的组件还意味着更少的组件之间的连接，因此在那里出错的机会更少。正如工业设计师努力减少机器中运动部件的数量一样，有经验的 Lisp 程序员使用自底向上设计来减少他们程序的大小和复杂性。

2. 自底向上设计促进代码重用。当你编写两个或更多个程序时，你为第一个程序编写的许多实用工具也将对后续程序有用。一旦你获得了大量的实用工具，编写新程序所需的工作量可能只是从头开始写 Lisp 所需工作量的一小部分。

3. 自底向上设计使程序更容易阅读。这种类型的抽象要求读者理解一个通用操作符；功能抽象的一个实例要求读者理解一个特定目的的子程序。

4. 因为它使你始终警惕代码中的模式，自底向上工作有助于澄清你对程序设计的想法。如果程序的两个远程组件在形式上相似，你将被引导注意到这种相似之处，也许会以更简单的方式重新设计程序。

在除了 Lisp 之外的其他语言中，一定程度上也可以进行自底向上设计。每当你看到库函数时，自底向上设计就会发生。然而，在这方面 Lisp 给了你更广泛的权力，并且增强语言在 Lisp 风格中起着更大的作用--以至于 Lisp 不仅仅是一种不同的语言，而是一种完全不同的编程方式。

确实，这种开发风格更适合可以由小团队编写的程序。然而，与此同时，它扩展了小团队能够完成的工作范围。在《人月神话》中，Frederick Brooks提出，一个程序员小组的生产力并不会随着规模的增长而线性增长。随着团队规模的增加，单个程序员的生产力会下降。Lisp 编程的经验提出了一个更愉快的表述这个定律的方式：随着团队规模的减小，单个程序员的生产力会提高。相对而言，小团队胜出，仅仅因为它更小。当一个小团队还利用 Lisp 可能的技术时，它可以赢得胜利。

**新内容：** [免费下载《On Lisp》](onlisptext.html)。