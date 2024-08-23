# Readme

![im](https://github.com/Kiumb1223/img_store/blob/master/Dji_DataProcess.png)

## 1. Environment Configuration

```
python == 3.11.5 
pyexiv2 ==2.12.0
```

其他所需要的库直接pip即可，唯独就是读取XMP信息的`pyexiv2`库最新版本`2.14.0`会导致程序崩溃。

我在win10以及win11的jupyterBook上测试了一下，版本`2.14.0`会导致程序崩溃，不太清楚原因。后来降低了一个版本，才能成功运行

## 2. Necessary Explanation

网络上关于DJI数据的暗角补偿等实现资料比较少，自己在复现过程中，遇到了一些问题，所幸这些都被我解决了。所以还是很有必要分享下我的实现，方便代码复用，提升开发效率。

* [大疆M3M/P4M 航拍图像辐射定标流程及python实现_大疆 calibrated optical centerx-CSDN博客](https://blog.csdn.net/weixin_43080939/article/details/129757681) 中也有相关实现，但是，我的实现比该博客中的实现时间复杂度更低，尤其是当图片尺寸越大时，越明显。

- 更多的文字信息，可以继续查看[DjiProcess.ipynb](DjiProcess.ipynb)
