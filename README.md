# 最优化学习代码记录
近期在学习最优化过程中，对优化方法使用小算例进行简单复现，自变量维度2，主要学习来源：崔雪婷老师的视频https://space.bilibili.com/507629580/video.
1.坐标轴交替下降法，求解二次函数，分别使用坐标轴方向作为下降方向，精确线搜索计算步长；
2.改进的坐标轴交替下降法，求解二次函数，使用坐标轴下降的合成方向作为最终下降方向，精确线搜索计算步长； 
3.最速下降法，求解二次函数，使用负梯度方向作为下降方向，精确线搜索计算步长；
4.牛顿法，求解凸二次函数，使用泰勒展式拟合后的函数梯度作为下降方向，步长为纯牛顿步长；
5.牛顿法，求解四次函数，使用泰勒展式拟合后的函数梯度作为下降方向，步长为纯牛顿步长；
6.修正牛顿法，求解四次函数，使用两种方法（1.对hesse阵增加单位阵；2.特征值分解，对不满足要求的特征值进行调整）实现矩阵正定得到下降方向，步长为纯牛顿步长；
7.拟牛顿DFP方法，求解四次函数，对hesse阵增加单位阵作为初始矩阵，DFP公式计算Hk+1进而得下降方向，步长为纯牛顿步长；
8.拟牛顿BFGS方法，求解四次函数，对hesse阵增加单位阵作为初始矩阵，BFGS公式计算Bk+1进而得下降方向，步长为纯牛顿步长；
9.拟牛顿SR-1方法，求解四次函数，对hesse阵增加单位阵作为初始矩阵，SR-1公式计算Bk+1进而得下降方向，步长为纯牛顿步长；
10.线性共轭梯度法，求解凸二次函数，根据梯度信息+目标函数的二次型矩阵，计算得到下降方向和步长；
11.非线性FR共轭梯度法，求解四次函数，根据梯度信息计算下降方向，使用Goldstein方法得到步长；
12.非线性PRP共轭梯度法，求解四次函数，根据梯度信息计算下降方向，使用Goldstein方法得到步长；
