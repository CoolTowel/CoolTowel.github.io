---
title: 国际天球参考系统 —— ICRS 简介
date: 2018-04-16 17:25:26
categories: 天文
tags:
  - 天文
---
前两日处理一些个天文数据，做的过程中发现自己以前对于天文参考系的认知还是太少，查了些资料后才有些更深入的了解。趁着刚开博客的热乎劲，随便写点儿凑个数。<!-- more -->

## ICRS是什么

<blockquote>国际天球参考系统 （ICRS）是国际天文联合会（IAU）目前采用的天球参考系统标准。它在 1997 年的第 23 届大会上通过，并于 1998 年起正式采用。它的原点是广义相对论框架下的 VLBI 测定的太阳系的质心，极轴的指向在太空中是"固定的"，赤经原点由 3C273B 标定。ICRS的内容大致与赤道座标系统是协调一致的：ICRS J2000.0 的平均极点在 12 h 的方向是 17.3±0.2 mas，在 18 h 的方向是 5.1±0.2 mas；平均分点在垂直于极轴的方向上从 ICRS 赤经原点移动了 78±10 mas。<p align="right">——<a href="https://www.iers.org/IERS/EN/Science/ICRS/ICRS.html">www.iers.org</a></p></blockquote>

本文将就这段话中的几个概念进行简要介绍。


## 什么是赤道坐标系
要理解ICRS首先要知道什么是赤道坐标系。所谓坐标就是给天上的天体定个位置，以便不同的天文工作者可以知道对方所指的某某天体究竟是哪个。

天文坐标系统其实自古有之，从中国古代的星官，到古希腊的星座，其实都可以看作是一种粗略的定位与坐标。再后来，人们运用数学、借助工具（比如浑仪、简仪）从实际的天文观测中抽象出了一套坐标系。其中就有赤道坐标系。这一坐标系不是任取的，而是从天体运行规律——周日视运动——中总结出来的。周日视运动其实就是地球的自转。赤道坐标系是当今天文学界使用最广泛的坐标系统，这一系统有诸多优点，我从个人的角度有这么两点：
+ 物理意义明确
+ 对实际的望远镜观测友好

首先物理意义明确是指该球面坐标系的极点就是地球自转轴与天球的交点，那么自然其赤道就是地球的赤道，事实上这也是为什么叫赤道坐标系的原因。

<a title="By Tfr000 (talk) 20:50, 17 April 2012 (UTC) [CC BY-SA 3.0 (https://creativecommons.org/licenses/by-sa/3.0) or GFDL (http://www.gnu.org/copyleft/fdl.html)], from Wikimedia Commons" href="https://commons.wikimedia.org/wiki/File:Ra_and_dec_demo_animation_small.gif"><img width="256" alt="Ra and dec demo animation small" src="https://upload.wikimedia.org/wikipedia/commons/6/66/Ra_and_dec_demo_animation_small.gif"></a>

上图展示了如何从地球的自转构建赤道坐标系。

其次是对于望远镜观测友好。为什么这样说呢，因为现代的望远镜大都使用赤道仪这一额外的设备来抵消地球的自转（一些口径过于大的则不使用），这就使得控制望远镜方向的两个轴就恰好对应着赤道坐标系中的两个的参数——赤经与赤纬。如果你要从一个已对准的目标转向另一个目标，则可以将两个方向上的差值算出，直接应用到赤道仪的两个轴上，来指向目标。

当然，这样也有缺点，就是对于在地球上的观测者，天体的实际方位不明确，需要知道当地的纬度（可以通过观测北极星来获知）及恒星时来确定天体方位，还要经过一番换算。不过，其他坐标系同样有这样的缺点，好在我们有手机星软件可以实时提供天体方位。

## ICRS的实现

在此之前，我对坐标系大部分的了解也就是前面一节中的那些了。但是这些最基础的定义，还并不能告诉我们某一天体的方位，除了坐标系，我们还需要参考系。

坐标系是一个数学概念，而参考系则要依靠物理实体（当然其中缺少不了数学）。我们都知道，确定一个物体的运动（运动事实上也就是位置）需要一个参照物。依据一个特定的参照物，选取一个坐标系，我们会得到一个物理上的参考系。

ICRS 中的坐标系统与赤道坐标系基本一致，重点在于如何选取参照物。

在通常的赤道坐标系中，我们规定太阳的春分点所在的位置为赤经零点，但是事实上，春分点并不是恒久不变的。由于地球的进动以及章动，春分点无时无刻不在运动着。进动是指地球自转轴绕着空间中的另一个轴旋转，章动则是在进动的过程中更加微小的运动。

<a title="By User Herbye (German Wikipedia). Designed by Dr. H. Sulzer (Original) [GFDL (http://www.gnu.org/copyleft/fdl.html) or CC-BY-SA-3.0 (http://creativecommons.org/licenses/by-sa/3.0/)], via Wikimedia Commons" href="https://commons.wikimedia.org/wiki/File:Praezession.svg"><img width="256" alt="Praezession" src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/bb/Praezession.svg/256px-Praezession.svg.png"></a>

<center><b>P 和 N 分别是进动与章动 </b><center>

因此，ICRS 选择使用几乎“恒久不动”的河外天体作为参照物，这就是 ICRF（International Celestial Reference Frame）——国际天球参考框架。

ICRF 是一系列河外源的精确位置，这些源通常是遥远的类星体，它们足够遥远，以保证这一参考框架的“惯性”性以及稳定性，这其中就有著名的也是第一个被发现类星体 3C 273。通过 VLBI——甚长基线射电干涉测量技术，我们可以将这些射电源的位置精确到数个毫角秒以内，以保证 ICRS 的精确性。

在 20 世纪，天文学家使用 FK5 星表实现他们的天球参考系统（自然的，它被 IAU 承认）。FK5 星表是由 Walter Fricke 等人于 1988 发表的一份包含了数千个恒星的位置的星表。天文学家依据该表中恒星的位置来标定未知天体的位置。星表中的恒星就好比画图纸中的网格线一样，是参考系的基石。但是由于恒星的自行，FK5 星表的精度无法与 ICRF 媲美。这是因为 ICRF 是基于遥远的河外天体，这些河外天体距离地球达数十亿光年甚至更远，而 FK5 使用的银河系内的恒星仅仅在几十万光年外。

{% asset_img icrf2.png %}

<center><b>最新的 ICRF2 中射电源的分布 </b> <I>来自：<a href:"http://hpiers.obspm.fr/icrs-pc/newwww/index.php">IERS ICRS Center</a></I> <center>

不过，所有基于 VLBI 技术的结果都是在射电波段的，在其他的波段还需要其他的观测数据。在光学波段，ICRF 采用依巴谷星表（这是依巴谷空间望远镜的成果）作为其光学实现，并且通过一些观测手段，将其与 VLBI 的观测结果相联系，共同组成 ICRF。

## 什么是 J2000.0

根据 ICRS 的定义，它的极点与赤经原点都是相对于遥远类星体不动的(在观测误差之内），这样一来，ICRS 就成为了一个在（天文学意义上的）短期内不会在空间中发生变化的坐标系。这使得 ICRS 变成了完全独立于地球运动的一个参考系，这是与赤道坐标系的初衷相悖的。

根据前面所说的地球自转的不稳定性，可以知道：对于一个时刻的天空，如果采用那个时刻真正的春分点与地球自转轴建立赤道坐标系，那么天文学家之间的沟通将无法进行——因为这个坐标系无时无刻不在变动。所以天文学家约定采取某一个时刻的地球运行状态作为赤道坐标系的基准。

现如今这个约定的时刻是 J2000.0，J 代表儒略纪元，2000.0 代表 2000 年一月一日（具体的时刻因时间系统的差异而有微小差别，但是是地球时的中午十二时整），简单来说就是公元 2000 年的第一天中午。在此之前，天文学家采用的是 B1950.0，简单来说是 1950 年的第一天。

那么我们来看，所谓的 J2000.0 在 ICRS 这个“永恒不动”的坐标系的位置：

{% asset_img The_International_Celestial_Ref.gif %}

<center> <I>来自：<a href:"https://www.iers.org/IERS/EN/Science/ICRS/pole_and_right_ascensions_origin.html">www.iers.org/IERS/EN/Science/ICRS/pole_and_right_ascensions_origin.html</a></I> <center>

图中的大圈是 FK5 星表中极点位置的误差圈，mas 是单位：毫角秒。可见新老系统是一致兼容的，并且事实上，一般光学波段成像的误差也达不到毫角秒的量级。

## 其他

其实这只是介绍了坐标系中空间的一部分。根据广义相对论 ，时间受到引力的影响，而一个完整的物理的参考系，不能没有时间。天文学中时间也是复杂而有趣的，不过本人才疏学浅，还未能有一个全面详尽的理解，以后学了相关的再来写一篇天文学中的时间好了（flag）。

## 参考文献

+ 《时空参考系》 科学出版社 Soffel, M. 等著；王若璞，赵东明译
+ <a href:"http://hpiers.obspm.fr/icrs-pc/newwww/index.php">IERS ICRS Center</a>
+ <a href:"https://www.iers.org/IERS/EN/Home/home_node.html">IERS</a>
