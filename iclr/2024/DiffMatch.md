## DIFFUSION MODEL FOR DENSE MATCHING
1. dense matching就是给定两幅类似的图片，求pixel之间的对应关系
2. 这个工作利用diffusion进行dense matching, diffusion出来的是对应的残差映射，即Eq.1中的F
3. 利用source和target图片的特征做condition信息，具体是用特征求一个相似度Eq.8，和初始的F_init
4. 声称该方法考虑了先验p(F), 而之前的方法是最大似然，该工作最大后验. Sec4.1 Sec4.2