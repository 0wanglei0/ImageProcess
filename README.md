# ImageProcess
自适应图像增强算法

1）代码是从Android项目中独立出来的，适应图片默认格式为RGBA

2）计算均值时，M(i,j)可以从M(i, j-1)或者M(i-1,j)中推断出来，所以算法复杂度为n*W*H，n为计算均值时窗口大小，WH为像素大小。

3）用一个Mat提前计算好每个窗口列的值，算法复杂度还可以直接优化到O(W*H)
