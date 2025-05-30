### BLOCK DIFFUSION: INTERPOLATING BETWEEN AUTOREGRESSIVE AND DIFFUSION LANGUAGE MODELS
1. diffusion + 自回归进行NLP的工作。思路就是在一个text block内使用diffusion, 在block之间使用AR
2. 克服了diffusion生成文本固定长度和不能高效利用如KV cache的cache机制的问题
3. 这个研究方向还是比较重要的，可能是以后LLM的发展趋势
4. 一个思路是，固定长度的问题能否用diffusion operator解决？one step的diffusion opeartor(即普通的neural operator)在这里可以替换掉diffusion operator吗?
5. 放waiting list,顺便复习看一下decrete diffusion.