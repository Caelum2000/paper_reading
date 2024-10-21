## Title: LeanDojo: Theorem Proving with Retrieval-Augmented Language Models
1. 利用RAG的方法进行机器定理证明
2. 基于的baseline是Lean，一个机器定理证明框架
3. RAG具体用在哪里？RAG用于 premise selection. 就是证明定理的时候需要引理，premise selection就是根据要证明的定理选择引理
4. 怎么进行RAG？就是根据encode后的余弦相似性