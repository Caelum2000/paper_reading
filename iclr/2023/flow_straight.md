## Title: Flow Straight and Fast: Learning to Generate and Transfer Data with Rectified Flow
1. 拟合ode的系数，使该系数符合直线ode的演化Eq.(1). 具体来说，对于两个不同分布的点x0,x1. 拟合ode需要使其接近x1-x0 
2. 注意ode不会使路径相交
3. 多次拟合后ode会越来越接近直线，但不需要Xt
4. 问题：为什么越接近直线越好