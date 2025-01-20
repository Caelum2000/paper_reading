## Aligner: Efficient Alignment by Learning to Correct
1. 通过给LLM是输出回答接入另一个aligner，来refine LLM的回答
2. 本质上是二次推理(self-judge, self-reminder)，但aligner比较轻量级