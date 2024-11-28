## MagicLens : Self-Supervised Image Retrieval with Open-Ended Instructions
1. 多模态RAG的工作。输入text+image作为query，然后查找image作为answer,见Fig.1
2. 设计了一套生成训练数据的pipeline
3. 将query的image 和 text 用clip等打成embedding然后放进encoder，最后用encoder得到的vector进行retrieval。见Fig.2
4. 利用对比学习的loss进行训练 query-answer对