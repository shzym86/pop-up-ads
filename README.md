# 网页广告弹窗效果

实现了图片和视频的网页广告弹窗效果。视频弹窗使用 HTML5 浏览器原生的播放器。

### 功能：

- 利用jquery实现遮罩弹窗的显示和关闭功能。
- 通过cookie控制广告弹窗每天显示一次。
- 视频播放结束后可添加自定义DOM结构及链接地址等。

### 使用：

为了查看和调试 cookie 功能，需要一个本地的服务器环境，这里使用最简单的 `http-server` node 模块，监听 8881 端口。

```
cd pop-up-ads
npm install
npm start
```

运行后访问：[http://localhost:8881](http://localhost:8881)

### 其它

- 为了提升视频播放速度，避免卡顿，建议将视频文件部署在CDN上。
- 如需节省流量，可在 video 标签中配置属性 `preload="none"`，禁止视频自动缓冲。