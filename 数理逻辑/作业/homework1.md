# 作业一
## 1.形式化

记鱼越大为命题A，鱼刺越大为命题B，鱼肉越少为命题C。

(1) A$\rightarrow$B (2) B$\rightarrow$C (3) C$\rightarrow$$\lnot$ A (4)结论：A$\rightarrow$$\neg$A

(1)与(3)相互矛盾，因为A与$\neg$A不可能同时成立，所以在逻辑上不是有效的，因此根据(1)(2)(3)得到结论(4)在逻辑上不是有效的。
## 2.证明：

因为每个命题符号都是wff

所以存在长度为1的wff

若a,b均为wff,则($\neg$a)与(a$\Box$b)均为wff,其中$\Box$是$\wedge$,$\vee$,$\rightarrow$,$\leftrightarrow$中一个

所以存在长度为4或5的wff，又因为除此以外的都不是wff,所以不存在长度为2或3的wff

假设存在长度为6的wff,显然,这个wff的形式与($\neg$a)与(a$\Box$b)中的一个相同，这与不存在长度为2或3的wff矛盾，假设不成立，不存在长度为6的wff

记c为长度为1的wff

则c,(c$\vee$c),(c$\vee$(c$\vee$c))的长度分别为1,5,9

又因为对原wff每取一次否会使wff的长度增加3，所以wff的长度为3n+1或3n+5或3n+9,(n=0,1,2,……)

综上所述,不存在长度为2,3或6的wff,但其他任意正整数长度的wff均可能存在。
## 3.证明：

记A为长度为1的wff

Base Case:当c=0时,$\alpha$形如A或($\neg$A),s=1,s=c+1成立

Induction Hypothesis:假设当c=n时,s=c+1成立,记此时wff为B

Inductive Step:当c=n+1时,此时的wff必形如(A$\Box$B),(($\neg$A)$\Box$B),(B$\Box$A),(B$\Box$($\neg$A))中的一个,其中$\Box$是$\wedge$,$\vee$,$\rightarrow$,$\leftrightarrow$中一个,此时s=c+1显然成立

综上，由数学归纳法可知：若$\alpha$是一个wff,则s=c+1成立
## 4.证明：

先证S′$\subseteq$S:


因为S′ = {α | 存在有穷构造序列 <α0, α1, . . . , αn> 使得 αn = α 且对任意 i ≤ n 满足定义 1.4 的3个条件之一}

所以$\forall$$\alpha$$\in$S′,$\alpha$是wff，所以S′$\subseteq$S成立

再证S$\subseteq$S′:$\forall$$\alpha$$\in$S,$\alpha$是wff，又因为wff均可由有限步产生，因此存在一个有穷构造序列 α0, α1, . . . , αn 使得 αn = α 且对任意 i ≤ n 满足定义 1.4 的 3 个条件之一，所以S$\subseteq$S′成立

综上所述，S′ = S