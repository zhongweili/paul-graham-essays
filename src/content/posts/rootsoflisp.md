---
title: the_roots_of_lisp
pubDate: 2007-02-02
---

> 原文：https://www.paulgraham.com/rootsoflisp.html 

            
2001年5月，我写了这篇文章，以帮助自己更好地理解麦卡锡的发现。虽然你在Lisp中编程并不需要了解这些，但对于想要理解Lisp本质的人来说，这应该是有帮助的 —— 无论是从起源还是语义核心的角度。Lisp之所以与众不同，一个显著特征是它有一个核心，这也是与其他语言不同之处，也是Lisp有方言的原因。

1960年，约翰·麦卡锡发表了一篇引人注目的论文，他在其中为编程做了一些类似于欧几里得为几何所做的事情。他展示了如何通过一小部分简单操作符和函数符号表示，就可以构建一个完整的编程语言。他将这种语言称为Lisp，即“列表处理”，因为他的一个关键想法是使用一种称为“列表”的简单数据结构来表示代码和数据。

了解麦卡锡的发现是值得的，这不仅是计算机历史上的一个里程碑，也是我们这个时代编程趋势的一个模型。在我看来，到目前为止有两种非常干净、一致的编程模型：C模型和Lisp模型。这两个模型似乎是高地，它们之间有沼泽般的低地。随着计算机变得更加强大，新开发的语言一直在向Lisp模型靠拢。过去20年中新编程语言的一个流行方案是将C模型的计算方式添加部分Lisp模型的元素，如运行时类型检查和垃圾回收。

在本文中，我将尝试以最简单的术语解释麦卡锡的发现。重点不仅是学习四十年前某人想出的一个有趣的理论结果，而是展示语言的发展方向。Lisp的不寻常之处 —— 实际上，Lisp的定义特性 —— 是它可以用自身编写。为了理解麦卡锡这样说的含义，我们将重走他的脚步，将他的数学符号翻译成运行的Common Lisp代码。