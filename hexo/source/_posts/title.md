---
title: Premiere轻松实现视频的变速（时间重映射）
tags: 
- Premiere
categories: Premiere
date: 2019-10-03 14:42:00
thumbnail: /images/gallery/-6e78d66b1cad8f22.jpg # 略缩图（记得加/）
---
&emsp;&emsp;原来自己在Premiere中调整视频速度都是通过直接改变，就像这样：
![image.png](https://upload-images.jianshu.io/upload_images/14271401-842b0c8f4c7fdd09.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![image.png](https://upload-images.jianshu.io/upload_images/14271401-8c45c7050e0e7ba3.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
&emsp;&emsp;可是这样调整出来的视频变速都是突变的，没有过度，很不自然。今天也在网上看了很多资料，最后我发现了一个改变视频速度的很牛逼的选项：**时间重映射**。
&emsp;&emsp;那今天呢，我就来教大家如何用Premiere中的**时间重映射**来实现视频的变快变慢。
#### 1、导入素材
#### 2、放大视频轨道方便后续操作
![image.png](https://upload-images.jianshu.io/upload_images/14271401-cb75a7c2d097c078.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
#### 3、打开时间重映射
&emsp;&emsp;右击**fx**
![image.png](https://upload-images.jianshu.io/upload_images/14271401-200ee8b33b4b502c.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![image.png](https://upload-images.jianshu.io/upload_images/14271401-3438e21f97b33d42.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


#### 4、找到变速的入点和出点并打上关键帧
![image.png](https://upload-images.jianshu.io/upload_images/14271401-62734226082bf3e0.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
两处关键帧已打好：
![image.png](https://upload-images.jianshu.io/upload_images/14271401-19efb55f636abe74.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
#### 5、调整视频速度
&emsp;&emsp;上下拖动中间的**时间线**即可改变视频的速度，同时系统还会给出此时的变速比例，方便大家对速度的掌控。
&emsp;&emsp;我这里需要的效果是速度减慢，因此我将两处关键帧中间的时间线向下拖动（减速）。
![image.png](https://upload-images.jianshu.io/upload_images/14271401-13d0525d6f6bc816.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

#### 6、设置变速过度
&emsp;&emsp;之前打下的两个关键帧都是可以“分开的”，且视频的速度过度也是通过拉扯关键帧来实现。
![image.png](https://upload-images.jianshu.io/upload_images/14271401-dadd7372e5ea016d.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![image.png](https://upload-images.jianshu.io/upload_images/14271401-bdd893a32fb146e7.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
&emsp;&emsp;如图所见，被拉开的关键帧中间的时间线是倾斜的，这也就表示视频速度已经有了初步的过度。可是浏览过后依旧觉得有点瑕疵，不是那么“丝滑”，那如何将过度变得丝滑呢？
![image.png](https://upload-images.jianshu.io/upload_images/14271401-0d9c880a7b7a4df0.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![image.png](https://upload-images.jianshu.io/upload_images/14271401-aab7e36dd1a4a1ff.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
&emsp;&emsp;至此，视频的变速教程已经结束。
---
##### 7、光流法渲染（给视频减速）
&emsp;&emsp;如果你在预览发现视频在减速后变得一卡一卡的，那是因为大家在给视频减速的过程中**时间插值**默认的是**帧采样**。**帧采样**在给视频加速的时候没有什么影响，但是如果给视频减速，如我上面的情况，就很容易出现一卡一卡的情况。那么该如何解决这种情况呢？
&emsp;&emsp;此时就要用到**光流法渲染**来给视频补帧，达到真正的丝滑柔顺效果。
![image.png](https://upload-images.jianshu.io/upload_images/14271401-5bdfbc8eaef77688.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
&emsp;&emsp;设置之后先不要着急播放预览，因为此时的视频还没有渲染，大家看到的还是原来的**帧采样**模式。
![image.png](https://upload-images.jianshu.io/upload_images/14271401-dfd48c7eaf8cab33.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![image.png](https://upload-images.jianshu.io/upload_images/14271401-d536fb052e0a3c0c.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
![image.png](https://upload-images.jianshu.io/upload_images/14271401-44e2562c9da86a70.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
---
&emsp;&emsp;至此，Premiere利用**时间重映射**轻松实现视频的变速的教程已经结束。
&emsp;&emsp;最后，希望大家能早日制作出属于自己的大片！！！
