## A Brain-Inspired Neurodynamic for Efficient Sequence Memory

## recommendation
Accept with minor revision

### To Author
1. The author in the paper treats different layers of the proposed three-layer model as corresponding to different brain regions. For example, the second layer is considered to represent the neocortex, and the third layer is considered to represent the hippocampus. Are there any stronger arguments or evidence to support this claim, such as whether the neuronal activity in these layers could resemble the patterns of the corresp  onding brain regions?

2. The author uses STDP as the learning rule for the three-layer network model. Has there been an attempt to use reinforcement learning (or surrogate gradient) to train this SNN network? Under different learning rules, do the network's performance and the manner in which memory degradation occurs differ?


### To Editor
The paper uses a three-layer spiking neural network and the STDP learning rule to address the problem of sequence pattern recognition. While some previous works have applied such models to image classification tasks, this study conducts destructive experiments to investigate the impact of connection loss on the model’s learning. In summary, provided the author can clarify the correspondence between the proposed model and biological brain regions, I recommend accepting this paper.