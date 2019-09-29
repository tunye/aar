# aar
在线aar库。



### 一. 依赖结构

skin和swipe为基础库，

core为核心库，依赖skin、swipe。

> 具备recyclerview、supportv7、网络能力（okhttp）、图片加载（glide）、弹性效果计算（facebook-rebound）、转json（fastJson）能力、皮肤管控、左滑返回。
>
> 提供基础Activity、基础列表Activity、api访问、圆形图、圆角图、圆形进度、Ripple效果、下拉加载、自定义toast、运行时状态、刘海屏适配、网络监控。

videocache（不带core）、comment、qrcode、pudding为应用组件库

image-select提供了本地图选取、大图预览、图片截取等能力。



### 二、依赖方式

根gradle添加

```gradle
maven { url "https://raw.githubusercontent.com/tunye/aar/master" }
```

依赖添加

```gradle
implementation 'com.buaa.ct:videocache:1.0.0'
implementation 'com.buaa.ct:image-selector:1.0.0'
implementation 'com.buaa.ct:pudding:1.0.0'
implementation 'com.buaa.ct:qrcode:1.0.0'
implementation 'com.buaa.ct:comment:1.0.0'

implementation 'com.buaa.ct:core:1.0.0'
```



### 三、版本

| 编号 | 名称           | 功能           |   子依赖   | 版本  |
| :--: | -------------- | -------------- | :--------: | :---: |
|  1   | videocache     | 流缓存         |     无     | 1.0.0 |
|  2   | comment        | 评论           |    core    | 1.1.0 |
|  3   | pudding        | 单页面弹框提示 |    core    | 1.0.2 |
|  4   | qrcode         | 二维码         |    core    | 1.0.2 |
|  5   | image-selector | 选图           |    core    | 1.1.1 |
|  6   | core           | 核心           | swipe;skin | 1.1.1 |
|  7   | swipe          | 左滑           |     无     | 1.0.1 |
|  8   | skin           | 皮肤           |     无     | 1.0.0 |



### 四、更新方式

工程目录执行 

```gradle
gradlew uploadArchives
```

