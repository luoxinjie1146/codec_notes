# [JPEG](https://blog.csdn.net/my_happy_life/article/details/82997597) overview

* 将原始图像分为8*8的小块, 每个block里有64pixels。
* 将图像中每个8*8的block进行DCT变换。
* 编码
  * DC分量
    * [DPCM编码](https://blog.csdn.net/gwhcsdn/article/details/71597342)
      * 以左侧像素点作为预测值
      * 量化系数不变
  * AC分量：RLC编码
    * Zig-Zag排列
    * 假设RLC编码之后得到了一个（M,N）的数据对，其中M是两个非零AC系数之间连续的0的个数（即，行程长度），N是下一个非零的AC系数的值
  * VLI编码
  * 熵编码：[Huffman编码](https://baike.baidu.com/item/%E5%93%88%E5%A4%AB%E6%9B%BC%E7%BC%96%E7%A0%81/1719730?fromtitle=HUFFMAN%E7%BC%96%E7%A0%81&fromid=364674&fr=aladdin)
    * 静态霍夫曼编码
    * 动态霍夫曼编码