---
title: chapter 2 Variables
date: 2024-11-28 00:02:00
type: "tags"
tags:
  - math
categories: an introduction to mathematics
mathjax: true
---

## 变量 Variables[ ˈverɪəbl]


数学作为一门科学起源于某人（可能是希腊人）首次证明了关于某些事物（something）或任何事物（anything）的命题，而这些命题并不需要具体指定某个确定的事物。这些命题最初是由希腊人提出并应用于几何学，因此，几何学成为了古希腊的重要数学科学。在几何学兴起后的几个世纪里，尽管一些后来的希腊数学家对代数有一些初步的认识，但代数直到很久之后才真正开始起步。
<!--more-->
通过使用字母替代算术中的具体数字，代数中引入了任意（any）和某些（some）的概念。因此，在代数中，我们不会去说2+3=3+2（表示交换律），而是概括地说，如果 $x$ 和 $y$ 代表任意（any）两个数字，则 $x+y=y+x$。同样，在说 $3>2$ 的时，我们概括地说，如果 x 是任意(any)数字，则存在某个（some）数（或某些数）$y$，使得$y>x$。顺便提一下，这后一种说法，严格来说，只是一个假设，但它对哲学和数学都至关重要；因为通过它，无限的概念被引入。也许，正是通过引入阿拉伯数字，在数学中完全放弃了将字母作为具体数字的用法，从而向数学家们展示了使用字母表示任意数字和某些数字的技术便利。罗马人会用MDCCCCX表示写这篇文章的年份，而我们写作1910，因此留下了字母供其他用途。但这只是一种猜测。代数兴起后，牛顿和莱布尼茨发明了微积分，数学思想的哲学进展在这些概念方面出现了停顿；直到最近几年才意识到，$any$和$some$对数学的本质有多么重要，这从而开辟了更多数学探索的课题。

现在让我们做一些简单的代数陈述，目的是确切地理解这些基本概念是如何产生的。

（1）对于任意（any)数x，x+2=2+x；

（2）对于某些（some）数x，x+2=3；

（3）对于某些（some）数x，x+2>3；

第一个要注意的是，在这里使用的某些（some）一词所包含的可能性。由于对于任意（any）数字x，x+2=2+x成立，因此对于某些（some）数字x也成立。因此，如此使用时，任意（any）必然包含某些（some），而某些（some）并不能排除掉任意（any）。然而，在第二个例子中，实际上只有一个（oneonly）数字x，符合x+2=3，只有数字1。因此，某些（some）可能只是那一个数字。但在第三个例子中，大于1的任意（any）数字x都满足x+2>3。因此，在这种情况下，有无穷多个数字与某些（some）对应。因此，某些（some）可能是介于任意（any)和只有一个（oneonly）之间的包括这两种极限情况任意情况。

陈述(2)和(3)很自然地被以下问题取代：

(2‘)什么数满足x+2=3

(3‘)什么数满足x+2>3

将陈述(2')，x+2=3看作是一个方程（equation），很容易看出它的解（solution）是x=3-2=1。当我们回答这个包含方程x+2=3的陈述时，x被称为未知数（unknown）。解方程的目的是确定未知数的值。方程在数学中很重要，似乎(2')展示了比原始陈述(2)更为彻底和基础的想法。然而，这是一个完全错误的观点。在数学中，在使用某些（some）或任意（any)中出现的未确定的“变量（variable）”的概念才是真正重要的；而在方程中，需要尽快解决的“未知数（unknown）”的概念只是次要的，尽管它当然也是非常重要的。初等代数中许多问题显得琐碎的一个原因是教科书过于关注解方程式。同样的说法适用于不等式(3')与原始陈述(3)的对比。

但是，大多数有趣的公式，特别是当涉及某些（some ）概念时，通常包含多个变量（variable）。例如，思考一对数字 x 和 y（可以是分数或整数），满足 x+y=1 ，涉及两个相关变量 x 和 y 的概念。往往当存在两个变量时，会出现相同的两种主要类型的陈述。例如，(1) 对于任意（any)一对数字 x 和 y，有 x+y=y+x；(2) 对于某些（some）数字对（pairs of numbers） x 和 y，有 x+y=1。

第二类陈述引发了对数对集合（the aggregate of pairs of numbers）的思考，这些数对通过某种固定关系联系在一起—在给定的例子中，通过关系 x+y=1 联系在一起。第一类公式的一个用途是，对于任意（any)一对数字都成立的公式，可以将第二类公式转换成无限多种等价形式。例如，关系 x+y=1 等价于以下关系：

y+x=1, (x-y)+2y=1, 6x+6y=6，等等。

因此，熟练的数学家会使用最方便于其当前目的的等价形式来考虑所讨论的关系。

一般来说，并不是所有的情况下，当一对项满足某一固定关系时，如果已知其中一项，那么另一个项也能够确定下来。例如，当 𝑥 和 𝑦 满足  $y^2 =x $  时，如果 𝑥=4，𝑦可以是  $\pm 2$，因此，对于任何正值的 𝑥，都存在多种可能的 𝑦 值。同样，在关系 $x+y>1$中，如果已知 x或 y中的一个，另一个项将存在无限多个可能的取值。

再次有另一个重要的观点需要注意。如果我们将自己限制在考虑关系$x+y=1$ 中的正数，无论是整数还是分数，那么，如果  $x$  或 $y$中的任意一个大于1，那么就没有正数可以使另一个数能够满足这个关系。因此， $x$ 的“范围”被限制在小于1的数字里， $y$的情况类似。再次，仅考虑整数（正数或负数），并取满足 $y^2=x$ 的数对。然后，无论 $y$被赋予任何整数值， $x$ 都可以假设一个对应的整数值。所以 $y$的“范围”在正整数或负整数中是不受限制的。但是 $x$ 的“范围”有两种限制。首先， $x$ 必须是正数，其次，由于  $y$ 必须是整数，所以  $x$  必须是一个完全平方数。因此， $x$ 的“范围”被限制在整数集 $1^2,2^2,3^2,4^2$，等等，即$1,4,9,16$，等等。

两个数对之间关系的一般属性的研究通过以下方式构建的图表大大地得到了简化:

![image-20240519231407121](https://typora-huang-cong.oss-cn-shanghai.aliyuncs.com/image-20240519231407121.png)

画两条相互垂直的直线$OX$ 和 $OY$ ；让任意数 $x$ 通过 $OX$ 方向的 $x$ 个单位长度（在任意比例尺度下）表示，任意数 $y$ 通过 $OY$ 方向的 $y$ 个单位长度（在任意比例尺度下）表示。因此，如果 $OM$ 在$OX$上的长度为 $x$ 个单位，$ON$在 $OY$ 上的长度为 $y$ 个单位，通过完成平行四边形 $OMPN$ 我们找到了一个对应于数对 $x$ 和 $y$ 的点 $P$。对于每一个点，都有一个对应的数对，而对于每一个数对，都有一个对应的点。这个数对被称为点的坐标。那些坐标满足某个固定关系的点可以通过方便的方式指示出来，例如通过画一条线，如果它们都在一条直线上，或者通过给区域涂色，如果它们都是区域内的点。如果关系可以用方程表示，比如 $x+y=1$ 或 $y^2=x$，那么这些点都位于一条直线上，在前一种情况下是直线，在后一种情况下是曲线。例如，仅考虑正数时，满足 $x+y=1$ 的坐标点位于图1中的直线 $AB$ 上，其中 $OA=1$ 且 $OB=1$。因此，直线段 $AB$ 提供了关系在限制为正数时的图像表现。

另一个关于两个变量之间关系的例子是，通过考虑一定质量的某种气体物质（如空气、煤气或蒸汽）在恒定温度下的压力和体积的变化来提供的。设$v$ 为其体积的立方英尺数，$p$ 为其压力，以每平方英寸磅数（psi）表示。然后，表达 $p$ 和$v$ 之间关系的定律，即波义耳定律，是说 $pv$ 的乘积是恒定的，前提是温度不变。让我们假设，例如，气体的量及其其他情况是这样的：我们可以设 $pv=I$（方程右侧的具体数值没有本质的区别）。

<img src="https://typora-huang-cong.oss-cn-shanghai.aliyuncs.com/image-20240520224818131.png" alt="image-20240520224818131" style="zoom: 67%;" />

然后在图2中，我们取两条线，$OV$ 和 $OP$ ，垂直交叉，并沿 $OV$ 画出 $OM$ 代表 $v$ 个体积单位，沿 $OP$ 画出 $ON$ 代表 $p$ 个压力单位。然后，通过完成平行四边形 $OMQN$ 找到的点 $Q$ 表示了当气体体积为 $v$ 立方英尺，压力为每平方英寸 $p$ 磅时的气体状态。如果考虑到被分析气体部分的情况是 $pv=I$，那么所有这些点 $Q$，对应于该部分气体的任何可能状态，必须位于曲线 $ABC$ 上，该曲线包括所有 $p$ 和 $v$ 为正且 $pv=I$ 的点。因此，这条曲线提供了体积和压力之间关系的形象表示。当压力很大时，相应的点 $Q$ 必须接近 $C$，甚至在曲线未绘制部分之外；此时体积将非常小。当体积很大时，$Q$ 将接近 $A$ 或在 $A$ 之外；此时压力将很小。注意，工程师或物理学家可能想知道与某确定的体积对应的特定压力。那么，当 $v$ 是已知数时，我们需要确定未知的 $p$。但这只是一个特定情况。在考虑气体的性质及其行为时，他必须心中有数整个曲线 $ABC$ 的一般形式及其一般特性。换句话说，真正基本的概念是满足关系式 $pv=I$ 的 变量对（ the pair of variables）的概念。这个例子说明了在数学的应用和理论中，变量（variables） 的概念是多么基础。


