## Title：ReLU Strikes Back: Exploiting Activation Sparsity in Large Language Models
1. 现在LLM大多用GELU，SiLU等作为actiavtion function, 因为这些函数比ReLU平滑，收敛速度和acc更好
2. 本论文表明，用ReLU在大多情况下能得到差不多的效果
3. ReLU使模型中的activation更稀疏（0值更多），因此对硬件友好（在特定硬件上可以减少IO带宽，但其实在GPU上没区别，因为GPU需要load 0）
4. 本文提出一种将LLM中GELU等转换成ReLU的方法，除此之外，还加了额外的ReLU。这样操作下来，使稀疏性大大提升