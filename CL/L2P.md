## Learning to Prompt for Continual Learning
1. 通过学习key-prompt pair来实现CL
2. key-prompt在这里是一对可学习的vector，可以看作给网络的condition
3. 输入图片经过选择网络得到keys，然后把对应keys的prompts输入网络
4. 选择网络是一个pretrain的encoder。prompt有一个prompt pool，一个图片可以对应多个keys
5. 训练loss在Eq.5。分选择网络部分和具体任务部分