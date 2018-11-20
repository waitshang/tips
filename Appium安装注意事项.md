# Appium安装注意事项

- 遇到chromedriver下载不动的情况，将安装命令变为`npm install -g appium --chromedriver_cdnurl=http://cdn.npm.taobao.org/dist/chromedriver`，该命令表示使用淘宝CDN加速chromedriver的下载，其他的不变。\[[npm 安装 chromedriver 失败的解决办法](https://segmentfault.com/a/1190000008310875)\]
- 安装过程出现heapdump+node-gyp错误的时候，使用管理员权限执行`npm install --global --production windows-build-tools`，完成后再次安装。\[[使用node heapdump](http://www.cppblog.com/zdhsoft/archive/2017/02/23/214693.html)\]
- 弹出类似`Unsupported platform for fsevents@1.1.3: wanted {"os":"darwin","arch":"any"}`的警告时忽略即可，fsevents仅适用于Mac。\[[报错：Unsupported platform for fsevents@1.1.3: wanted {"os":"darwin","arch":"any"}](https://blog.csdn.net/time888/article/details/79013036)]

[1]: https://www.v2ex.com/t/406002	"设置 http_proxy 和 https_proxy 全局环境变量"
[2]: https://blog.csdn.net/yanzi1225627/article/details/80247758	"npm设置和取消代理的方法"

