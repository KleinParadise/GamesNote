### 矩阵实现2D线性变换
一个顶点(x,y)可以写成为一列的矩阵,再与对应功能的变换矩阵相乘,实现对顶点的变换
1. ***Scale***   
![pic_one](/Image/trans1.png)  
2. ***reflection***  
![pic_one](/Image/trans2.png)  
3. ***shear***  
![pic_one](/Image/trans3.png)  
3. ***rotate***  
![pic_one](/Image/trans4.png)  


### 齐次坐标

***为什么要引入齐次坐标？***  

对一个顶点(x,y)的位移操作,无法通过两矩阵的相乘来实现。  
![pic_one](/Image/trans5.png)  
![pic_one](/Image/trans6.png)  

通过齐次坐标,可以让位移操作也满足线性变换。  
![pic_one](/Image/trans7.png)  
![pic_one](/Image/trans8.png)  



### 先变换再平移  
![pic_one](/Image/trans9.png)  
先平移在变换  
![pic_one](/Image/trans10.png)   
先变换再平移  
![pic_one](/Image/trans11.png)  

### 矩阵变换(相乘)不满足交换率  
![pic_one](/Image/trans12.png) 

### 先矩阵相乘再乘顶点
![pic_one](/Image/trans13.png)  

### 复杂的顶点变换处理
先将顶点变换原点,在执行变换矩阵操作,变完之后在平移回原来的位置  
![pic_one](/Image/trans14.png)
  

### 3D顶点变换矩阵  
![pic_one](/Image/trans15.png)  
