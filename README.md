# MachineLearning
## Original notes on Machine Learning, all rights reserved. NO REPRINT.

## 写在前面：

不管是机器学习还是深度学习，对数学的要求都超过对编程能力的要求。确实，很多算法都有开源代码，不杀猪甚至不花钱就能得到猪肉。沿用这一类比，如果只会调包，而不知其所以然，就好比囫囵吞枣似的生吃猪肉。将探索机器学习领域时的思考总结记录存档，总结的目的不是为了强调“是什么”，而是为了突出由“做什么→怎么做（为什么）→是什么”的中间过程。

很多思路都是相似的，比如Vapnik希望找到一条“街道”把平面上不同类别的点分开，并且“街道”越宽越好，他以此构造成本函数，再经过他在数学上的处理，在1960s的时候，他得到了支持向量机。进一步讲，如果数据集在当前空间线性不可分，可以通过空间映射的手段，将数据值映射至高维空间，达到线性可分的目的。将这一处理方式引入SVM中，在数学公式中发现，我们需要的只是两个映射后的高维空间向量的点积，它是一个标量。有没有手段可以跳过从低维到高维的映射，直接获得这一标量呢？答案是肯定的，因为找到了核函数的方法，直接由低维向量在低维变换后点积运算，同样可以得到前述标量。

而PCA的算法流程与此类似，同样是构造成本函数，求解成本函数最值。而PCA中携带着“正交”的概念，假设用于叠加的基向量相互正交，互不影响。这种正交叠加的思想在数学中很常见，比如拉普拉斯提出的中心极限定理，比如高斯提出的正态分布。AdaBoosting方法延续了正交的概念，不断生成弱分类器，通过上调弱分类器中偏差较大分量的w值，扩大弱分类器的表征空间，最后，将所有弱分类器叠加得到强分类器。

提醒一句，机器学习和深度学习领域一直在衍生新名词，但相比于20年前，方法的本质并没有发生太多变化。有很多层的人工神经网络改头换面，称之为“深度学习”，以前的统计学习方法也被重新包装起来，更名为“机器学习”。在计算速度和智能硬件飞速发展的信息时代，统计学习方法被催化着生根发芽，长成了枝叶茂密的大树大花。

乱花渐欲迷人眼，过多关注表面的东西，人会很容易迷离。而在统计学习的数学世界里，草浅尚未没马蹄。
## 
0.1.BP神经网络的工作原理

0.2.傅里叶变换和卷积初探

0.3.卷积积分和卷积神经网络

0.4.K-means聚类

0.5.核函数

0.6.subsampling方法

0.7.支持向量机

1.1.二分类的成本误差和梯度下降法

1.2.前后向传播和梯度下降法的实现

1.3.Python的广播机制和入门实践

1.4.激活函数的选择
