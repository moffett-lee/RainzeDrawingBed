# RainzeDrawingBed
个人博客图床搭建
### GitHub + jsDelivr + TinyPNG+ PicGo 打造稳定快速、高效免费图床
#### 前言
##### Q：为什么要使用图床呢？什么是图床？

A：写博客文章时，图片的上传和存放是一个问题，有的朋友可能会把图片放到和博客同一个仓库当中，使用相对路径来引用，这样后期维护起来会比较麻烦。还有的朋友会在不同的平台发布同一篇文章，这样一来每个平台都要上传图片，为了解决这些问题，比较推荐的做法是把图片统一上传到一个在线的第三方静态资源库中，我们把这个资源库称为图床，其返回一个图片的URL，使用markdown+图片url的方式写作文章，一次编写，到处使用~

##### Q：图床的选择

A：推荐使用GitHub作为图床，特点是免费、稳定，有一个小缺点是国内访问速度慢，不过没关系，可以使用jsDelivr免费CDN加速。

##### Q：jsDelivr是什么？

A：jsDelivr是国外的一家优秀的公共 CDN 服务提供商，该平台是首个「打通中国大陆与海外的免费CDN服务」，无须担心中国防火墙问题而影响使用。官网：http://www.jsdelivr.com/

### 图床打造
新建GitHub仓库，注意仓库要设置成公开

参照 官方文档 生成一个token密钥

在 这里 下载PicGo，安装完成后打开，图床设置 选 GitHub图床，并填写相应的信息

仓库名：前面新建的仓库，格式：<用户名>/<仓库名>
分支名：填写主分支master即可
Token：前面生成的token密钥
存储路径：按你自己的需求填写
自定义域名：图片上传后，PicGo 会按照 自定义域名+上传的图片名 的方式生成访问链接，此处我们填写jsDelivr的CDN加速地址，格式：https://cdn.jsdelivr.net/gh/<用户名>/<仓库名>

使用https://tinypng.cn/压缩你要上传的图片（如图片已经很小或你有更好的压缩工具可省略这一步）
在PigGo的上传区上传你的图片，到相册一键复制刚刚上传的图片URL，至此，你就可以在你的文章当中愉快的插入图片啦~， 更多功能自己去探索吧~~

### 效果图

![](https://cdn.jsdelivr.net/gh/Ezuy-Lee/RainzeDrawingBed/media/pcGo20210627182151.png)

![](https://cdn.jsdelivr.net/gh/Ezuy-Lee/RainzeDrawingBed/media/picGo20210627182213.png)




