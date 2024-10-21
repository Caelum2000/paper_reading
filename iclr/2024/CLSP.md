## CANDIDATE LABEL SET PRUNING: A DATA-CENTRIC PERSPECTIVE FOR DEEP PARTIAL-LABEL LEARNING
1. 研究内容是PLL，partial-label learning. 是一个样本有多个候选标签，只有一个是真的
2. 采用kNN对样本的label剪枝，将离群的label挑出来
3. 问题：label的repsentation sapce怎么得出，比如离散的标签，如类别怎么embedding