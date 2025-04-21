## SAM as the Guide: Mastering Pseudo-Label Refinement in Semi-Supervised Referring Expression Segmentation
1. 进行Referring Expression Segmentation （RES）。貌似是根据语言进行分割
2. 引入了半监督方法
3. 和Segment Anything Model (SAM)有关，放waiting list


### review
1. 根据半监督学习来根据natural language进行seg
2. 有一个teacher和student，teacher对unlabel的图片生成伪标签，然后指导student学习
3. 该工作在上面的基础上，使用SAM(seg anything)指导teacher生成的伪标签效果（提出IOM+CPI），见Fig.3