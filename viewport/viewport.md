# viewport_t1.htm
* 只设置initial-scale, 测试时发现会出现从竖屏到横屏的时候会自动放大
* offsetHeight = document.documentElement.offsetHeight - document.body.offsetHeight 减去这个offsetHeight之后还是有一点点滚动条

# viewport_t2.htm
* 禁止用户缩放屏幕后不会出现viewport_t1.htm中从竖屏到横屏的时候会自动放大的问题
* 测试例子是1000 * 400 ， 可以换成其他任意大小，代码里面的所有宽高都要一起换

#参考资料
* [HTML5 height](http://ryanve.com/lab/dimensions)
* [阿里巴巴移动端高清、多屏适配方案](http://www.aliued.com/?p=3166)