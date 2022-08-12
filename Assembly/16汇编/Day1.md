# Day1

16位CPU：8086
32位CPU：x86
64位CPU：x64 / x86_64
![image.png](https://upload-images.jianshu.io/upload_images/22388988-833c09bb8e3b9358.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![image.png](https://upload-images.jianshu.io/upload_images/22388988-cbd8408605d8b460.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
通用寄存器可以操作高8位和低8位，其他寄存器不行
![image.png](https://upload-images.jianshu.io/upload_images/22388988-fdbd6cb8645c9942.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
windows自带用法DEBUG
-u：从IP地址开始看汇编
![image.png](https://upload-images.jianshu.io/upload_images/22388988-993714610db729a1.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
-a：从IP地址处开始写汇编
![image.png](https://upload-images.jianshu.io/upload_images/22388988-c6db68f904376fde.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
-g：从IP地址开始执行
![image.png](https://upload-images.jianshu.io/upload_images/22388988-7a1f1a9dedaae9b8.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
-p：单步执行
![image.png](https://upload-images.jianshu.io/upload_images/22388988-93102d06a41d823a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

---
进位标志CF（NC变成CY）
![image.png](https://upload-images.jianshu.io/upload_images/22388988-16cc1ff214544a2e.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![image.png](https://upload-images.jianshu.io/upload_images/22388988-0f1e1c07865923de.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

零标志ZF（NZ变成ZR）
![image.png](https://upload-images.jianshu.io/upload_images/22388988-666f6a29f67bcb40.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![image.png](https://upload-images.jianshu.io/upload_images/22388988-33cf2b4af023772c.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![image.png](https://upload-images.jianshu.io/upload_images/22388988-b338a5d9061829a4.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

符号标志SF（NG是负数，PL是正数）
检验运算结果是不是负数。
![image.png](https://upload-images.jianshu.io/upload_images/22388988-0b7c53caa490e668.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![image.png](https://upload-images.jianshu.io/upload_images/22388988-67fbeb5d02701bed.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

奇偶标志PF（PO是奇数，PE是偶数）
![image.png](https://upload-images.jianshu.io/upload_images/22388988-baf1261b285bae96.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![image.png](https://upload-images.jianshu.io/upload_images/22388988-90fc3e593ac49cea.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

溢出标志OF（ 没溢出是NV，溢出是0V）
无符号数计算不会溢出，有符号数计算才考虑溢出。
7fff是最大的有符号数32767 7fff+1=8000 也就是-32768
32767+1=-32768（同号相加）
同理 -32768-1 =32767（异号相减）
会出现溢出
![image.png](https://upload-images.jianshu.io/upload_images/22388988-2564c5f61fb73395.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![image.png](https://upload-images.jianshu.io/upload_images/22388988-c96c4055a6856241.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

辅助进位标志AF（没进位是NA，进位是AC）
![image.png](https://upload-images.jianshu.io/upload_images/22388988-88ed95193640cec7.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![image.png](https://upload-images.jianshu.io/upload_images/22388988-414d1d9bf85d44a6.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

方向标志DF
![image.png](https://upload-images.jianshu.io/upload_images/22388988-3eab273d26357f0f.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

中断允许标志IF
![image.png](https://upload-images.jianshu.io/upload_images/22388988-503a11375f008f42.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

陷阱标志TF
![image.png](https://upload-images.jianshu.io/upload_images/22388988-51427bee4c49bbb6.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![1653447631(1).png](https://upload-images.jianshu.io/upload_images/22388988-a9a11bccff2c0765.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)