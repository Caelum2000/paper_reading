## DAB-DETR: Dynamic Anchor Boxes are Better Queries for DETR
1. 指出DERT原始论文中收敛慢的原因在于没在transformer decoder中加positional embedding, 而是采用了可学习的位置编码
2. 在decoder的key中加上了positional embedding，然后query采用可学习的anchor 4元组(x,y,w,h). 详情见Fig.1的对比图
3. 不断更新anchor 4元组