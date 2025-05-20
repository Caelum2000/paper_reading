### IMPROVING PROBABILISTIC DIFFUSION MODELS WITH OPTIMAL DIAGONAL COVARIANCE MATCHING
1. 指出diffusion process使用固定的covariance会拖慢速度，因为之前的工作表明固定covariance需要很大的T。
2. 本文基于之前的一个Moment matching的工作，寻找最优的covariance
3. 问题：covariance对diffusion 整个pipeline的影响是否有一些更具有“物理意义”的解释？类似从scoring matching或optimal transport的角度？如果仅是“调” convariance，那仅仅就是一调参的过程。（答案可能在VDM系列或本文的related work）