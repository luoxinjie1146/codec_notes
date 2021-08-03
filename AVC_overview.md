# H.264/AVC overview

## [帧内编码](https://blog.csdn.net/shaqoneal/article/details/77203414)

* 预测编码
  * 4x4亮度分量预测
    * 垂直模式
    * 水平模式
    * DC模式
    * 左下模式
    * 右下模式
    * 右垂直模式
    * 下水平模式
    * 做垂直模式
    * 上水平模式
  * 色度分量与16x16亮度分量
    * 垂直模式
    * 水平模式
    * 均值模式
    * 平面模式
* [PCM编码](https://blog.csdn.net/xietingcandice/article/details/41646311)：编码器直接传输图像的像素值，而不经过预测和变换。