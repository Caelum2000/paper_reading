## Title: Meta Continual Learning Revisited: Implicitly Enhancing Online Hessian Approximation via Variance Reduction
1. 介绍了CL的两种approaches: regularization based 和 meta-learning based
2. 在regularization based中，主要是估计hessian还还原之前task的信息，但是propostion 1的推导貌似有些奇怪。table.1 中hessian的逆也有点反直觉。需要调研之前的相关工作
3. meta-learning framework 中，作者提出本质上是对于memory buffer中数据的Hessian进行估计，见propostion 2. 但 propostion 2中 $H^{j}_M=\nabla^2_{\theta_k} L$感觉应该是$H^{j}_M=\nabla_{\theta_k} \nabla_{\theta} L$ ?
4. 提出了一种类似EMA的方法，来减小meta-learning 梯度估计中的 variance, 这个具体数学细节没check。