---
title: 前方的另一条路-新
pubDate: 2001-01-01
---

> 原文：https://www.paulgraham.com/road.html 

            markdown
2001年9月

_（本篇文章基于在BBN实验室的一次演讲，解释了为什么未来一大批软件将基于服务器运行，这一趋势对程序员意味着什么，以及为何这对创业公司而言是个巨大的机遇。）_

1995年夏，我和我的朋友 Robert Morris 决定创业。那时，随着 Netscape 即将上市，关于在线商务的讨论铺天盖地。实际上，网上仅有大约三十家真正的商店，都是手工搭建的。如果未来网上商店数量激增，就必须有专门的软件来创建它们，因此我们决定开发这样的软件。

最初的一周左右，我们计划开发一款传统的桌面应用。但某天，我们萌生了一个想法，为何不让软件运行在我们的 Web 服务器上，并通过浏览器作为操作界面呢？我们尝试将软件改写为 Web 版本，结果明显这是正确的方向。如果软件运行在服务器上，对用户和我们自己来说都会更简单。

这个计划证明是成功的。如今，作为 [Yahoo Store](http://store.yahoo.com)，这款软件成为了最受欢迎的在线商店构建工具，拥有约 14,000 名用户。

当我们开始 Viaweb 时，几乎没人理解我们所说的“软件运行在服务器上”是什么意思。直到一年后 Hotmail 推出，人们才开始明白这一概念。现在，每个人都知道这是一种可行的方法。我们当时所做的，现在有了一个名字：应用服务提供商，或 ASP。

我认为未来很多软件都将采用这种模式编写。即便是 Microsoft——他们最不愿看到这种变化的公司，似乎也认识到了有些事情必须从桌面转移到服务器上。如果软件从桌面搬到服务器，这将为开发者带来一个截然不同的世界。本文描述了我们作为这个新世界最早的探索者所见到的一些惊奇。在软件确实转移到服务器上的程度上，我在这里所描述的，即是未来。

**下一个大事件？**

当我们回顾桌面软件时代，我相信我们会对人们容忍的不便感到惊讶，正如我们现在对早期汽车所有者所忍受的不便感到惊讶一样。在最初的二三十年里，你必须是汽车专家才能拥有汽车。但汽车带来的巨大好处让许多非专家也想拥有它们。

计算机现在正处于这个阶段。当你拥有一台桌面计算机时，你最终会学到关于它内部的更多知识，超出了你本想了解的。但在美国，超过一半的家庭拥有一台。我的母亲有一台她用来发送电子邮件和记账的电脑。大约一年前，她惊慌地收到一封来自 Apple 的信，提供给她一个新版本操作系统的折扣。一个 65 岁的老太太想要使用电脑发送电子邮件和记账，却不得不考虑安装新操作系统，这里显然出了问题。普通用户甚至不应该知道“操作系统”这个词，更不用说“设备驱动程序”或“补丁”了。

现在，有了另一种交付软件的方式，可以让用户免于成为系统管理员。基于 Web 的应用程序是在 Web 服务器上运行并使用 Web 页面作为用户界面的程序。对于普通用户来说，这种新型软件将会更简单、更便宜、更便携、更可靠，而且通常比桌面软件更强大。

使用基于 Web 的软件，大多数用户不必考虑除了他们使用的应用程序之外的任何事情。所有混乱、变化的东西都会坐落在某个服务器上，由那些擅长此类事情的人来维护。因此，你通常不需要一台计算机，只需要有键盘、屏幕和 Web 浏览器的东西。也许它会有无线互联网接入。也许它还会是你的手机。无论它是什么，它都将是消费电子产品：大约 200 美元的东西，人们主要根据外壳的外观来选择。你将为互联网服务支付的费用比硬件更多，就像你现在对电话所做的那样。[1](#the_other_road_ahead_note1)

对于需要大量交互的软件用户，比如 Photoshop，他们仍然希望计算发生在桌面上。但如果你看看大多数人使用计算机做的事情，十分之一秒的延迟不会是问题。我的母亲并不真正需要一台桌面计算机，而且有很多像她这样的人。

**用户的胜利**

我家附近有一辆车，保险杠上贴着一个标语，写着“宁死不受不便”。大多数人，在大多数时候，会选择需要最少工作的选项。如果基于 Web 的软件获胜，那将是因为它更方便。看起来它会更方便，对用户和开发者都是如此。

使用纯粹基于 Web 的应用程序，你所需要的只是一个连接到互联网的浏览器。所以你可以在任何地方使用基于 Web 的应用程序。当你在桌面计算机上安装软件时，你只能在那台计算机上使用它。更糟糕的是，你的文件被困在那台计算机上。随着人们习惯于网络，这种模式的不便越来越明显。

这里的突破口是基于 Web 的电子邮件。现在数以百万计的人意识到，无论你在哪里，都应该可以访问电子邮件消息。如果你可以查看你的电子邮件，为什么不可以查看你的日历呢？如果你可以和同事讨论一个文档，为什么不能编辑它呢？为什么你的任何数据都应该被困在某台远处桌子上的计算机上呢？

“你的计算机”的整个概念正在消失，被“你的数据”所取代。你应该能够从任何计算机获取你的数据。或者说，任何客户端，而客户端不必是一台计算机。

客户端不应该存储数据；它们应该像电话一样。事实上，它们可能会变成电话，反之亦然。随着客户端变得更小，你有另一个理由不将数据保存在它们身上：你随身携带的东西可能会丢失或被盗。在出租车里遗忘你的 PDA 就像硬盘崩溃一样，只不过你的数据是交给了[某人](http://news.zdnet.co.uk/business/0,39020645,2077931,00.htm)而不是被消灭。

使用纯粹基于 Web 的软件，你的数据和应用程序都不会保存在客户端上。所以你不必安装任何东西就可以使用它。当没有安装时，你就不必担心安装出错。应用程序和你的操作系统之间不可能有不兼容，因为软件不在你的操作系统上运行。

因为不需要安装，尝试基于 Web 的软件将会很容易，也很常见。你应该期望能够免费试用任何基于 Web 的应用程序，只需访问提供它的网站。

在 Viaweb，我们的整个网站就像一个大箭头，指引用户进行试用。

在尝试了演示版之后，注册服务应该只需要填写一个简短的表格（越简短越好）。那应该是用户需要做的最后一项工作。使用基于 Web 的软件，你应该可以在不支付额外费用、不做任何工作，甚至