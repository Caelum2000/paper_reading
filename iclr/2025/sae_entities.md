### DO I KNOW THIS ENTITY? KNOWLEDGE AWARENESS AND HALLUCINATIONS IN LANGUAGE MODELS
1. 使用LLM的内部表示来解释和判断幻觉为什么产生
2. 用了Sparse AutoEncoder(SAE)LLM的representation进行reconstruction, 并使用中间的隐变量来解释LLM
3. SAE可以上采样特征（隐变量更大），而且保持稀疏的约束。见Eq.3。这一点是否可以用snn实现？