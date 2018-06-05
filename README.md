# MINLP resource
MINLP (Mixed integer nonlinear programming) 问题被[Jon Lee](https://ioe.engin.umich.edu/people/jon-lee/)誉为所有确定性规划之母。
该类问题在工程和科学问题中广泛存在。举例来说，电气工程中的机组运行优化，输电拓展，通信工程中的信息攻击的最优响应，无线带宽。 有相关文章已经说明证明MINLP问题不能被任何单个算法求解，即使是有很小规模整数变量的问题。
这一类问题求解复杂，但由于有着很广泛的应用前景和研究价值，所以相关的研究也在不断推进。

目前来说，求解此类问题主要有两大类算法。一类是确定性优化算法，另一类是problem independent的进化算法。由于进化算法不是专门设计解决MINLP问题，所以这里不错详细介绍。
解决MINLP问题的确定性优化算法主要包括single-tree类和multi-tree类。single-tree类有非线性分支定界法（nonlinear branch and bound）和非线性分支裁剪法（
Nonlinear Branch and cut）。而multi-tree类主要是基于解耦思想的外部近似法（outer approximation method）和benders解耦法 (Benders decomposition method)。


**推荐相关的专著**

[Mixed-Integer Nonlinear Optimization](http://www.mcs.anl.gov/papers/P3060-1112.pdf)

[Review of Nonlinear Mixed-Integer and Disjunctive Programming Techniques](https://link.springer.com/article/10.1023/A:1021039126272)

[Mixed-integer nonlinear programming techniques for the synthesis of engineering systems](https://pdfs.semanticscholar.org/b784/47c13d3e62aa680c29bcd241bfbc1716eb7b.pdf)

**PPT介绍**

[Mixed Integer Nonlinear Programming algorithms](https://www.ibm.com/developerworks/community/wikis/form/anonymous/api/wiki/de368162-e90b-432c-a4e9-795cc51440dd/page/3758050a-ad9b-4e9a-a22b-6f6731b88742/attachment/25008c4e-d432-44b3-845b-e1ed744b7d0a/media/ROADEF_MINLP_english.pdf)  IBM公司文件，自动下载链接

当然也要介绍一下这个领域泰斗级的人物，也就是outer approximation algorithm的提出者[Ignacio Grossmann教授](http://egon.cheme.cmu.edu/)。

MINLP由于有着整数和连续变量，甚至包括在整数变量确定时存在非线性特性，因此，在使用确定性规划求解时，必然涉及到运筹与优化中基础的优化问题，如NLP（Non-linear programming）问题，ILP（Integer linear programming）问题。这两方面的问题都有成熟的求解算法。如果想补一补基础可以学习[Stephen P. Boyd](https://web.stanford.edu/~boyd/)的[convex optimization](http://web.stanford.edu/class/ee364a/)，有很详细的slides，电子书，以及视频教程。

**Solvers**

支持Matlab平台的有：
Matlab自带的Optimization Toolbox，[Cvx](http://cvxr.com/cvx/)，[YAMLIP](https://yalmip.github.io/)，等

使用C，C++，Python语言的优化工具包[COIN-OR](https://github.com/coin-or),可解决问题的类型很广泛，推荐，也是本人以后要长期研究学习的一个工具包。



