### SCALING LAWS FOR PRECISION
1. 提出了precision版本的scaling law，见Eq.1
2. 这里的precision主要是指quantizition时候的precision, 类如4bit, 16bit等
3. 指出了quantization的两种方式:
   1. quantization-aware training: 仅量化权重不量化激活，在做运算的时候需要反量化回去，仅为了节省带宽
   2. low-precision training: 量化权重且量化激活，仅用一种量化的数进行各种运算。节省计算时间和内存
4. 结论表明用更多的参数，更低的精度要比同FLOPs下的高精度低参数量好