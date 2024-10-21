## ZIPFORMER: A FASTER AND BETTER ENCODER FOR AUTOMATIC SPEECH RECOGNITION
1. zipformer针对语音识别任务，是基于conformer(transformer+Conv)进行改进
2. 将transformer改成了unet的结构，可以不同尺度交互
3. 更改了convformer中的layernorm, 改为了类似RMSnorm的形式。
4. 更改了激活函数和优化器
5. 为什么要用RMSnorm? layernorm计算量大而且有一个可学习的factor,因此没必要减去均值除以标准差这么复杂