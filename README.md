# SimpleValine,Based on [Valine](https://valine.js.org)

https://ashin.wang 评论框架采用 [Valine](https://valine.js.org)，非常喜欢它来搭配 Hexo。

Valine的优点：
+ 不需要注册，支持匿名评论
+ 基于LeanCloud，无广告
+ 支持邮件提醒
+ 多个部署，调用同一个LeanCloud

针对Valine，冒昧再次进行了简化，使其更加简洁。
![](https://tva1.sinaimg.cn/large/006y8mN6ly1g6zg5fxdjgj30mx09gt90.jpg)

## 1.原版的Valine
原版[Valine在这里](https://valine.js.org)，具体的安装使用可参考原作者的 [Valine使用](https://valine.js.org)。

注意 
+ [LeanCloud中国](http://leancloud.cn)，在2019年10月起绑定的域名需要备案，但是可以使用[LeanCloud国际版](http://LeanCloud.app)，个人免费版的加载速度都不快。

原版效果如下
![](https://tva1.sinaimg.cn/large/006y8mN6ly1g6zg3gv8i9j30ke0cwwf1.jpg)

## 2.简化版的SimpleValine
+ 删除 ~~Powered By Valine~~
+ 删除 ~~快来做第一个评论的人吧~~
+ 去掉 ~~网址(http://)~~

效果图如下
![](https://tva1.sinaimg.cn/large/006y8mN6ly1g6zg5fxdjgj30mx09gt90.jpg)

------

## 3.使用简化版的Valine
以Next主题为例，在路径：`blog⁩/⁨themes⁩/⁨next⁩/⁨layout⁩/⁨_third-party⁩/⁨comments/valine.swig`， 修改`valine.swig`第一行为
 ```
 {%- set valine_uri = theme.vendors.valine | default('https://cdn.jsdelivr.net/gh/AshinWang/SimpleValine@v0.1/SimpleValine.min.js') %}
 ```
 + 经过简化后的`Valine.min.js`放在GitHub托管，Repo:[https://github.com/AshinWang/SimpleValine](https://github.com/AshinWang/SimpleValine)


## 4.加入邮箱提醒
直接参考
+ [Valine](https://valine.js.org/notify.html)
+ [Valine Admin 配置手册](https://deserts.io/valine-admin-document/)


