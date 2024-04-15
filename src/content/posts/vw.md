---
title: snapshot_viaweb_june_1998
pubDate: 1998-01-01
---

> 原文：https://www.paulgraham.com/vw.html 

            
2012 年 1 月

1998 年 6 月雅虎收购宣布前几个小时，我拍摄了 Viaweb 网站的一个快照。我觉得有一天可能会有趣看看。

首先映入眼帘的是页面有多小。1998 年的屏幕要小得多。如果我没记错的话，我们的首页过去只能适应人们当时通常使用的窗口大小。

那时的浏览器（IE 6 还有 3 年才会出现）字体很少，而且没有反锯齿。如果你想让页面看起来好看，就得将显示文本渲染为图片。

你可能会注意到 Viaweb 和 Y Combinator 的标志有某种相似之处。我们在创办 YC 时就是为了开个玩笑这么做的。考虑到一个红色圆圈有多基本，当我们创办 Viaweb 时，我感到惊讶的是有多少其他公司没有用它作为他们的标志。稍后我意识到了原因。

在公司页面上，你会注意到一个叫 John McArtyem 的神秘人物。罗伯特·莫里斯（又名 Rtm）在 Worm 事件后对媒体报道非常敏感，他不想让自己的名字出现在网站上。我设法说服他同意一个妥协：我们可以使用他的简历，但不用他的名字。他后来在这一点上有所放松。

特雷弗在收购完成时差不多同时毕业，所以在 4 天内，他从一名贫穷的研究生变成了百万富翁博士。我作为一名新闻稿作家的巅峰是庆祝他的毕业，配有我在会议期间为他画的一幅图。

在 90 年代，要吸引用户，你必须在杂志和报纸中被提及。当时没有像今天这样在线被发现的方式。所以我们过去会支付一个公关公司每月 16,000 美元来让我们在媒体中被提及。幸运的是，记者喜欢我们。

在我们关于从搜索引擎获取流量的建议中（我认为当时还没有 SEO 这个词），我们说只有 7 个搜索引擎很重要：Yahoo、AltaVista、Excite、WebCrawler、InfoSeek、Lycos 和 HotBot。注意到什么遗漏了吗？Google 是在那年 9 月成立的。

我们通过一个叫做 Cybercash 的公司支持在线交易，因为如果我们缺少这个功能，我们在产品比较中就会被打败。但 Cybercash 太差劲了，大多数商店的订单量很低，所以最好是让商家像电话订单一样处理订单。我们在网站上有一个页面，试图劝说商家不要进行实时授权。

整个网站都像一个漏斗一样组织，将人们引导到试用页面。在线试用软件是一件新鲜事。我们在动态 URL 中放入 cgi-bin 来愚弄竞争对手关于我们的软件如何工作的。

我们有一些知名用户。不用说，Hollywood 的 Frederick's 流量最大。我们对大型商店收取每月 300 美元的固定费用，所以拥有大量流量的用户让人有点担心。我曾经计算过 Frederick's 在带宽方面给我们造成的成本，大约是每月 300 美元。

因为我们托管了所有商店，这些商店在 1998 年 6 月的页面浏览量总共超过 1000 万，我们消耗的带宽在当时看起来很多。我们的办公室有 2 条 T1 线路（3 Mb/秒）。那时候还没有 AWS。即使合租服务器看起来太冒险，因为经常出现问题。所以我们把服务器放在办公室里。更准确地说，放在了特雷弗的办公室。作为与其他人共享他的办公室的独特特权，他不得不与 6 台尖叫的塔式服务器共享。他的办公室因此被昵称为热水池。大多数时候他的一堆窗式空调可以跟得上。

为了描述页面，我们有一种模板语言叫做 RTML，据说代表着某个意思，但事实上我是以 Rtm 的名字命名的。RTML 是 Common Lisp 加上一些宏和库，隐藏在一个结构编辑器下，看起来像是有语法。

由于我们进行持续发布，我们的软件实际上没有版本。但在那个时代，行业媒体期望有版本，所以我们就编造了版本号。如果我们想引起很多关注，我们就会把版本号设置为整数。顺便说一句，整个 Viaweb 网站都是用我们的软件制作的，尽管它不是一个在线商店，因为我们想体验我们的用户所经历的。

1997 年底，我们发布了一个通用购物搜索引擎叫做 Shopfind。那个时候它很先进。它有一个可编程的网络爬虫，可以爬取大多数不同的在线商店，并挑选出产品。