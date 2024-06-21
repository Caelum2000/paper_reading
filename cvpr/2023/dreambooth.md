## Title: DreamBooth: Fine Tuning Text-to-Image Diffusion Models for Subject-Driven Generation
1. 通过少量的图片预训练stable diffusion。达到对某一个subject定制的生成
2. 对这个subject，需要用一个不常见的单词指代
3. 训练的pipeline见Figure。 
4. 提出了一个prior preservation loss. 可以提高多样性