# mydnspod(过期)

2019-10-17 左右,dnspod已经更新了新官网,该脚本失效.

[油猴插件地址/安装方式](https://greasyfork.org/zh-CN/scripts/387189-zeusro-%E5%AE%BD%E7%89%88-dnspod-cn)

让 dnspod 适配 1080p 屏幕

## 效果

![img](doc/result.png)

## 实现细节

一开始做的时候有点摸不着头脑,document经常获取不到元素.后来仔细观察发现这个破网站一开始用了 iframe 加载,过一段时间后又把iframe的标记去掉,于是我只能写个函数,监听这种变化.

除此以外,要考虑几个点:

1. 静态页面布局的调整
2. 对点击/修改/取消操作做了事件监听,最大程度对齐

## TODO

1. 适配其他尺寸屏幕(不大可能去实现(逃~))
2. 去掉定时器(请告诉我怎么监听iframe变化)

## 吐槽

域名配置页用了iframe加载来实现局部更新,而且过了一段时间之后iframe会消失,导致开发难度加大;页面布局一会用css,一会用内联CSS,我也是很郁闷.
