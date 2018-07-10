# loading.js

H5页面加载插件

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
