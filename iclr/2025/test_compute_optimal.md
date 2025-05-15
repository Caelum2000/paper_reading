## SCALING LLM TEST-TIME COMPUTE OPTIMALLY CAN BE MORE EFFECTIVE THAN SCALING PARAMETERS FOR REASONING
1. 研究的问题是对于LLM，怎么在inference的时候通过增加计算开销来提升推理质量
2. 本文指出，对于不同难度的prompt，需要不同的提升方法，并设计一种adaptive的方法，可以通过prompt难度来选择不同的提升算法
3. 常见的推理时提升算法在Fig.2