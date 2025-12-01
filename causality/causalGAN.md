### CAUSALGAN: LEARNING CAUSAL IMPLICIT GENERATIVE MODELS WITH ADVERSARIAL TRAINING
1. 宣称不仅能够对conditional prob进行采样，更能对inervention prob进行采样的GAN
2. 由多个部分组成，causal controller, D， G，Labler, Anti-labeler。并根据causal graph进行计算见Fig,2(b)
3. Loss 如 Equation 2~5所示，虽然Eq.5比较奇怪，但appendix中证明了其作用
4. 感觉并没有做到采样任意intervention, 只是采样了在特定grapgh下的inetrvention。就是用causal controller生成了label. 而且在某些图下，$p(x|l)=p(x|do(l=l_0))$