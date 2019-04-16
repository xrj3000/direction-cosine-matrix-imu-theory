# 向量点叉乘
在计算DCM、使用它的元素进行导航和控制的时候，我们将用到两个非常有用的向量乘法：点乘和叉乘。两个向量A和B的点乘结果是一个标量，通过执行矩阵的乘法——A作为行向量、B作为列向量而被计算出来：
$$
A\cdot B=A^TB=\left[\begin{matrix}A_x&A_y&A_z\end{matrix}\right]\left[\begin{matrix}A_x\\A_y\\A_z\end{matrix}\right]=A_xB_x+A_yB_y+A_zB_z \tag{Eqn. 8}
$$

其实两个向量的点乘产生的结果等于两向量模的乘积，乘以两向量夹角的余弦值：
$$
A\cdot B=\left|A\right|\left|B\right|\cdot cos(\theta_{AB}) \tag{Eqn. 9}
$$
 注意点乘是可交换的：$ A \cdot B=B\cdot A $。两个向量A、B的叉乘结果是一个向量，这个向量的各个组成部分由下面公式计算出来： 
$$
\left(A\times B\right)_x=A_yB_z-A_zB_y\\
\left(A\times B\right)_y=A_zB_x-A_xB_z\\ 
\left(A\times B\right)_z=A_xB_y-A_yB_x 
\tag{Eqn. 10}
$$
这个向量垂直于A、B向量，它的模等于两向量模的乘积，乘以夹角的正弦值：

![orth](../images/orth.png)

另一方面：
$$
(A\times B)\cdot A=(A\times B)\cdot B=0\\
|A\times B|=|A||B|sin(\theta_{AB}) \tag{Eqn. 11}
$$


注意叉乘是反交换的：$A\times B=-B\times A$
