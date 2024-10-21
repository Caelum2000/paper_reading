## SMALL-SCALE PROXIES FOR LARGE-SCALE TRANS- FORMER TRAINING INSTABILITIES
1. 探究了一些trick对大规模transformer训练不稳定性的影响。方法是将大规模transformer训练不稳定现象在小规模的transformer上出现
2. 主要是关注两种instability, 一是在attention map中logits过大的问题，二是输出的probs divergence的问题
3. 探究了warm-up, weight-decay, muParam对稳定性的影响
4. attention map logits大可以用qk-norm解决
5. 不warm-up会影响稳定性
6. 问题：muParam和z-loss是什么 