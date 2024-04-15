---
title: javas_cover
pubDate: 2005-12-13
---

> 原文：https://www.paulgraham.com/javacover.html 

            
2001年4月

这篇文章是我与其他程序员关于为什么 Java 有可疑之处的讨论的结果。这并不是对 Java 的批评！而是对黑客雷达的一个案例研究。

随着时间的推移，黑客们对技术的好坏有了一种直觉。我觉得尝试写下 Java 为何让我感到可疑可能会很有趣。

有些人读过这篇文章后认为这是一个有趣的尝试，写出了以前没有人写过的东西。其他人则说我可能会因为似乎在写自己不了解的东西而惹上麻烦。所以，以防有所作为，让我澄清一下，我在这里写的不是关于 Java（我从未使用过）而是关于黑客雷达（我思考过很多）。

***

俗语“书不能以其封面判断”起源于书籍在普通硬纸板封面上销售的时代，每位购买者都可以根据自己的口味装订。在那个时代，你无法通过封面判断一本书。但出版业已经进步了：现代出版商努力让封面成为你可以通过它判断一本书的东西。

我在书店里花了很多时间，我觉得我现在已经学会了理解出版商想要告诉我的关于一本书的一切，也许还多一点。我没有在书店里度过的时间，我大部分时间都花在电脑前，我觉得我在某种程度上也学会了通过封面来评判技术。也许只是运气好，但我避免了一些后来证明是真正糟糕的技术。

到目前为止，Java 对我来说看起来像一个糟糕的东西。我从未写过 Java 程序，对它的参考书籍也只是粗略地瞥了一眼，但我有一种直觉，它不会是一种非常成功的语言。我可能会被证明是错的；对技术做出预测是一项危险的事业。但就它的价值而言，作为一种时间胶囊，这就是为什么我不喜欢 Java 的原因：

1. 它被过分炒作。真正的标准不需要推广。没有人需要推广 C、Unix 或 HTML。一个真正的标准往往在大多数人听说之前就已经建立起来了。在黑客雷达屏幕上，Perl 的地位与 Java 相当，甚至更大，仅仅凭借其自身的优点。

2. 它的目标太低。在最初的 Java 白皮书中，Gosling 明确表示 Java 的设计并不是为了对习惯于 C 的程序员来说太困难。它被设计成另一个 C++：C 加上一些从更高级语言中借鉴的想法。像情景喜剧、垃圾食品或包裹旅行一样，Java 的设计者们有意地为不如他们聪明的人设计了一个产品。从历史上看，为其他人设计的语言通常很糟糕：Cobol、PL/I、Pascal、Ada、C++。好的语言是那些为自己的创作者设计的语言：C、Perl、Smalltalk、Lisp。

3. 它有别有用心。有人曾说，如果人们写书只是因为有话要说，而不是因为他们想写书，那么这个世界将会更美好。同样，我们之所以一直听说 Java，并不是因为它对编程语言有什么新的见解。我们之所以听说 Java，是因为 Sun 打算通过 Java 打击微软。

4. 没有人喜欢它。C、Perl、Python、Smalltalk 和 Lisp 程序员喜欢他们的语言。我从未听说过有人说他们喜欢 Java。

5. 人们被迫使用它。我认识的许多使用 Java 的人之所以使用它，是因为他们觉得自己不得不使用。要么是他们觉得这是他们为了获得资金而必须做的事情，要么是他们认为客户会想要这样做，要么是他们被管理层告知要这样做。这些都是聪明人；如果这项技术很好，他们本来会自愿使用的。

6. 它有太多厨师。最好的编程语言是由小团队开发的。Java 似乎是由一个委员会管理的。如果 Java 最终成为一种好的语言，那将是历史上第一次委员会设计了一种好的语言。

7. 它官僚主义。就我对 Java 的了解，似乎有很多做事的协议。真正好的语言不是这样的。它们让你做你想做的事