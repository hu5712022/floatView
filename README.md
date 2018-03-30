# floatView
floatView

一个基于峰驼函数的流动体验

流动view，当时是为了播放音乐时做的特效，放在recyclerview 和 listview 里很合适哦。

峰驼函数，其实就是高中学的 正态分布函数(高斯函数)，然后自己改装一下来得到想要的峰驼

我这里是这样改装的：
```
  /**
     * 峰驼 函数
     *
     * @param x x值 传0返回最大值
     * @return y 值 0 到 1 之间
     */
    public float camel(float x) {
        // a*b^(-x^2)    a 控制高度   b 控制胖瘦  默认  a=1  b = 10
        float a = 1;
        float b = 10;
        return (float) (a * Math.pow(b, -x * x));
    }
  
```
![avatar](https://raw.githubusercontent.com/hu5712022/floatView/master/floatview.gif)
