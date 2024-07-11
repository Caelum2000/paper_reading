## Title: A Watermark for Large Language Models
1. 给LLM加水印，使其生成的文字有一些固定的特征。可以通过算法检测是否有这些特征
2. 加水印的具体方法是将词表分为green and red list，然后仅从green list采样。然后用统计学假设检验方法检验
3. 本文写了一个hard的方法，一个soft的方法，其中soft对生成效果影响较小   
4. 可以生成private的水印，就是每个水印有不同的特征