# Language Generation in the Limit Tutorial @ COLT 2025

## 前序工作：Works on Language Generation in the Limit
1. Language Generation in the Limit 就是指在有限的时间步下，辨识一种语言。
2. 这里“辨识”的定义不是很清晰，比如算法提前知道什么信息？
3. 论文：Language Identification in the Limit — E. Mark Gold

### Language Generation in the Limit
1. 在有限时间步内，不断对算法输入一个语言L中的string，然后该算法需要输出语言中的string
2. 论文：Language Generation in the Limit — Jon Kleinberg and Sendhil Mullainathan
3. 有一篇从学习理论角度看该过程的，有点意思：Generation through the Lens of Learning Theory — Jiaxun Li, Vinod Raman, and Ambuj Tewari 

### Language Generation in the Limit with Breadth
1. 该部分就是强调：在generation的过程中，不仅仅需要能够生成语言，还需要breadth。就是说不能mode collapse
2. 论文：On the Limits of Language Generation: Trade‑Offs Between Hallucination and Mode Collapse — Alkis Kalavasis, Anay Mehrotra, and Grigoris Velegkas 。改论文是说语言模型的幻觉和mode collapse不可兼得。幻觉对应生成的语言不准确，mode collapse对应没有breadth


### 思考
1. 能不能将Trade‑Offs Between Hallucination and Mode Collapse的证明思想用到ai safety上，即ASR和性能不可兼得
2. 有一篇论文：Generation from Noisy Examples — Ananth Raman and Vinod Raman。该文章主要是研究在上述场景设置下，如果给算法输入有噪声的数据，那么算法能不能生成真实的语言？这是否能用到模型学习时剔除有害信息？