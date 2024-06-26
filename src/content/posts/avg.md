---
title: 击败平均水平
pubDate: 2003-01-01
---

> 原文：https://www.paulgraham.com/avg.html 

            
006 打败平均水平

想要创业吗？获得[Y Combinator](http://ycombinator.com/apply.html)的资助。

2001年4月，修订于2003年4月

（本文源自2001年Franz开发者研讨会上的演讲。）

1995年夏天，我的朋友罗伯特·莫里斯和我创办了一家名为Viaweb的初创公司。我们的计划是编写软件，让最终用户建立在线商店。当时这款软件的新颖之处在于，它在我们的服务器上运行，使用普通的网页作为界面。

这个软件的另一个不同寻常之处在于，它主要使用一种叫做Lisp的编程语言编写。这是第一个主要由最终用户编写的大型应用程序之一，迄今为止，Lisp主要用于大学和研究实验室。

**秘密武器**

埃里克·雷蒙德写了一篇名为“如何成为黑客”的文章，在其中，他告诉那些想成为黑客的人应该学习哪些编程语言。他建议从Python和Java开始，因为它们易学。认真的黑客还会想学习C，以便破解Unix，以及Perl用于系统管理和cgi脚本。最后，真正认真的黑客应该考虑学习Lisp：

> 学习Lisp是值得的，因为当你最终掌握它时，你将获得深刻的启迪体验；即使你以后实际上并不经常使用Lisp，这种体验也会让你成为更好的程序员，直到你的余生。 

这与学习拉丁语的理由相同。它不会让你找到工作，除非可能成为古典教授，但它会提高你的思维，让你成为使用英语等你想要使用的语言的更好的作者。

但等一下。这个比喻并不适用那么远。拉丁语不会让你找到工作，因为没有人说它。如果你用拉丁语写作，没有人能理解你。但Lisp是一种计算机语言，计算机会用你，程序员，告诉它们的任何语言来交流。

因此，如果Lisp确实能让你成为更好的程序员，就像他说的那样，为什么你不想使用它呢？如果一个画家被提供一支可以让他成为更好画家的画笔，我觉得他会想在所有的画作中使用它，不是吗？我并不是在取笑埃里克·雷蒙德。总的来说，他的建议是好的。他对Lisp的评价基本上是传统智慧。但传统智慧中存在矛盾：Lisp会让你成为更好的程序员，但你却不会使用它。

为什么不呢？毕竟，编程语言只是工具。如果Lisp确实能产生更好的程序，你应该使用它。如果不能，那谁需要呢？

这不仅仅是一个理论问题。软件是一个非常竞争激烈的行业，容易产生自然垄断。一个能更快更好地编写软件的公司，在其他条件相同的情况下，将使其竞争对手破产。当你开始一家初创公司时，你会非常敏锐地感受到这一点。初创公司往往是赢或输的命题。要么你变得富有，要么一无所有。在初创公司中，如果你押注在错误的技术上，你的竞争对手将击败你。

罗伯特和我都很了解Lisp，我们看不到任何理由不信任我们的直觉并选择Lisp。我们知道其他人都在用C++或Perl编写他们的软件。但我们也知道这并不意味着什么。如果你那样选择技术，你就会在运行Windows。当你选择技术时，你必须忽略其他人在做什么，只考虑哪种技术最有效。

在1995年，我们了解到一些我们的竞争对手不明白的东西，甚至现在很少有人明白：当你在写只需要在自己的服务器上运行的软件时，你可以使用任何你想要的语言。当你在写桌面软件时，有一种强烈的偏见，倾向于使用与操作系统相同的语言。十年前，编写应用程序意味着用C语言编写应用程序。但是对于基于Web的软件，特别是当你同时拥有语言和操作系统的源代码时，你可以使用任何你想要的语言。

这种新的自由是一把双刃剑。现在你可以使用任何语言，你必须考虑使用哪一种。那些试图假装一切都没变的公司，可能会发现他们的竞争对手并不这样认为。

如果你可以使用任何语言，你会选择