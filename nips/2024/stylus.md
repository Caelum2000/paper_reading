## Stylus: Automatic Adapter Selection for Diffusion Models
1. 提供一系列adapter,然后根据输入的promopt选择最合适的promopt
2. 用一个vlm对每个adapter的能力进行描述，生成描述的方式是通过vlm对adapter的model card进行总结。model card有该adapter的生成的图片和prompt
3. 利用一个llm判断输入的prompt是否与对adapter的描述匹配