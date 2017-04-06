# PRML中概率论部分学习

标签（空格分隔）： 概率论 机器学习

---

#1 概率论
![此处输入图片的描述][1]
两个不同颜色的盒子中放着不同的水果。
盒子颜色记为随机变量B，B={r,b}
$$ p(B=r)=\frac{4}{10}; $$
$$ p(B=r)=\frac{6}{10}; $$


  [1]: https://raw.githubusercontent.com/taogg123/learning/74b7f2a1a3f8eb3ba00f329dacf353cd31fecf9a/picture/box.png

**联合概率**：
$p(X=x_i,Y=y_i)=\frac{n_{ij}}{N}$

**加和规则**：
$ p(X=x_i)=\sum_{j=1}^Lp(X=x_i,Y=y_j) $
>$p(X=x_i)$有时又称作边缘概率（marginal probability），是因为它是由忽略其他条件而得到的

**乘积规则**
$ p(X,Y)=p(X|Y)p(Y) $

**贝叶斯定理（Bayes' theorem）**
$$ p(Y|X)=\frac{p(X|Y)p(Y)}{p(X)} $$
利用加和规则可以将贝叶斯公式的分母写成如下形式
$$ p(X)=\sum_Yp(X|Y)p(Y) $$

在观察水果之前就可以知道$p(B)$,称为**先验概率（prior probabilility）**。
知道了水果，通过贝叶斯公式求出$p(B|F)$称为**后验概率（posterior probability）**。



  
  