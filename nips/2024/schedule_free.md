## The Road Less Scheduled
1. 貌似提出了一种不需要scheduler的优化器。
2. 放waiting list


### review
1. 需要对位置求滑动平均，而不是对grad求滑动平均，这也许等价动量法，但没太见过。需要看前置工作
2. 现在要搞清楚该工作相对于之前工作的改进是什么，要解决什么问题即exact worst-case optimal rates。需要看Exact convergence rate of the last iterate in subgradient methods和hen, why and how much? adaptive learning rate scheduling by refinement.
3. 还是没搞清楚在解决什么问题, 动量似乎是它提出的method的一种特殊情况，文章给人感觉很怪
4. 提出的方法其实在在Polyak-Ruppert (PR) average 和 primal average之间折中，primal average就是动量法