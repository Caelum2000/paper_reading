## Title: LEARNING ENERGY DECOMPOSITIONS FOR PARTIAL INFERENCE IN GFLOWNETS
1. related work里一些GFlowNet的变体 
2. GFlowNet 仅有final state 的 reward, 因此是稀疏，会造成一些问题。对此之前有文章进行了改进，把每个state加一个energy
3. 本文的贡献是将一条轨迹不同动作的energy进行分解，并学习到分解后的能量。见Eq.3.
4. 将分解后的能量加到DB loss里，见Eq.4