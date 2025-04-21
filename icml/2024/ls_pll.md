## Does Label Smoothing Help Deep Partial Label Learning?
1. 利用label smoothing 解决 Partial Label Learning
2. label smoothing和Partial Label Learning都不知道是什么，放waiting list


### review
1. 该工作主要解决partial labeling learning 中出现false-positive的label问题，这个离群点会对test产生影响。解决方法是label smoothing，把false-positive离群点平滑掉
2. partial label 指的是一个data sample有多个标签的情况，比如人工标注时对于一条数据可以不同人有不同的标注
3. label smoothing就是把hard的one-hot平滑成一个连续的分布，见Eq.1, Eq.2