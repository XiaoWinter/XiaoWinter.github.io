---
title: chapter 8 Imaginary Numbers(continued)
date: 2024-11-28 00:08:00
type: "tags"
tags:
  - math
categories: an introduction to mathematics
mathjax: true
---


# IMAGINARY NUMBERS (*continued*)

THE DEFINITION of the multiplication of ordered couples is guided by exactly the same considerations as is that of their addition. The interpretation of multiplication must be such that

有序对的乘法定义完全遵循与其加法相同的原则。乘法的解释必须满足以下条件：
<!--more-->
($1 $) the result is another ordered couple,

($2 $) the operation is commutative, so that
$$
(x,y) \times (x',y') =  (x',y')\times(x,y)
$$
($3 $) the operation is associative, so that
$$
\left \{ (x,y) \times (x',y') \right \} \times (u,v)= (x,y) \times \left \{ (x',y') \times (u,v) \right \}
$$
($4 $) must make the result of division unique [ with an exception for the case of the zero couple (0,0)], so that when we seek to determine the unknown couple (x,y) so as to satisfy the equation

必须使得除法的结果唯一（零有序对 $(0,0)$ 的情况除外），这样当我们试图确定未知的有序对 $(x, y)$ 以满足方程时，结果是明确的。
$$
(x,y) \times (a,b) = (c,d)
$$
there is one and only one answer, which we can represent(表示) by 
$$
(x,y) = (c,d) {\div} (a,b), or \space by \space (x,y) = \frac{(c,d)}{(a,b)}.
$$
($5$) Furthermore the law involving both addition and multiplication, called the distributive law, must be satisfied, namely
$$
(x,y) \times \left \{ (a,b)+(c,d) \right \}=\left \{ (x,y) \times (a,b) \right \} + \left \{ (x,y) \times (c,d) \right \}.
$$
All these conditions ($1 $), ($2 $), ($3 $), ($4 $), ($5$) can be satisfied by an interpretation which , though it looks complicated at first, is capable of simple geometrical interpretation.

所有这些条件 ($1 $), ($2 $), ($3 $), ($4 $), ($5$)都可以通过一种解释来满足，尽管这种解释乍一看似乎复杂，但实际上可以用简单的几何学方法来解释。

By definition we put

根据定义，我们设定
$$
(x,y) \times (x',y') = \left \{ (xx'-yy'),(xy'+x'y) \right\}
$$

This is the definition of the meaning of the symbol $\times$ when it it written between two ordered couples. It follows evidently from this definition that the result of multiplication is another ordered couple, and that the value of the right-hand side of equation (A) is not altered by simultaneously interchanging x with x' and y with y'. Hence conditions ($1$) and ($2$) are evidently satisfied. The proof of that satisfaction of ($3$) , ($4$), ($5$) is equally easy when we have given the geometrical interpretation, which we will proceed to do in a moment. But before doing this it will be interesting to pause and see whether we have attained the object for which all this elaboration was initiated.

这是符号 $\times$ 在两个有序对之间书写时含义的定义。显然，根据这一定义，乘法的结果是另一个有序对，且通过同时将 $x$ 与 $x'$、$y$ 与 $y'$ 互换，方程 (A) 右侧的值不会发生变化。因此，条件 ($1$) 和 ($2$) 显然满足。当我们给出几何解释后，条件 ($3$)、($4$)、($5$) 的证明也同样容易。 但在此之前，暂停一下思考我们是否达到了这一精细构建的目标将是有趣的。

We came across equation of the form $x^2=-3$ , to which no solutions could be assigned in terms of positive and negative real numbers. We the found that all our difficulties would vanish if we could interpret the equation $x^2=-1$ , i.e. if we could so define $\sqrt{(-1)}$ that $\sqrt{(-1)} \times \sqrt{(-1)} = -1$ .

我们遇到了形如 $x^2 = -3$ 的方程，在正实数和负实数范围内无法为其赋予任何解。然后我们发现，如果能够解释方程 $x^2 = -1$，即如果我们能够定义 $\sqrt{(-1)}$ 使得 $\sqrt{(-1)} \times \sqrt{(-1)} = -1$，那么我们所有的难题将迎刃而解。

Now let us consider the three special ordered couples $(0,0),(1,0),$ and $(0,1)$.

现在让我们考虑三个特殊的有序对 (0,0),(1,0),(0,1)(0,0), (1,0), (0,1)(0,0),(1,0),(0,1)。

We have already proved that

我们已经证明了
$$
(x,y)+(0,0)=(x,y)
$$
For the future we follow the custom of omitting the $+$ sign wherever possible, thus (1,0) stands for (+1,0) and (0,1) for (0,+1).

对于将来，我们遵循惯例，在可能的情况下省略正号“$+$”，因此 $(1,0)$ 表示 $(+1,0)$，而 $(0,1)$ 表示 $(0,+1)$。

Furthermore we now have

此外，我们现在拥有
$$
(x,y) \times (0,0) = (0,0)
$$
Hence both for addition and for multiplication the couple (0,0) plays the part of zero in elementary arithmetic and algebra; compare the above equations with $x+0=x$, and $x\times 0 = 0$

因此，无论对于加法还是乘法，有序对 $(0,0)$ 都在基础算术和代数中起到了“零”的作用；将上面的等式与 $x+0=x$ 和 $x \times 0 = 0$ 进行比较。

Again consider $(1,0)$: this plays the part of 1 in elementary arithmetic and algebra. In these elementary sciences the special characteristic of 1 is that $x\times 1=x$, for all values of $x$ . Now by our law of multiplication

再来看有序对 $(1,0)$：它在基础算术和代数中起到了“1”的作用。在这些基础学科中，1 的特殊性质在于对所有 $x$ 值都有 $x \times 1 = x$。现在，根据我们的乘法法则
$$
(x,y)\times(1,0)=\left\{(x-0),(y+0)\right\}=(x,y)
$$
Thus (1,0) is the unit couple.

因此，$(1,0)$ 是单位有序对。

Finally consider (0,1): this will interpret for us the symbol $\sqrt{(-1)}$ . The symbol must therefore possess the characteristic property that $\sqrt{(-1)}\times\sqrt{(-1)}=-1$ .Now by the law of multiplication for ordered couples.

最后，我们来看有序对 $(0,1)$：它将为我们解释符号 $\sqrt{(-1)}$。因此，这个符号必须具备这样的特性，即 $\sqrt{(-1)} \times \sqrt{(-1)} = -1$。现在，根据有序对的乘法法则。
$$
(0,1)\times(0,1)=\left\{(0-1),(0+0)\right\}=(-1,0)
$$
But $(1,0)$ is the unit couple, and $(-1,0)$ is the negative unit couple; so that $(0,1)$ has the desired property. There are , however, two roots of -1 to be provided for , namely $\pm \sqrt{(-1)}$. Consider (0,-1); here again remembering that $(-1)^2=1$, we find, $(0,-1)\times(0,-1)=(-1,0)$ .

但是，$(1,0)$ 是单位有序对，$(-1,0)$ 是负单位有序对；因此，$(0,1)$ 具有所需的特性。然而，需要考虑到 $-1$ 有两个平方根，即 $\pm \sqrt{(-1)}$。考虑有序对 $(0,-1)$；在这里，同样记住 $(-1)^2=1$，我们可以得到 $(0,-1) \times (0,-1) = (-1,0)$。

Thus $(0,-1)$ is the other square root of $\sqrt{(-1)}$. Accordingly, the ordered couples $(0,1)$ and $(0,-1)$ are the interpretations of $\pm\sqrt{(-1)}$ in terms of ordered couples. But which corresponds to which? Does $(0,1)$ correspond to $+\sqrt{(-1)}$ and $(0,-1)$ to $-\sqrt{(-1)}$, or $(0,1)$ to $-\sqrt{(-1)}$, and $(0,1)$ to  $+\sqrt{(-1)}$? The answer is that it is perfectly indifferent which symbolism we adopt.

因此，$(0,-1)$ 是 $\sqrt{(-1)}$ 的另一个平方根。因此，有序对 $(0,1)$ 和 $(0,-1)$ 就是 $\pm\sqrt{(-1)}$ 在有序对中的解释。但是，哪个对应于哪个呢？是 $(0,1)$ 对应 $+\sqrt{(-1)}$，而 $(0,-1)$ 对应 $-\sqrt{(-1)}$，还是 $(0,1)$ 对应 $-\sqrt{(-1)}$，而 $(0,-1)$ 对应 $+\sqrt{(-1)}$？答案是，采用哪种符号体系完全无关紧要。

The ordered couples can be divided into three types, (1) the 'complex imaginary' type $(x,y)$, in which neither x nor y is zero; (2) the 'real' type $(x,0)$; (3) the 'pure imaginary' type $(0,y)$. Let us consider the relations of these types to each other. First multiple together the 'complex imaginary' couple $(x,y)$ and the 'real' type $(a,0)$ we find

有序偶对可以分为三种类型：(1) **复数虚数型** $(x, y)$，其中 $x$ 和 $y$ 都不为零；(2) **实数型** $(x, 0)$；(3) **纯虚数型** $(0, y)$。让我们来考虑这些类型彼此之间的关系。首先，将 **复数虚数型** $(x, y)$ 与 **实数型** $(a, 0)$ 相乘，我们得到
$$
(a,0) \times (x,y) = (ax,ay)
$$
 

Thus the effect is merely to multiply each term of the couple $(x,y)$ by the positive or negative real number a.

因此，其效果仅仅是将偶对 $(x, y)$ 的每一项乘以正或负的实数 $a$。

Secondly, multiply together the 'complex imaginary' couple $(x,y)$ and the 'pure imaginary' couple $(0,b)$ , we find
$$
(0,b)\times (x,y) = (-by,bx)
$$
Here the effect is more complicated, and is best comprehended in the geometrical interpretation to which we proceed after nothing three yet more special cases.

在这里，效果更为复杂，并且最好在我们记录了另外三个更特殊的情况之后，进入几何解释来理解它。

Thirdly, we multiply the 'real' couples (a,0) by the imaginary (o,b) and obtain
$$
(a,0) \times (0,b) = (0,ab)
$$


Fourthly we multiply the two 'real' couples (a,0) and (a',0) and obtain
$$
(a,0)\times(a',0)=(aa',0)
$$
Fifthly, we multiply the two 'imaginary couples' (0,b) and (0,b') and obtain
$$
(0,b) \times (0,b')=(-bb',0)
$$
We now turn to the geometrical interpretation, beginning first with some special cases. Take the couples (1,3) and (2,0) and consider the equation
$$
(2,0) \times (1,3) = (2,6)
$$


![image-20241110162010749](https://typora-huang-cong.oss-cn-shanghai.aliyuncs.com/image-20241110162010749.png)

In the diagram (Fig.11) the vector $OP$ represents $(1,3)$, and the vector $ON$ represents $(2,0)$, and the vector $OQ$ represents $(2,6)$. Thus the product $(2,0) \times (1,3)$ is found geometrically by taking the length of the vector $OQ$ to be the product of the length of the vector $OP$ and $ON$ , and (in this case ) by producing $OP$ to $Q$ to be of the required length. Again, consider the product $(0,2) \times (1,3)$ we have 

在图（图11）中，向量 $OP$ 表示 $(1,3)$，向量 $ON$ 表示 $(2,0)$，而向量 $OQ$ 表示 $(2,6)$。因此，乘积 $(2,0) \times (1,3)$ 从几何上可以通过将向量 $OQ$ 的长度视为向量 $OP$ 和 $ON$ 的长度之积来找到，并且（在这种情况下）通过将 $OP$ 延长到 $Q$ 使其达到所需的长度。同样，考虑乘积 $(0,2) \times (1,3)$，我们得到
$$
(0,2) \times (1,3) = (-6,2)
$$
The vector $ON_1$, corresponds to $(0,2)$ and the vector $OR$ to $(-6,2)$. Thus $OR$ which represents the new product is at right angles to $OQ$ and of the same length. Notice that we have the same law regulating the length of $OQ$ as in the previous case, namely, that its length is the product of the lengths of the two vectors which are multiplied together; but now that we have $ON_1$ along the 'ordinate' axis $OY$, instead of $ON$ along the 'abscissa' axis $OX$, the direction of $OP$ has been turned through a right-angle.

向量 $ON_1$ 对应于 $(0,2)$，向量 $OR$ 对应于 $(-6,2)$。因此，表示新乘积的向量 $OR$ 与 $OQ$ 成直角，并且长度相同。请注意，我们有相同的规则来调节 $OQ$ 的长度，就像之前的情况一样，即 $OQ$ 的长度是两个相乘向量的长度的乘积；但现在由于 $ON_1$ 位于 $OY$ 轴（“纵坐标”轴）上，而不是像之前的 $ON$ 位于 $OX$ 轴（“横坐标”轴）上，$OP$ 的方向已经旋转了一个直角。

Hitherto in these examples of multiplication we have looked on the vector $OP$ as modified by the vectors $ON$ and $ON_1$ . We shall get a clue to the general law of the direction by inverting the way of thought, and by thinking of the vectors $ON$ and $ON_1$ as modified by the vector $OP$. The law for the length of the product of the two vectors. The new direction for the enlarged $ON$ (i.e $OQ$) is found by rotating it in the (anti-clockwise) direction of rotation from $OX$ towards $OY$ through an angle equal to the angle $XOP$: it is an accident of this particular case that this rotation makes $OQ$ lie along the line $OP$. Again consider the product of $ON_1$ and $OP$; the new direction for the enlarged $ON_1$ (i.e. $OR$) is found by rotating $ON_1$ in the anti-clockwise direction of rotation through an angle equal to the angle $XOP$, namely, the angle $N_1OR$ is equal to the angle $XOP$.

至今为止，在这些乘法的示例中，我们一直将向量 $OP$ 视为被向量 $ON$ 和 $ON_1$ 所改变。通过反向思考，并将 $ON$ 和 $ON_1$ 视作被 $OP$ 所改变，我们可以得到关于方向普遍规律的一些线索。两个向量乘积的长度规律为：扩大后的 $ON$（即 $OQ$）的新方向，可以通过将其从 $OX$ 轴朝 $OY$ 轴逆时针旋转一个等于角 $XOP$ 的角度来得到。在这种特殊情况下，这种旋转使 $OQ$ 恰好位于 $OP$ 的延长线上，这只是一个偶然现象。再考虑 $ON_1$ 与 $OP$ 的乘积，扩大后的 $ON_1$（即 $OR$）的新方向可以通过将 $ON_1$ 逆时针旋转一个等于角 $XOP$ 的角度来得到，即角 $N_1OR$ 等于角 $XOP$。



The general rule for the geometrical representation of multiplication can now be enunciated thus:

用于几何表示乘法的一般法则现在可以这样表述:

The product of the two vectors $OP$ and $OQ$ is a vector $OR$, whose length is the product of the lengths of $OP$ and $OQ$ and whose direction $OR$ is such that the angle $XOR$ is equal to the sum of the angle $XOP$ and $XOQ$.

这两个向量 $OP$ 和 $OQ$ 的乘积是一个向量 $OR$，其长度是 $OP$ 和 $OQ$ 长度的乘积，并且 $OR$ 的方向使得角 $XOR$ 等于角 $XOP$ 和角 $XOQ$ 的和。

![image-20241110181054355](https://typora-huang-cong.oss-cn-shanghai.aliyuncs.com/image-20241110181054355.png)

Hence we can conceive the vector $OP$ as making the vector $OQ$ rotate through an angle $XOP$ (i.e. the angle $QOR$= the angle $XOP$), or the vector $OQ$ as making the vector $OP$ rotate through the angle $XOQ$ (i.e. the angle $POR$= the angle $XOQ$).

因此，我们可以将向量 $OP$ 想象为使向量 $OQ$ 旋转一个角度 $XOP$（即角 $QOR = XOP$），或者将向量 $OQ$ 想象为使向量 $OP$ 旋转角度 $XOQ$（即角 $POR = XOQ$）。

We do not prove this general law, as we should thereby be led into more technical processes of mathematics than falls within the design of this book. But now we can immediately see that the associative law [numbered ($3$) above] for multiplication is satisfied. Consider first the length of the resultant vector; this is got by the ordinary process of multiplication for real numbers; and thus the associative law holds for it.

我们不证明这个一般法则，因为那样我们将进入比本书设计范围更为技术性的数学过程。但现在我们可以立即看到，乘法的结合律（上面编号为（$3$））是成立的。首先考虑结果向量的长度；它是通过实数的普通乘法过程得到的；因此，结合律对它成立。

Again, the direction of the resultant vector is got by the mere addition of angles, and the associative law hold for this process also.

同样，结果向量的方向是通过简单的角度相加得到的，结合律对这个过程也成立。

So much for multiplication. We have now rapidly indicated, by considering addition and multiplication, how an algebra or 'calculus' of vectors in one plane can be constructed, which is such that any two vectors in the plane can be added, or subtracted, and can be multiplied, or divided one by the other.

乘法就讲到这里。我们现在通过快速地考虑加法和乘法，已经大致说明了如何构建一个平面内的向量代数或“微积分”，使得平面内的任意两个向量可以相加、相减，或互相乘、互相除。

We have not considered the technical details of all these processes because it would lead us too far into mathematical details; but we have shown the general mode of procedure. When we are interpreting our algebraic symbols in this way, we are said to be employing 'imaginary quantities' or 'complex quantities'. These terms are mere details, and we have far too much to think about to stop to inquire whether they are or are not very happily chosen.

我们没有考虑所有这些过程的技术细节，因为这将使我们过多地进入数学细节；但我们展示了大致的操作方法。当我们以这种方式解释代数符号时，我们称之为使用“虚数”或“复数”。这些术语只是细节，而我们有太多事情需要考虑，没时间停下来去探究它们是否选得非常恰当。

The net result of our investigations is that any equations like $x+3=2$ or $(x+3)^2=-2$ can now always be interpreted into terms of vectors, and solutions found for them. In seeking for such interpretations it is well to note that 3 becomes $(3,0)$, and -2 becomes $(-2,0)$, and x becomes the 'unknown' couple $(u,v)$ : so the two equations become respectively $(u,v)+(3,0)=(2,0)$, and $\left\{(u,v)+(3,0)\right\}^2=(-2,0)$

我们研究的最终结果是，类似于 $x+3=2$ 或 $(x+3)^2=-2$ 的任何方程现在都可以用向量的形式解释，并且可以为这些方程找到解。在寻找这种解释时，值得注意的是，3 可以表示为 $(3,0)$，-2 表示为 $(-2,0)$，而 $x$ 则成为“未知”对偶 $(u,v)$：因此，这两个方程分别变成了 $(u,v)+(3,0)=(2,0)$ 和 $\left\{(u,v)+(3,0)\right\}^2=(-2,0)$。

We have now completely solved the initial difficulties which caught our eye as soon as we considered even the elements of algebra. The science as it emerges from the solution is much more complex in ideas than that with which we started. We have, in fact, created a new and entirely different science, which will serve all the purposes for which the old science was invented and many more in addition. But, before we can congratulate ourselves on this result to our labours, we must allay a suspicion which ought by this time to have arisen in the mind of the student. The question which the reader ought to be asking himself is: Where is all this invention of new interpretations going to end? It is true that we have succeeded in interpreting algebra so as always to be able to solve a quadratic equation like $x^2-2x+4=0$ ; but there is an endless number of other equations, for example, $x^2-2x+4=0,x^4+x^3+2=0$, and so on without limit. Have we got to make a new science whenever a new equation appears?

我们现在已经完全解决了最初的困难，这些问题一开始在我们仅仅考虑代数的基本要素时就显现出来。从这些解决方案中产生的这门科学在思想上要比我们开始时的简单概念复杂得多。实际上，我们创造了一门全新而完全不同的科学，它不仅能够满足旧科学的所有用途，还可以实现许多额外的功能。但在为我们努力的成果庆祝之前，我们必须消除一种疑虑——到此时，这种疑虑应当已经在学生的心中产生了。读者应该问自己的问题是：所有这些新的解释发明将会通向何方？确实，我们已经成功地解释了代数，使我们始终能够解像 $x^2 - 2x + 4 = 0$ 这样的二次方程；但实际上，还有无穷多的其他方程，比如 $x^2 - 2x + 4 = 0$、$x^4 + x^3 + 2 = 0$ 等等，不胜枚举。难道我们每次遇到一个新方程时都要创造一门新的科学吗？

Now, if this were the case, the whole of our preceding investigations, though to some minds they might be amusing, would in truth be of very trifling importance. But the great fact, which has made modern analysis possible, is that, by the aid of this calculus of vectors, every formula which arises can receive its proper interpretation; and the 'unknown' quantity in every equation can be shown to indicate some vector. Thus the science is now complete in itself as far as its fundamental ideas are concerned. It was receiving its final form about the same time as when stream engine was being perfected, and will remain a great and powerful weapon for the achievement of the victory of thought over things when curious specimens of that machine repose in museums in company with the helmets and breastplates of a slightly earlier epoch.

现在，如果真是这样，我们之前的所有研究，尽管对某些人来说可能是有趣的，但实际上却显得微不足道。然而，使现代分析成为可能的伟大事实是，通过这个向量的微积分，每个出现的公式都可以得到适当的解释；而每个方程中的“未知”量都可以表示为某个向量。因此，就其基本思想而言，这门科学现在已自成体系。它在大约与蒸汽机完善的同一时期获得了最终的形式，并将继续作为一项伟大而强大的工具，推动思想战胜物质的胜利，而当那台机器的奇特样本在博物馆里与稍早时期的头盔和胸甲一起安放时，它将依然发挥作用。
