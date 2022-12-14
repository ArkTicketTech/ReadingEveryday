### 2022.12.14
本日章节 附录 B.1

### 附录
#### B.1 拉格朗日乘子法  
本节不会或者理解有困难的同学可以看这里  
https://zhuanlan.zhihu.com/p/154517678  
简单来说，拉格朗日乘子法的目的就是为了寻找**多元函数**在一组**约束**下的极值的方法。  
通过引入拉格朗日乘子，可以将有约束条件的最优化问题转变为无约束优化问题。  
对于等式约束，只需对拉格朗日函数对x与λ分别求偏导后置零即可求解。对于不等式约束，则考虑最优点在不等式约束限制的空间范围内与边界两种情况。  
如果最优点在这个范围内，那么只需考虑f(x)梯度为零的点，若最优点在边界上，则类似于上面的等式约束，但需要注意的是此时此时f(x)与g(x)的梯度必然相反。  
同时考虑二者，可以得到KKT(Karush-Kuhn-Tucker)条件。  
最后，一个优化问题可以从两个角度来考察——”主问题”与”对偶问题”。规定其对偶函数为拉格朗日函数的下确界表示，那么对于主问题可行域中的点都有式(B.8)，这是因为要求的是对应拉格朗日函数的最小化值，那么自然符合约束条件，在μ非负的情况下，自然可以得到(B.8)。  
最后可知，对偶函数给出了主问题最优值的下届，也引出了对偶问题(B.11)。但说实话，这里的对偶问题的作用我还没有完全理解，可能要在之后的学习中才能明白了。    

P62 To be continued