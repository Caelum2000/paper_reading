## DiffWire: Inductive Graph Rewiring via the Lovász Bound
1. 对图进行rewire从而减小over-squashing和over-somthing等问题
2. 提出了CT-layer，通过学习commute embedding来计算commute time，进而算Effective Resistance，然后可以得到哪里是bottleneck，从而在这个地方加edge，缓解over-squashing
3. 提出了GAP-layer,通过减小特征值之间的差距来增大Lovász Bound，从而解决over-smoothing?