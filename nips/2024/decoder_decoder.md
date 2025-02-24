## You Only Cache Once: Decoder-Decoder Architectures for Language Models
1. 只用decoder，只需要cache一次KV cache
2. 放waiting list

### review
1. 有两个decdoer, 第一个是self-decoder, 第二个是cross decoder
2. self-decoder 产生一个global KV，然后在cross decoder中共用这个gloabl KV,这样一来就可以只cache一次cross-decoder中的KV（即 global KV）
3. self-decoder使用了一个efficient attention使KV cache的memory复杂度降低