## MULTI-SOURCE DIFFUSION MODELS FOR SIMULTANE- OUS MUSIC GENERATION AND SEPARATION
1. 分不同的source用diffusion进行音乐生成（例如交响乐有钢琴，小提琴等不同source）
2. 可以对mix的音乐信号分离source，具体方法是用mix做label， 然后condition DDPM
3. 有代码，直接github搜索