# 计算机视觉初体验

## 1、基础知识
首先最基本的问题是**什么是计算机视觉？**
>计算机视觉被视为人工智能的重要分支，即让计算机利用人工智能去认识世界的方式。计算机视觉包括图像处理、机器学习、三维理论。更进一步的说，就是使用摄像机和电脑代替人眼对目标进行识别、跟踪和测量等机器视觉，并进一步做图形处理，使电脑处理成为更适合人眼观察或传送给仪器检测的图像。

### 计算机视觉的应用

无人驾驶、人脸识别、以图搜图、VR/AR、3D重构、医学图像分析、无人机等。如今计算机视觉的涉及可以说是无处不在。   such as：微软公司推出的Kinect,即是能够模拟人的动作的技术，其核心技术是在于通过捕捉人的骨架运动来效仿玩家的动作，让玩家可以透过直接的动作与电脑互动。

### 图像处理

高度、宽度   
假如一张照片的分辨率为：1920*1080dpi（单位），1920就是照片的宽度，1080就是图片的高度。

深度    
存储每个像素所用的位数，比如正常RGB的深度就是 2^8 * 3 = 256 * 3 = 768 ， 那么此类图片中的深度为768，每个像素点都能够代表768中颜色。

通道数   
RGB图片就是有三通道，RGBA类图片就是有四通道

颜色格式   
是将某种颜色表现为数字形式的模型，或者说是一种记录图像颜色的方式。比较常见的有：RGB模式、RGBA模式、CMYK模式、位图模式、灰度模式、索引颜色模式、双色调模式和多通道模式。

图片格式与压缩     常见的图片格式JPEG，PNG，BMP等都是图片的一种压缩编码方式   
举例：JPEG压缩   
1、将原始图像分为8*8的小块，每个block里有64pixels。   
2、将图像中每个8*8的block进行DCT变换     

图像的采样和量化  
 一般来说，采样间隔越大，所得图像像素数越少，空间分辨率低，质量差，严重时出现马赛克效应；采样间隔越小，所得图像像素数越多，空间分辨率高，图像质量好，但数据量大。   
 ![图像采样]（https://images2015.cnblogs.com/blog/1150128/201704/1150128-20170423180408804-1321761433.png）
