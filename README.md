# loading.js

H5页面加载插件

在移动端的活动页面中，一般会有大量的图片资源，为了让用户在使用过程中更流畅，一般会采用资源预加载的方式，同时在加载资源的时候给予一定的进度提示，这样用户既不会在等待的过程中感到枯燥，也不会在页面使用中出现资源及时加载卡顿的情况。

在下面的对比图中，左侧是没有采用任何预加载处理，右侧是使用了loading预加载图片。可以清晰的看到，右侧的效果虽然用户看到真正的内容相对比较晚，但是整个的体验会更顺畅一些；而左侧的效果，从视线上来讲更跳跃性。

![对比效果](https://github.com/nfer/loading.js/raw/master/compare.gif)

## 使用方法

```
npm install loading.js --save

const loading = require('loading.js');

const imgs = [...];
function loadingCallback(percent, done) {
    // do something with percent and done
}
loading(imgs, loadingCallback);
```
