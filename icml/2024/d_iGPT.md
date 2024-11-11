## Rejuvenating image-GPT as Strong Visual Representation Learners
1. inspire from 之前iGPT的工作，就是根据之前的pixel预测下一个pixel(autoregressive)。这个工作是预训练一个ViT构成的encoder, 从前面patch的encode预测下一个patch的encode
2. 采用了蒸馏的方法，使ViT encoder对其一个tokenizer(Eg. CLIP). 有一个Discriminative Docoder对其之前patch的encode。Generative Decoder对其下一个patch的encode。（见Fig.2; Eq.6 Eq.7 ）