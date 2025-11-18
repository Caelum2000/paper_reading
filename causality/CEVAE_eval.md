### A Critical Look at the Consistency of Causal Estimation with Deep Latent Variable Models
1. 主要是指出了Causal Effect Inference with Deep Latent-Variable Models（CEVAE）存在的问题
2. 首先是如果不合理地假设confounder 的分布p(z)，那么结果就会不准确，例如如果假设z为gaussian，但是他是binary，就会出现问题。原因可能是这样破坏了graph，这个confounder成了某个未知的confounder
3. 其次，指出如果proxy的分布过于复杂，则会不work。这一部分和Measurement bias and effect restoration in causal inference里的一些结论有关。没仔细看
