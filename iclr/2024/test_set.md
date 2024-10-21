## PROVING TEST SET CONTAMINATION IN BLACK BOX LANGUAGE MODELS
1. 该论文的目的是检测是否某个test set在pretrain的时候被使用
2. 方法是打乱test set中的某些可以替换顺序的部分，比如问句的顺序，见Fig.1
3. 看LLM是否对特定顺序输出大的likehood
4. 我感觉这个方法的有效性取决于在pretain的时候是否是将打乱顺序的部分当一个seqence训练的。要是属于不同的seqence可能效果不明显    