### The WMDP Benchmark: Measuring and Reducing Malicious Use With Unlearning
1. 提出了一个科学安全数据集，并用这个数据集进行unlearning来alignment
2. 包含生物化学和计算机三个方面。对每个方面分析了可能产生有害影响的方式，并根据这个进行针对性生成。相当于对生成数据的llm进行了CoT。
3. unlearning方式很简单，就是对齐表征，见Alg.1和Fig.7