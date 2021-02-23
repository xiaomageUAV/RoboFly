![image](https://github.com/xiaomageUAV/RoboFly/blob/master/04_images/top_3d%20(2).PNG)

# 简介

RoboFly是小马哥在2018年8月推出的一款完全开源的小四轴。

这款小四轴开发的初衷是为了让大家更低成本的通过一个完整的小项目来学习电路板设计、STM32编程开发、四轴飞行器的基本原理等知识。


# RoboFly的硬件架构

主控：STM32F103C8T6(没错，就是在2020年底因缺货疯狂涨价的的芯片之一)

姿态传感器：MPU6050

气压计：SPL06/FBM32/BMP280

无线通讯：2.4G

![image](https://github.com/xiaomageUAV/RoboFly/blob/master/04_images/hardwareframe.png)

# 开发说明

硬件设计软件为Altium Designer

程序文件使用Keil 打开即可，需要自行安装相关库。

因尺寸限制，STM32F013C8T6下载程序接口为SH1.0 5P端子口，配合e-Link32烧录器进行下载即可。

![image](https://github.com/xiaomageUAV/RoboFly/blob/master/04_images/top_smt.JPG)

# 打样焊接装配说明

PCB为两层板，通用工艺，基本上所有板厂都可以加工打样，成本低廉。板子用到的阻容器件最小为0603，而且在布局的时候已经考虑手工焊接的因素，布局较为松散，方便焊接。

板子上除了气压计使用烙铁焊接有一点难度之外，其他所有器件基本可以使用烙铁焊接完成。推荐使用刀头烙铁进行焊接。

焊接装配参考下图进行即可

###### 注意事项：气压计1脚标识在肚子上，而不是铁壳上的气孔。如果错误的把气孔当作1脚标识，可能会焊接反了导致板子上3.3V对地短路。

![image](https://github.com/xiaomageUAV/RoboFly/blob/master/04_images/Assembly%20drawing.png)
