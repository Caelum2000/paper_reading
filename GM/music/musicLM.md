## Title: MusicLM: Generating Music From Text
1. 利用 VQ-VAE + autoregressive 模型
2. 利用类似CLIP的MuLAN实现由text-to-audio特征的转变，然后condition到autoregressive模型
3. 疑问：为什么要加一个w2v-BERT，貌似多此一举 