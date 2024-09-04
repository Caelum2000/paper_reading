## A Mechanistic Understanding of Alignment Algorithms: A Case Study on DPO and Toxicity
1. 研究LLM有害词汇的产生机制。是由MLP中一些特定的vector产生
2. 研究了DPO对齐消除有害词汇的机制。并没有消除MLP中有害的vector，使MLP的输入不会激活那些vector
3. 提出了通过扩大MLP有害vector的激活区域来攻击DPO对齐效果的方法。就是扩大有害vector的模值，激活区域就会扩大