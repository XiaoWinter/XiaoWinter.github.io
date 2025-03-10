---
title: chapter 14 Series
date: 2025-03-10 10:07:00
type: "tags"
tags:
  - math
categories: the introduction of mathematics
mathjax: true
---

# SERIES[级数]

No PART of Mathematics suffers more from the triviality of its initial presentation to beginners than the great subject of series. Two minor examples of series, namely arithmetic and geometric series, are considered; these examples are important because they are the simplest examples of an important general theory. But the general ideas are never disclosed and thus the examples, which exemplify noting, are reduced to silly trivialities.

没有哪部分数学比级数这一伟大课题更容易在向初学者介绍时显得琐碎。两个小的级数例子——即算术级数和几何级数——被考虑在内；这些例子之所以重要，是因为它们是一个重要一般理论的最简单例子。但是，普遍的理念从未被揭示出来，因此这些例子——本应展示重要内容——反而沦为无聊的琐事。

The general mathematical idea of a series is that of a set of things ranged in order, that is, in sequence. This meaning is accurately represented in the common use of the term. Consider, for example, the series of English Prime Ministers during the nineteenth century, arranged in the order of their first tenure of that office within the century. The series commences with Willian Pitt, and ends with Lord Rosebery, who, appropriately enough, is the biographer of the first member. We might have considered other serial orders for the arrangement of these men; for example, according to their height or their weight. These other suggested orders strike us as trivial in connexion with Prime Ministers, and would not naturally occur to the mind; but abstractly they are just as good orders as any other. When one order among terms is very much more important or more obvious that other orders, it is often spoken of as the order of those terms. Thus the order of the integers would always be taken to mean their order as arranged in order of magnitude. But of course there is an indefinite number of other ways of arranging them. When the number of things considered is finite, the number of ways of arranging them in order is called the number of their permutations. The number of permutations of a set of $n$ things, where $n$ is some finite integer, is 

级数的数学一般概念是指一组事物按顺序排列，即按顺序排列的序列。这个意义在该术语的常见用法中得到了准确的表达。例如，考虑19世纪英国首相的序列，按他们在世纪内首次担任该职务的顺序排列。这个序列从威廉·皮特开始，最终由罗斯伯里勋爵结束，恰如其分的是，他是皮特的传记作者。我们本可以考虑其他序列方式来安排这些人物；例如，根据他们的身高或体重来排序。与首相相关的这些其他建议的排序方式在我们看来显得琐碎，而且不太容易想到；但是抽象地说，它们与任何其他排序方式一样合理。当某一排序在各个项之间比其他排序更为重要或更明显时，人们常常将其称为这些项的“排序”。因此，整数的排序通常指它们按大小顺序排列的方式。但当然，还有无数其他方式来排列这些整数。当考虑的事物数量是有限的时，按顺序排列它们的方式的数量被称为它们的排列数。若一个集合包含$n$个事物，其中$n$是某个有限整数，那么这些事物的排列数是
$$
n \times (n-1) \times (n-2) \times (n-3)\times \dots \times4\times3\times2\times1
$$
that is to say, it is the product of the first $n$ integers; this product is so important in mathematics that a special symbolism is used for it, and it is always written '$n!$'. Thus, $2!=2\times1=2,$ and $3!=3\times2\times1=6$ , and $4!=4\times3\times2\times1=24$, and $5!=5\times4\times3\times2\times1=120$. As $n$ increases, the value of $n!$ increases very quickly; thus $100!$ is a hundred times as large as $99!$.

换句话说，它是前$n$个整数的积；这个积在数学中非常重要，以至于有一种特殊的符号表示它，并且总是写作$n!$。因此，$2! = 2 \times 1 = 2$，$3! = 3 \times 2 \times 1 = 6$，$4! = 4 \times 3 \times 2 \times 1 = 24$，$5! = 5 \times 4 \times 3 \times 2 \times 1 = 120$。随着$n$的增加，$n!$的值增加得非常快；例如，$100!$是$99!$的100倍。

It is easy to verify in the case of small values of $n$ that $n!$ is the number of ways of arranging $n$ things in order. Thus consider two things $a$ and $b$; these are capable of the two orders $ab$ and $ba$, and $2!=2$.

对于小的$n$值，可以很容易地验证$n!$是将$n$个事物按顺序排列的方式的数量。因此，考虑两个事物$a$和$b$；这两个事物可以有两种排列方式：$ab$和$ba$，因此$2! = 2$。

Again, take three things $a,b,$ and $c$; there are capable of the six orders, $abc,acb,bac,bca,cab,cba,$ and $3!=6$. Similarly for the twenty-for orders in which four things $a,b,c$ and $d,$ can be arranged.

再考虑三个事物$a$、$b$和$c$；它们可以有六种排列方式：$abc, acb, bac, bca, cab, cba$，因此$3! = 6$。类似地，对于四个事物$a$、$b$、$c$和$d$，它们可以有二十四种排列方式。

When we come to the infinite set of things —— like the sets of all the integers, or all the fractions, or all the real numbers for instance—— we come at once upon the complications of the theory of order-types. This subject was touched upon in Chapter 6 in considering the possible orders of the integers, and of the fractions, and of the real numbers. The whole question of order-types forms a comparatively new branch of mathematics of great importance. We shall not consider it any further. All the infinite series which we consider now are of the same order-type as the integers arranged in ascending order of magnitude, namely, with a first term, and such that each term has a couple of next-door neighbours, one on either side, with the exception of the first term which has, of course, only one next-door neighbour. Thus, if $m$ be any integer (not zero), there will be always an $m$th term. A sreies with a finite number of terms (say $n$ terms) has the same characteristics as far as next-door neighbours are concerned as an infinite series; it only differs from infinite series in having a last term, namely, the $n$th.

当我们谈到无限集合——比如所有整数、所有分数或所有实数的集合——我们立刻遇到序列类型理论的复杂性。这个话题在第六章中有所涉及，当时我们考虑了整数、分数和实数的可能排序。序列类型的整个问题构成了数学中的一个相对较新的、非常重要的分支。我们现在不再进一步讨论它。我们现在考虑的所有无限级数都与按大小升序排列的整数的序列属于同一种序列类型，即具有第一个项，并且每个项都有一对邻近项，分别位于两边，除了第一个项，它当然只有一个邻近项。因此，如果$m$是任何非零整数，那么总会有第$m$项。一个有限项数的级数（比如$n$项）在邻近项的关系上与无限级数相同；它与无限级数的唯一区别在于它有一个最后一项，即第$n$项。

The important thing to do with a series of numbers——using for the future 'series' in the restricted sense which has just been mentioned——is to add its successive terms together.

对一个数列来说——这里将“数列”一词用于刚才提到的狭义的定义——最重要的事情是将其连续的项相加。

Thus if $u_1,u_2,u_3,\dots,u_n,\dots,$ are respectively the 1st, 2nd, 3rd, 4th,...,nth,...,terms of a series of numbers, we form successively the series $u_1,u_1+u_2,u_1+u_2+u_3,u_1+u_2+u_3+u_4,$ and so on; thus the sum of the 1st $n$ terms may be written

因此，如果$u_1, u_2, u_3, \dots, u_n, \dots$分别是数列的第1项、第2项、第3项、第4项，...、第$n$项，...，我们依次形成数列$u_1, u_1 + u_2, u_1 + u_2 + u_3, u_1 + u_2 + u_3 + u_4,$等等；因此，第$n$项的和可以写作
$$
u_1+u_2+u_3+\dots+u.
$$
If the series has only a finite number of terms, we come at last in this way to the sum of the whole series of terms. But, if the series has an infinite number of terms, this process of successively forming the sums of the terms never terminates; and in this sense there is no such thing as the sum of an infinite series.

如果数列只有有限项，我们通过这种方式最终得到整个数列的和。但如果数列有无限项，这个依次形成各项和的过程永远不会结束；从这个意义上说，根本不存在无限级数的和。

But why is it important successively to add the terms of a series in this way? The answer is that we are here symbolizing the fundamental mental process of approximation. This is a process which has significance far beyond the regions of mathematics. Our limited intellects cannot deal with complicated material all at once, and our method of arrangement is that of approximation. The statesman in framing his speech puts the dominating issues first and lets the details fall naturally into their subordinate places. These is, of course, the converse artistic method of preparing the imagination by the presentation of subordinate or special details, and then gradually rising to a crisis. In either way the process is one of gradual summation of effects; and this is exactly what is done by the successive summation of the terms of a series. Our ordinary method of stating numbers is such a process of gradual summation, at least, in the case of large numbers. Thus 568,213 presents itself to the mind as ——

但为什么要以这种方式依次加总数列的各项呢？答案是，我们在这里象征性地表示了近似的基本心理过程。这是一个具有深远意义的过程，远远超出了数学的范畴。我们的智力有限，无法一次性处理复杂的材料，我们的安排方法就是近似法。政治家在起草演讲时把主要问题放在前面，让细节自然而然地归位。当然，也有相反的艺术方法，即通过呈现从属或特殊的细节来逐步引导想象力，最后达到一个高潮。不管是哪种方式，这个过程都是逐步累积效果的过程；这正是通过依次加总数列的各项所完成的。我们日常表示数字的方法也可以看作是一个逐步累积的过程，至少在处理大数字时是如此。因此，568,213 在脑海中呈现出来的是 ——
$$
500,000+60,000+8,000+200+10+3
$$
In the case of decimal fractions this is so more avowedly. Thus 3.14159 is ——

在十进制小数的情况下，这一点更加明显。因此，$3.14159$是 ——
$$
3+\frac{1}{10}+\frac{4}{100}+\frac{1}{1000}+\frac{5}{10000}+\frac{9}{100000}
$$
Also, 3 and $3+\frac{1}{10},$ and $3+\frac{1}{10}+\frac{4}{100},$ and $3+\frac{1}{10}+\frac{4}{100}+\frac{1}{1000},$and $3+\frac{1}{10}+\frac{4}{100}+\frac{1}{1000}+\frac{5}{10000}$ are successive approximations to the complete result 3.14159. If we read 568,213 backwards from right to left, starting with the $3$ units, we read it in the artistic way, gradually preparing the mind for the crisis of 500,000.

同样，$3$ 和 $3 + \frac{1}{10}$，$3 + \frac{1}{10} + \frac{4}{100}$，$3 + \frac{1}{10} + \frac{4}{100} + \frac{1}{1000}$，以及 $3 + \frac{1}{10} + \frac{4}{100} + \frac{1}{1000} + \frac{5}{10000}$ 是对完整结果 3.14159 的逐步近似。如果我们从右到左反向读取 568,213，从$3$的单位开始，我们以艺术的方式读取它，逐步为 500,000 的危机做准备。

The ordinary process of numerical multiplication proceeds by means of the summation of a series. Consider the computation

数字乘法的普通过程是通过加总一个数列来进行的。考虑以下计算
$$
342 \\ 
658 \\
{\rule{2cm}{0.3pt}} \\
2736 \\ 
1710 \\
2052 \\
{\rule{2cm}{0.3pt}}\\
225036
$$
Hence the three lines to be added form a series of which the first term is the upper line. The series follows the artistic method of presenting the most important term last, not from any feeling for art, but because of the convenience gained by keeping a firm hold on the units' place, thus enabling us to omit some 0's, formally necessary.

因此，要添加的三条线形成一个序列，其中第一个项是上边的线。这个序列遵循了艺术表达方法，即将最重要的项放在最后，而不是出于对艺术的感受，而是因为通过牢牢把握单位位置所获得的便利，从而使我们能够省略一些形式上必要的零。

But when we approximate by gradually adding the successive terms of an infinite series, what are we approximating to? The difficulty is that the series has no 'sum' in the straightforward sense of the word, because the operation of adding together its terms can never be completed. The answer is that we are approximating to the $limit$ of the summation of the series, and we must now proceed to explain what the 'limit' of a series is.

但是，当我们通过逐步添加一个无穷级数的连续项来进行近似时，我们到底是在近似什么呢？问题在于，这个级数并没有一个“和”，按照这个词的直白意思，因为将它的各项加在一起的操作永远无法完成。答案是，我们是在接近级数求和的**极限**，接下来我们必须解释什么是级数的“极限”。

The summation of a series approximates to a limit when the sum of any number of its terms, provided the number large enough, is as nearly equal to the limit as you care to approach. But this description of the meaning of approximating to a limit evidently will not stand the vigorous scrutiny of modern mathematics. What is meant by *large enough,* and by *nearly equal,* and by *care to approach*? All these vague phases must be explained in terms of the simple abstract ideas which alone are admitted into pure mathematics.

当一个数列的求和接近某个极限时，如果该数列中任意数量的项的和（前提是项数足够大）与该极限的差距小到你愿意接近的程度，就可以说该求和接近极限。但这种对“接近极限”意义的描述显然无法经得起现代数学的严格审视。那么，“足够大”是什么意思？“几乎等于”是什么意思？“愿意接近”又是什么意思？所有这些模糊的表述必须用纯数学中所承认的简单抽象概念来加以解释。

Let the successive terms of the series be $u_1,u_2,u_3,u_4,...,u_n,\&c.$, so that $u_n$ is the $nth$ term of the series. Also let $s_n$ be the sum of the $1st$ $n$ terms, whatever $n$ may be. So that ——

让数列的连续项分别为 $u_1, u_2, u_3, u_4, \dots, u_n, \dots$，其中 $u_n$ 是数列的第 $n$ 项。又设 $s_n$ 为前 $n$ 项的和，无论 $n$ 取什么值。所以——
$$
s_1=u_1,s_2=u_1+u_2,s_3=u_1+u_2+u_3, and \\
s_n=u_1+u_2+u_3+...+u_n.
$$
 Then the term $s_1,s_2,s_3,...s_n,...$ form a new series, and the formation of this series is the process of summation of the original series. Then the 'approximation' of the $summation$ of the original series to a 'limit' means the 'approximation of the terms of this new series to a limit'. And we have now to explain what we mean by the approximation to a limit of the terms of a series.

然后，项 $s_1, s_2, s_3, \dots, s_n, \dots$ 形成一个新的数列，这个数列的形成过程就是原始数列求和的过程。那么，原始数列的“求和”逼近一个“极限”，意味着这个新数列的各项逼近一个极限。接下来，我们需要解释什么是数列各项逼近极限的意思。

Now, remembering the definition (given in Chapter 11) of a $standard \space  of \space approximation$, the idea of a limit means this: $l$ is the limit of the terms of the series $s_1,s_2,s_3...,s_n,...,$ if , corresponding to each real number $k$ , taken as a standard of approximation, a term $s_n$ of the series can be found so that all succeeding terms (i.e. $s_{n+1},s_{n+2},\&c.$) approximate to $l$ within that standard of approximation. If another smaller standard $k^1$ be chosen, the term $s_{n}$ may be too early in the series, and a later term $s_m$ with the above property will then be found.

现在，回忆一下（在第11章中给出的）“逼近标准”的定义，极限的概念是这样的：如果对于每一个实数 $k$，作为逼近标准，都能找到数列 $s_1, s_2, s_3, \dots, s_n, \dots$ 中的某项 $s_n$，使得所有后续的项（即 $s_{n+1}, s_{n+2}, \dots$）都能在该逼近标准内逼近 $l$，那么 $l$ 就是数列的极限。如果选择另一个更小的标准 $k^1$，那么 $s_n$ 可能在数列中出现得过早，此时会找到一个更晚的项 $s_m$，它满足上述的性质。

If this property holds, it is evident that as you go along to series $s_1,s_2,s_3,...,s_n,...,$ from left to right, after a time you come to terms $all \space of $ which are nearer to $l$ than any number which you may like to assign.  In other words you approximate to $l$ as closely as you like. The close connextion of this definition of the limit of a series with the definition of a continuous function given in Chapter 11 will be immediately perceived.

如果这个性质成立，那么显然，当你从左到右遍历数列 $s_1, s_2, s_3, \dots, s_n, \dots$ 时，经过一段时间后，你会遇到所有的项，这些项都比你可能选定的任何数字都更接近 $l$。换句话说，你可以任意精确地逼近 $l$。这一数列极限的定义与第11章中给出的连续函数定义有着紧密的联系，读者会立即察觉到这一点。

Then coming back to the original series $u_1,u_2,u_3,...,u_n,$ the limit of the terms of the series $s_1,s_2,s_3,...,s_n,...,$ is called the 'sum to infinity' of the original series. But it is evident that this use of the word 'sum' is very artificial, and we must not assume the analogous properties to those of the ordinary sum of a finite number of terms without some special investigation.

回到原始数列 $u_1, u_2, u_3, \dots, u_n, \dots$，数列 $s_1, s_2, s_3, \dots, s_n, \dots$ 的极限被称为原始数列的“无穷和”。但是显然，这里使用“和”这个词是非常人工的，我们不能假设它具备与有限项的普通和相同的性质，而不经过一些特殊的研究。

Let us look at an example of a 'sum to infinity'. Consider the recurring decimal $0.1111...$ This decimal is merely a way of symbolizing the 'sum to infinity' of the series $0.1,0.01,0.001,0.0001,\&c$. The corresponding series found by summation is $s_1=0.1,s_2=0.11,s_3=0.111,s_4=0.1111,\&c.$ The limit of the terms of this series is $\frac{1}{9}$; this is easy to see by simple division, for 

让我们来看一个“无穷和”的例子。考虑循环小数 $0.1111...$。这个小数仅仅是表示数列 $0.1, 0.01, 0.001, 0.0001, \dots$ 的“无穷和”。通过求和得到的对应数列是 $s_1 = 0.1, s_2 = 0.11, s_3 = 0.111, s_4 = 0.1111, \dots$。这个数列的极限是 $\frac{1}{9}$；通过简单的除法就能容易看出这一点，因为
$$
\frac{1}{9}=0.1+\frac{1}{90}=0.11+\frac{1}{900}=0.111+\frac{1}{9000}=\&c.
$$
Hence, if $\frac{3}{17}$ is given (the $k$ of the definition), $0.1$ and *all* succeeding terms differ from $\frac{1}{9}$ by less than $\frac{3}{17}$; if $\frac{1}{1000}$ is given (another choice for the $k$ of the definition), $0.111$ and all succeeding terms differ from $\frac{1}{9}$ by less than $\frac{1}{1000}$; and so on, whatever choice for $k$ be made.

因此，如果给定 $\frac{3}{17}$（即定义中的 $k$），那么 $0.1$ 以及 *所有* 后续项与 $\frac{1}{9}$ 的差异小于 $\frac{3}{17}$；如果给定 $\frac{1}{1000}$（另一个 $k$ 的选择），那么 $0.111$ 以及所有后续项与 $\frac{1}{9}$ 的差异小于 $\frac{1}{1000}$；无论选择什么 $k$，都可以这样进行。

It is evident that nothing that has been said gives the slightest idea as to how the 'sum to infinity' of a series is intrinsically out of the question, for the simple reason that such a 'sum', as here defined, does not always exist. Series which possess a sum to infinity are called $convergent$, and those which do not possess a sum to infinity are called $divergent$.

显然，迄今为止所说的任何内容都没有提供丝毫关于为什么数列的“无穷和”本质上是不可能的想法，原因很简单：根据这里的定义，这样的“和”并不总是存在。拥有无穷和的数列称为**收敛**数列，而没有无穷和的数列称为**发散**数列。

An obvious example of a divergent series is $1,2,3,...,n,...,i.e.$ the series of integers in their order of magnitude. For whatever number $l$ you try to take as its sum to infinity, and whatever standard of approximation $k$ you choose, by taking enough terms of the series you can always make their sum differ from $l$ by more than $k$. Again, another example of a divergent series is $1,1,1,\&c.,i.e.$ the series of which each term is equal to $1$. Then the sum of $n$ terms is $n$, and this sum grows without limit as $n$ increases. Again, another example of a divergent series is $1,-1,1,-1,1,-1,\&c.,i.e$ the series in which the terms are alternately $1$ and $-1$. The sum of an odd number of terms is $1$, and of an even number of terms is $0$. Hence the terms of the series $s_1,s_2,s_3,...,s_n,...,$ do not approximate to a limit, although they do not increase without limit.

一个明显的发散数列的例子是 $1, 2, 3, \dots, n, \dots$，即按大小顺序排列的整数数列。无论你尝试将哪个数 $l$ 作为它的无穷和，且无论你选择什么样的逼近标准 $k$，只要取足够多的项，你总能使它们的和与 $l$ 的差距超过 $k$。另一个发散数列的例子是 $1, 1, 1, \dots$，即每项都等于 $1$ 的数列。那么，前 $n$ 项的和是 $n$，随着 $n$ 的增大，这个和是无限增长的。再举一个发散数列的例子是 $1, -1, 1, -1, 1, -1, \dots$，即项交替为 $1$ 和 $-1$ 的数列。奇数项的和是 $1$，偶数项的和是 $0$。因此，数列 $s_1, s_2, s_3, \dots, s_n, \dots$ 的项虽然不会无限增大，但它们并没有逼近某个极限。

It is tempting to suppose that the condition for $u_1,u_2,...,u_n,...,$ to have a sum to infinity is that $u_n$ should decrease indefinitely as $n$ increases. Mathematics would be a much easier science than it is, if this were the case. Unfortunately the supposition is not true.

人们可能会倾向于认为，数列 $u_1, u_2, \dots, u_n, \dots$ 存在无穷和的条件是 $u_n$ 随着 $n$ 增大而无限减小。如果真是这样，数学将比现在容易得多。不幸的是，这个假设并不成立。

For example, the series

例如，数列
$$
1,\frac{1}{2},\frac{1}{3},\frac{1}{4},...,\frac{1}{n},...
$$
is divergent. It is easy to see that this is the case; for consider the sum of $n$ terms beginning at the $(n+1)^{th}$ term. These $n$ terms are $\frac{1}{n+1},\frac{1}{n+2},\frac{1}{n+3},...,\frac{1}{2n}$: there are $n$ of them and $\frac{1}{2n}$ is the least among them. Hence their sum is greater than $n$ times $\frac{1}{2n},i.e.$ 

is greater than $\frac{1}{2}$. Now, without altering the sum to infinity, if it exists, we can add together neighbouring terms, and obtain the series

是发散的。很容易看出这是正确的；因为考虑从第 $(n+1)^{th}$ 项开始的 $n$ 项的和。这 $n$ 项是 $\frac{1}{n+1}, \frac{1}{n+2}, \frac{1}{n+3}, \dots, \frac{1}{2n}$：它们共有 $n$ 项，而 $\frac{1}{2n}$ 是其中最小的一项。因此，它们的和大于 $n$ 倍的 $\frac{1}{2n}$，即大于 $\frac{1}{2}$。现在，在不改变无穷和的情况下（如果它存在的话），我们可以将相邻的项相加，得到数列
$$
1,\frac{1}{2},\frac{1}{3}+\frac{1}{4},\frac{1}{5}+\frac{1}{6}+\frac{1}{7}+\frac{1}{8},\&c.
$$
that is , by what has been said above, a series whose terms after the 2nd are greater than those of the series,

也就是说，根据上述所说，得到的数列，其第二项之后的各项大于原数列的各项。
$$
1,\frac{1}{2},\frac{1}{2},\frac{1}{2},\&c.,
$$
where all the terms after the first are equal. But this series is divergent. Hence the original series is divergent$^1$.

其中，所有第一项之后的项都相等。但这个数列是发散的。因此，原始数列也是发散的。

The question of divergency shows how careful we must be in arguing from the properties of the sum of a finite number of terms to that of the sum of an infinite series. For the most elementary property of a finite number of terms is that of course they possess a sum: but even this fundamental property is not necessarily possessed by an infinite series. This caution merely states that we must not be misled by the suggestion of the technical term 'sum of an infinite series'. It is usual to indicate the sum of the infinite series.

发散性的问题表明，我们在从有限项和的性质推论到无限级数和的性质时必须非常小心。因为有限项的最基本性质当然是它们具有和：但即使这个基本性质，无限级数也不一定具备。这个警告仅仅是指出，我们不能被“无穷级数和”这一技术术语的表象所误导。通常会表示无限级数的和。
$$
u_1,u_2,u_3,...,u_n,...,by \\
u_1+u_2+u_3+...+u_n+...
$$
We now pass on to a generalization of the idea of a series , which mathematics, true to its method, makes by use of the variable. Hitherto, we have only contemplated series in which each definite term was definite number. But equally well we can generalize, and make each term to be some mathematical expression containing a variable $x$. Thus we may consider the series $1,x,x^2,x^3,...,x^n,...,$ and the series

我们现在转向数列概念的一个概括，数学通过使用变量，忠实于其方法，做出了这一概括。迄今为止，我们只考虑了每一项都是确定数值的数列。但我们同样可以进行概括，使得每一项成为包含变量 $x$ 的某个数学表达式。因此，我们可以考虑数列 $1, x, x^2, x^3, \dots, x^n, \dots$，以及这个数列
$$
x,\frac{x^2}{2},\frac{x^3}{3},...,\frac{x^n}{n},...
$$
In order to symbolize the general idea of any such function conceive of a function of $x,f_n(x)$ say, which involves in its formation a variable integer $n$, then, by giving $n$ the values $1,2,3,\&c.,$ in succession, we get the series

为了象征任何此类函数的一般概念，可以设想一个函数 $f_n(x)$，其中涉及一个变量整数 $n$，然后，通过依次赋予 $n$ 值 $1, 2, 3, \dots$，我们得到数列。
$$
f_1(x),f_2(x),f_3(x),...,f_n(x),...
$$
Such a series may be convergent for some values of $x$ and divergent for others, It is , in fact , rather rare to find a series involving a variable $x$ which is convergent for all values of $x$ ,——at least in any particular instance it is very unsafe to assume that this is the case. For example, let us examine the simplest of all instances, namely, the 'geometrical' series.

这样的数列对于某些 xx 的值可能是收敛的，而对于其他值则是发散的。事实上，找到一个对于所有 xx 值都收敛的数列是相当罕见的——至少在任何特定的实例中，假设这是成立的都是非常不安全的。例如，让我们来研究最简单的一个例子，即“几何”级数。
$$
1,x,x^2,x^3,...,x^n,...,
$$
The sum of $n$ terms is given by
$$
s_n=1+x+x^2+x^3+...+x^n.
$$
Now multiply both sides by $x$ and we get
$$
xs_n=x+x^2+x^3+x^4...+x^n+x^{n+1}.
$$
Now substract the last line form the upper line and we get
$$
s_n(1-x)=s_n-xs_n=1-x^{n+1},
$$
and hence (if $x$ be not equal to $1$)
$$
s_n=\frac{1-x^{n+1}}{1-x}=\frac{1}{1-x}-\frac{x^{n+1}}{1-x}.
$$
Now if $x$ be numerically less than 1, for sufficiently large values of $n$, $\frac{x^{n+1}}{1-x}$ is always numerically less than $k$ ,however $k$ be chosen. Thus, if $x$ be numerically less than 1, the series $1,x,x^2,x^3,...,x^n,...,$ is convergent, and $\frac{1}{1-x}$ is its limit. This statement is symbolized by

现在，如果 $x$ 的绝对值小于 1，对于足够大的 $n$ 值，$\frac{x^{n+1}}{1-x}$ 的绝对值总是小于某个常数 $k$，无论 $k$ 取什么值。因此，如果 $x$ 的绝对值小于 1，数列 $1, x, x^2, x^3, \dots, x^n, \dots$ 是收敛的，并且 $\frac{1}{1-x}$ 是它的极限。这个结论用符号表示为


$$
\frac{1}{1-x}=1+x+x^2+x^3+...+x^n+...,(-1<x<1).
$$
But if $x$ is numerically greater than 1, or numerically equal to 1, the series is divergent. In other words, if $x$ lie between $-1$ and $1$ , the series is convergent; but if $x$ be equal to $-1$ or $+1$ , or if $x$ lie outside the interval $-1$ to $+1$ , then the series is divergent. Thus the series is convergent at all 'points' within the interval $-1$ to $+1$ , exclusive of the end points.

但是，如果 $x$ 的绝对值大于 1，或者 $x$ 的绝对值等于 1，则该数列是发散的。换句话说，如果 $x$ 位于 $-1$ 和 $1$ 之间，则该数列是收敛的；但如果 $x$ 等于 $-1$ 或 $+1$，或者 $x$ 位于区间 $-1$ 到 $+1$ 之外，则该数列是发散的。因此，该数列在区间 $-1$ 到 $+1$ 内的所有“点”处收敛，但不包括端点。

At this stage of our inquiry another question arise. Suppose that the series

在我们探讨的这个阶段，又出现了一个问题。假设级数
$$
f_1(x)+f_2(x)+f_3(x)+...+f_n(x)+...
$$
is convergent for all values of $x$ lying within the interval $a$ to $b$, i.e. the series is convergent for any value of $x$ which is greater than $a$ and less than $b$. Also, suppose we want to be sure that in approximating to the limit we add together enough terms to come within some standard of approximation $k$. Can we always state some number of terms, say $n$, such that, if we take $n$ or more terms to form the sum, then *whatever* value $x$ has within the interval we have satisfied the desired standard of approximation?

对于所有位于区间 $a$ 到 $b$ 内的 $x$ 值是收敛的，即对于任意一个大于 $a$ 且小于 $b$ 的 $x$ 值，级数都是收敛的。并且，假设我们希望确保在逼近极限时，所加的项数足够，使得它符合某个标准的逼近误差 $k$。我们能否始终给出一个项数，比如 $n$，使得如果我们取 $n$ 或更多项来求和，那么无论区间内的 $x$ 值是什么，都能满足所需的逼近标准？

Sometimes we can and sometimes we cannot do this for each value of $k$. When we can, the series is called uniformly convergent throughout the interval, and when we cannot do so, the series is called non-uniformly convergent throughout the interval. It makes a great difference to the properties of a series whether it is or is not uniformly convergent through an interval. Let us illustrate the matter by the simplest example and the simplest numbers.

有时我们可以做到，有时我们不能做到这一点，对于每个 $k$ 值。当我们可以做到时，称该级数在整个区间上是均匀收敛的；而当我们不能做到时，称该级数在整个区间上是非均匀收敛的。级数是否在一个区间内均匀收敛，对该级数的性质有很大的影响。让我们通过最简单的例子和最简单的数字来说明这个问题。

Consider the geometric series

考虑几何级数
$$
1+x+x^2+x^3+...+x^n+...
$$
It is convergent throughout the interval $-1$ to $+1$ , excluding the end values $x=\pm1$.

But it is not uniformly convergent throughout this interval. For if $s_n(x)$ be the sum of $n$ terms, we have proved that the difference between $s_n(x)$ and the limit  $\frac{1}{1-x} $ is $ \frac{x^{n+1}}{1-x}$ . Now suppose $n$ be any given number of terms, say 20, and let $k$ be any assigned standard of approximation, say $0.001$. Then , by taking $x$ near enough to $+1$ or near enough to $-1$, we can make the numerical value of $\frac{x^21}{1-x}$ to be greater than $0.001$. Thus 20 terms will not do over the whole interval, though it is more than enough over some parts of it. 

它在区间 $-1$ 到 $+1$ 上是收敛的，但不包括端点值 $x = \pm 1$。

然而，它在整个区间内并不是均匀收敛的。因为如果 $s_n(x)$ 是前 $n$ 项的和，我们已经证明，$s_n(x)$ 和极限 $\frac{1}{1-x}$ 之间的差是 $ \frac{x^{n+1}}{1-x}$。现在，假设 $n$ 是任何给定的项数，比如 20，并且设 $k$ 是任何指定的近似标准，比如 $0.001$。然后，通过取 $x$ 足够接近 $+1$ 或 $-1$，我们可以使得 $ \frac{x^{21}}{1-x}$ 的数值大于 $0.001$。因此，20 项不能在整个区间上有效，尽管它在某些部分足够使用。

The same reasoning can be applied whatever other number we take instead of 20, and whatever standard of approximation instead of $0.001$. Hence the geometric series $1+x+x^2+x^3+...+x^n+...$ is non-uniformly convergent over its *whole* interval of convergence $-1$ to $+1$. But if we take any smaller interval lying at both ends within the interval $-1$ to $+1$, the geometrical series if uniformly convergent within it, For example, take the interval $0$ to $+\frac{1}{10}$. Then any value for $n$ which makes $ \frac{x^{n+1}}{1-x}$ numerically less than $k$ at these limits for $x$ also serves for all values of $x$ between these limits, since it so happens that $ \frac{x^{n+1}}{1-x}$ diminishes in numerical value as $x$ diminishes in numerical value. For example, take $k=0.001$; then , putting $x=\frac{1}{10},$ we find:

相同的推理可以应用于我们取任何其他数字代替20，并且代替$0.001$的近似标准也是如此。因此，几何级数 $1+x+x^2+x^3+...+x^n+...$ 在其*整个*收敛区间 $-1$ 到 $+1$ 上是非均匀收敛的。但是，如果我们取一个位于区间 $-1$ 到 $+1$ 内部的较小区间，那么几何级数在该区间内是均匀收敛的。例如，取区间 $0$ 到 $+\frac{1}{10}$。然后，对于任何使得 $ \frac{x^{n+1}}{1-x}$ 在这些区间的端点处的数值小于$k$的$n$，它同样适用于这些端点之间的所有$x$值，因为恰好是 $ \frac{x^{n+1}}{1-x}$ 随着$x$数值的减小而减小。例如，取$k=0.001$；然后，代入$x=\frac{1}{10}$，我们得到：
$$
for,n=1, \frac{x^{n+1}}{1-x}=\frac{(\frac{1}{10})^2}{1-\frac{1}{10}}=\frac{1}{90}=0.111...,\\
for,n=2, \frac{x^{n+1}}{1-x}=\frac{(\frac{1}{10})^3}{1-\frac{1}{10}}=\frac{1}{900}=0.0111...,\\
for,n=1, \frac{x^{n+1}}{1-x}=\frac{(\frac{1}{10})^4}{1-\frac{1}{10}}=\frac{1}{9000}=0.00111...,
$$
Thus three terms will do for the whole interval, though, of course, for some parts of the interval it is more than is necessary. Notice that, because

因此，三个项就足够覆盖整个区间，尽管当然在区间的某些部分，它的项数多于所需的数量。注意，由于


$$
1+x+x^2+x^3+...+x^n+...
$$


is convergent (though not uniformly) throughout the interval $-1$ to $+1$, for each value of $x$ in the interval some number of terms $n$ can be found which will satisfy a desired standard of approximation; but, as we take $x$ nearer and nearer to either end value $+1$ or $-1$, larger and larger values of $n$ have to be employed.

在区间 $-1$ 到 $+1$ 上是收敛的（尽管不是均匀收敛的），对于区间内的每个 $x$ 值，都可以找到一个项数 $n$，使其满足所需的近似标准；但是，随着我们将 $x$ 越来越接近任一端点值 $+1$ 或 $-1$，必须使用越来越大的 $n$ 值。

It is curious that this important distinction between uniform and non-uniform convergence was not published till 1847 by Stokes——afterwards, Sir George Stokes——and later, independently in 1850 by Seidel, a German mathematician.

有趣的是，均匀收敛和非均匀收敛之间这个重要的区别直到1847年才由Stokes（后来的乔治·斯托克斯爵士）发布，随后在1850年，德国数学家赛德尔（Seidel）独立地也做出了类似的研究。

The critical points, where non-uniform convergence comes in, are not necessarily at the limits of the interval throughout which convergence holds. This is a speciality belonging to the geometrical series.

非均匀收敛出现的临界点不一定位于收敛区间的端点。这是几何级数的一个特殊性质。

In the case of the geometric series $1+x+x^2+x^3+...+x^n+...$, a simple algebraic expression $\frac{1}{1-x}$ can be given for its limit in its interval of convergence. But this is not always the case. Often we can prove a series to be convergent within a certain interval, though we know nothing more about its limit except that it is the limit of the series. But this is a very good way of defining a function; viz. as the limit of an infinite convergent series, and is , in fact, the way in which most functions are, or ought to be, defined.

在几何级数 $1+x+x^2+x^3+...+x^n+...$ 的情况下，我们可以给出一个简单的代数表达式 $\frac{1}{1-x}$ 作为其在收敛区间内的极限。但情况并非总是如此。我们通常可以证明一个级数在某个区间内是收敛的，尽管我们对其极限一无所知，除了它是该级数的极限。但这其实是一种非常好的函数定义方式；即将其定义为一个无限收敛级数的极限，实际上，这也是大多数函数的定义方式，或者说应该是它们的定义方式。

Thus, the most important series in elementary analysis is 

因此，在初等分析中，最重要的级数是
$$
1+x+\frac{x^2}{2!}+\frac{x^3}{3!}+...+\frac{x^n}{n!}+...,
$$


Where $n!$ has the meaning defined earlier in this chapter. This series can be proved to be absolutely convergent for *all* values of $x$ , and to be uniformly convergent within any interval which we like to take. Hence it has all the comfortable mathematical properties which a series should have. It is called the exponential series. Denote its sum to infinity by exp$x$. Thus, by definition,

其中 $n!$ 的含义是本章前面定义的。这个级数可以证明对于 *所有* 的 $x$ 值是绝对收敛的，并且在我们选择的任何区间内都是均匀收敛的。因此，它具有一个级数应该具备的所有舒适的数学性质。它被称为指数级数。我们用 $\exp{x}$ 来表示它的和。于是，按照定义，
$$
\exp{x} =1+x+\frac{x^2}{2!}+\frac{x^3}{3!}+...+\frac{x^n}{n!}+...,
$$


expx is called the exponential function.

$\exp{x}$ 被称为指数函数。



It is fairly easy to prove, with a little knowledge of elementary mathematics, that

用一些初等数学知识，证明这一点是相当简单的，具体来说，
$$
(\exp{x})\times (\exp{y})=\exp{(x+y)}
$$


in other words that
$$
(\exp{x})\times (\exp{y})=1+(x+y)+\frac{(x+y)^2}{2!}+\frac{(x+y)^3}{3!}+...+\frac{(x+y)^n}{n!}+...,
$$
This property $(A)$ is an example of what is called an addition-theorem. When any function [say $f(x)$] has been defined, the first thing we do is to try to express $f(x+y)$ in terms of known functions of $x$ only, and know functions of $y$ only. If we can do so, the result is called an addition-theorem. Addition-theorems play a great part in mathematical analysis. Thus the addition-theorem for the sine is given by

这个性质 $(A)$ 是所谓的加法定理的一个例子。当一个函数（比如 $f(x)$）已经被定义时，我们做的第一件事就是尝试将 $f(x+y)$ 用仅与 $x$ 相关的已知函数和仅与 $y$ 相关的已知函数表示。如果我们能够做到这一点，那么这个结果就被称为加法定理。加法定理在数学分析中起着重要作用。比如，正弦函数的加法定理是
$$
sin(x+y)=sin\space x\space cos \space y+cos\space x\space sin \space y
$$
and for cosine by
$$
cos(x+y)=cos\space x\space cos \space y-sin\space x\space sin \space y
$$


As a matter of fact the best ways of defining sin $x$ and cos $x$ are not by the elaborate geometrical methods of the previous chapter, but as the limits respectively of the series

实际上，定义 $\sin{x}$ 和 $\cos{x}$ 的最佳方法并不是通过上一章中的复杂几何方法，而是分别通过以下级数的极限来定义它们：
$$
x-\frac{x^3}{3!}+\frac{x^5}{5!}-\frac{x^7}{7!}+\&c....,
$$


and 
$$
1-\frac{x^2}{2!}+\frac{x^4}{4!}-\frac{x^6}{6!}+\&c....,
$$
so that we put 
$$
sin\space x=x-\frac{x^3}{3!}+\frac{x^5}{5!}-\frac{x^7}{7!}+\&c....,\\
cos\space x=1-\frac{x^2}{2!}+\frac{x^4}{4!}-\frac{x^6}{6!}+\&c....,
$$


These definitions are equivalent to the geometrical definitions, and both series can be proved to be convergent for all values of $x$ , and uniformly convergent throughout any interval. These series for sine and cosine have a general likeness to the exponential series given above. They are, indeed, intimately connected with it by means of the theory of imaginary numbers explained in Chapter 7 and 8.

这些定义与几何定义是等价的，并且这两个级数可以证明对于所有 $x$ 值都是收敛的，并且在任何区间内都是均匀收敛的。这些正弦和余弦的级数与上面给出的指数级数有着一般的相似性。实际上，它们通过第 7 章和第 8 章中解释的虚数理论与指数级数有着密切的联系。

![image-20250228001125028](https://typora-huang-cong.oss-cn-shanghai.aliyuncs.com/image-20250228001125028.png)

The graph of the exponential function is given in Fig.29. It cuts the axis $OY$ at the point $y=1$, as evidently it ought to do , since when $x=0$ every term of the series except the first is zero. The importance of the exponential function is that it represents any changing physical quantity whose rate of increase at any instant is a uniform percentage of its value at that instant. For example, the above graph represents the size at any time of a population with a uniform birth-rate, a uniform death-rate, and no emigration, where the $x$ corresponds to the time reckoned from any convenient day, and the $y$ represents the population to the proper scale. The scale must be such that $OA$ represents the population at the date which is taken as the origin. But we have here come upon the idea of 'rates of increase' which is the topic for the next chapter.

指数函数的图形如图29所示。它在 $OY$ 轴上与点 $y=1$ 相交，这显然是它应该达到的地方，因为当 $x=0$ 时，除了第一个项外，级数的所有项都是零。指数函数的重要性在于它表示任何物理量的变化，这种变化在任何时刻的增长率是其当前值的一个固定百分比。例如，上述图形表示的是在出生率、死亡率均匀且没有移民的情况下，人口在任何时刻的大小，其中 $x$ 对应从某个方便的日期起算的时间，$y$ 表示按适当比例缩放的人口数。这个比例必须使得 $OA$ 代表被取为原点的日期时的人口数。但我们在这里接触到了“增长率”的概念，这是下一章的主题。

![image-20250228001227518](https://typora-huang-cong.oss-cn-shanghai.aliyuncs.com/image-20250228001227518.png)

An important function nearly allied to the exponential function is found by putting——$x^2$ for $x$ as the argument in the exponential function. We thus get $exp(-x^2)$. the graph $y=exp(-x^2)$ is given in Fig.30.

与指数函数密切相关的一个重要函数是通过将 $x^2$ 代入指数函数中作为自变量得到的。这样我们得到 $\exp(-x^2)$。图30给出了图形 $y=\exp(-x^2)$。



The curve, which is something like a cocked hat, is called the curve of normal error. Its corresponding function is vitally important to the theory of statistics, and tells us in many cases the sort of deviations from the average results which we are to expect.

这条曲线看起来有点像一个倒置的三角帽，称为正态误差曲线。它对应的函数对统计学理论至关重要，并在许多情况下告诉我们应当预期的偏离平均值的偏差类型。

Another important function is found by combining the exponential function with the sine, in this way:

另一个重要的函数是通过将指数函数与正弦函数结合得到的，具体方式如下：
$$
y=\exp(-cx)\times sin \frac{2\pi x}{p}
$$
![image-20250228001200802](https://typora-huang-cong.oss-cn-shanghai.aliyuncs.com/image-20250228001200802.png)

Its graph is given in Fig.31. The point $A,B,O,C,D,E,F,$ are placed at equal intervals $\frac{1}{2}p$, and an unending series of them should be drawn forwards and backwards. This function represents the dying away of vibrations under the influence of friction or of 'damping' forces. Apart from the friction, the vibrations would be periodic, with a period $p$, but the influence of the friction makes the extent of each vibration smaller than that of the preceding by a constant percentage of that extent. This combination of the idea of 'periodicity' (which requires the since or cosine for its symbolism) and of 'constant percentage' (which requires the exponential function for its symbolism) is the reason for the form of this function, namely, its form as a product of a sine-function into an exponential function.

它的图形如图31所示。点 $A, B, O, C, D, E, F$ 被均匀地放置在间隔为 $\frac{1}{2}p$ 的位置，应该在前后绘制出无尽的这样的点序列。这个函数表示在摩擦力或“阻尼”力的作用下，振动的衰减。除了摩擦力，振动将是周期性的，周期为 $p$，但摩擦力的影响使得每次振动的幅度比前一次小，并且这个减少量是前一次幅度的一个恒定百分比。这个结合了“周期性”（它需要正弦或余弦作为符号）和“恒定百分比”（它需要指数函数作为符号）的概念，正是该函数形式的原因，也就是它作为正弦函数与指数函数的乘积形式。























 $^1$if a series with all its terms positive is convergent, the modified series found by making some terms positive and some negative according to any definite rule is also convergent. Each one of the set of series thus found, including the original series, is called 'absolutely convergent'. But it is possible for a series with terms partly positive and partly negative to be convergent, although the corresponding series with all its terms positive is divergent. For example, the series

$^1$ 如果一个所有项均为正数的数列是收敛的，那么通过按照某个明确规则将一些项变为正数、一些项变为负数所得到的修改后的数列也是收敛的。这样得到的每一个数列集合，包括原始数列，都被称为“绝对收敛”的数列。但是，对于一个部分为正、部分为负的数列，它可能是收敛的，尽管将其所有项变为正数后得到的数列是发散的。例如，数列
$$
1-\frac{1}{2}+\frac{1}{3}-\frac{1}{4}+\&c.
$$
is convergent though we have just proved that 

是收敛的，尽管我们刚刚证明了
$$
1+\frac{1}{2}+\frac{1}{3}+\frac{1}{4}+\&c.
$$
is divergent. Such convergent series, which are not absolutely convergent, are much more difficult to deal with than absolutely convergent series.

是发散的. 这种收敛的级数，不是绝对收敛的，比绝对收敛的级数要难处理得多。
