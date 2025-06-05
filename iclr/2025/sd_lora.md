### SD-LORA: SCALABLE DECOUPLED LOW-RANK ADAPTATION FOR CLASS INCREMENTAL LEARNING
1. 使用lora做continual learning（class incremental）
2. 指出vanilla lora不能很好的学到方向的模，见Eq.3. 因此作者提出方向和模分别学习
3. class incremental的方法是Eq.4, 不断加多个lora项